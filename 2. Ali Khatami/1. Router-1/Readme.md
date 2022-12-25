### Router 1 configuration <br> <br><br>

Router-1 will have 3 interfaces f0/0, s1/0 and s1/1.  Interface **f0/0** will be connected to its internal network, **s1/0** will be connected to Router-2 and interface **s1/1** will be connected to Router-4.

Router-1 terminal commands are given below:
```
conf t
    int f0/0
        ip address 172.16.68.1 255.255.255.192
        no shut
        exit

    int s1/0
        ip address 10.0.0.1 255.255.255.252
        no shut
        exit

    int s1/1
        ip address 40.0.0.1 255.255.255.252
        no shut
        exit

    router ospf 1

        network 172.16.68.0 0.0.0.63 area 0
        network 10.0.0.0 0.0.0.3 area 0 
        network 40.0.0.0 0.0.0.3 area 0
        end
```
<br><br>
```
show  ip int brief
```
![1](https://user-images.githubusercontent.com/60141836/209469401-6e2e259c-6b31-4c3d-b9f9-ecd4f5ac0509.png)

<br><br>
```
show  ip route
```
![2](https://user-images.githubusercontent.com/60141836/209469402-6433cc8c-68f6-4f41-94a8-7c5bbf0ac310.png)

<br><br>
```
show  ip ospf route
```
![3](https://user-images.githubusercontent.com/60141836/209469403-3d203f70-ece7-4965-b495-bf04c3e6aec4.png)

<br><br>
```
show  ip ospf int
```
![4 1](https://user-images.githubusercontent.com/60141836/209469404-782163ff-e892-4c15-b304-54941f98f1de.png)
<br>
![4 2](https://user-images.githubusercontent.com/60141836/209469406-db80149a-2011-4537-b8ee-16cb062b6b10.png)

<br><br>
```
show  ip ospf neigh detail
```
![5](https://user-images.githubusercontent.com/60141836/209469409-733bfaf1-f609-482a-8d9a-57a68f1f2648.png)
