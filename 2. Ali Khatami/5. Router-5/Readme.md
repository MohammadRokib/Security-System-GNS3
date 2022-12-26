### Router 5 configuration <br> <br><br>

Router-5 will have 2 interfaces f0/0 and s1/0.  Interface **f0/0** will be connected to its internal network and interface **s1/1** will be connected to the Firewall.

Router-5 terminal commands are given below:
```
conf t
    int f0/0
        ip address 192.16.68.1 255.255.255.0
        no shut
        exit

    int s1/0
        ip address 60.0.0.2 255.255.255.252
        no shut
        exit

    router ospf 1

        network 192.16.68.0 0.0.0.255 area 0
        network 60.0.0.0 0.0.0.3 area 0
        end
```
<br><br>
```
show  ip int brief
```
![1](https://user-images.githubusercontent.com/60141836/209486168-21509f6d-1c4f-40ff-b33b-5819de571ddf.png)

<br><br>
```
show  ip route
```
![2](https://user-images.githubusercontent.com/60141836/209486169-cc42314b-b1da-4b2b-a577-555e7891d45c.png)

<br><br>
```
show  ip ospf route
```
![3](https://user-images.githubusercontent.com/60141836/209486164-c712802d-275b-48f5-bd12-7cdd39d3f42a.png)

<br><br>
```
show  ip ospf int
```
![4](https://user-images.githubusercontent.com/60141836/209486166-3f0ce23e-90dc-4de8-b05b-66a0e46b00b0.png)

<br><br>
```
show  ip ospf neigh detail
```
![5](https://user-images.githubusercontent.com/60141836/209486167-b6622f4e-0a16-4f4d-b303-d1b66402a120.png)
