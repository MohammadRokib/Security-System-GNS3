### Router 3 configuration <br> <br><br>

Router-3 will have 3 interfaces f0/0, s1/0 and s1/1.  Interface **f0/0** will be connected to its internal network, **s1/0** will be connected to Router-4 and interface **s1/1** will be connected to Router-2.

Router-3 terminal commands are given below:
```
conf t
    int f0/0
        ip address 172.16.68.129 255.255.255.192
        no shut
        exit

    int s1/0
        ip address 30.0.0.1 255.255.255.252
        no shut
        exit

    int s1/1
        ip address 20.0.0.1 255.255.255.252
        no shut
        exit

    router ospf 1

        network 172.16.68.128 0.0.0.63 area 0
        network 20.0.0.0 0.0.0.3 area 0 
        network 30.0.0.0 0.0.0.3 area 0
        end
```
<br><br>
```
show  ip int brief
```
![1](https://user-images.githubusercontent.com/60141836/209476034-3aee8a1b-86db-4286-adc7-06498dcd1699.png)

<br><br>
```
show  ip route
```
![2](https://user-images.githubusercontent.com/60141836/209476031-3fd5e99b-a7bb-42aa-a97f-65c6287b2452.png)

<br><br>
```
show  ip ospf route
```
![3](https://user-images.githubusercontent.com/60141836/209476038-12faab83-b9c7-40df-a34e-8c3d41a5ff5f.png)

<br><br>
```
show  ip ospf int
```
![4 1](https://user-images.githubusercontent.com/60141836/209476037-f0d473bb-6e46-4afd-8467-4aa041bb9d8c.png)
<br>
![4 2](https://user-images.githubusercontent.com/60141836/209476036-25bfc516-c144-4758-8c7f-60053260c7fb.png)

<br><br>
```
show  ip ospf neigh detail
```
![5](https://user-images.githubusercontent.com/60141836/209476035-88c39090-5071-45a4-a8fe-ae629c95946d.png)
