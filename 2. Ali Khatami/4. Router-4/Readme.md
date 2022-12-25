### Router 4 configuration <br> <br><br>

Router-4 will have 3 interfaces f0/0, s1/0 and s1/1.  Interface **f0/0** will be connected to its internal network, **s1/0** will be connected to Router-3 and interface **s1/1** will be connected to Router-1.

Router-4 terminal commands are given below:
```
conf t
    int f0/0
        ip address 172.16.68.193 255.255.255.192
        no shut
        exit

    int s1/0
        ip address 30.0.0.2 255.255.255.252
        no shut
        exit

    int s1/1
        ip address 40.0.0.2 255.255.255.252
        no shut
        exit

    router ospf 1

        network 172.16.68.192 0.0.0.63 area 0
        network 30.0.0.0 0.0.0.3 area 0
        network 40.0.0.0 0.0.0.3 area 0
        end
```
<br><br>
```
show  ip int brief
```
![1](https://user-images.githubusercontent.com/60141836/209476277-1f524f6e-4787-4d71-b16b-6eb9df81ad9e.png)

<br><br>
```
show  ip route
```
![2](https://user-images.githubusercontent.com/60141836/209476278-b6228ddc-d785-4d72-b5dc-0ae658ddd1d8.png)

<br><br>
```
show  ip ospf route
```
![3](https://user-images.githubusercontent.com/60141836/209476280-4792137a-93f9-42aa-87d2-901893cb0e03.png)

<br><br>
```
show  ip ospf int
```
![4 1](https://user-images.githubusercontent.com/60141836/209476281-2857b066-a522-4e1b-beab-7195c9ed4b59.png)
<br>
![4 2](https://user-images.githubusercontent.com/60141836/209476274-74c32dd5-7fd4-4141-bf6d-4a8852ec69f8.png)

<br><br>
```
show  ip ospf neigh detail
```
![5](https://user-images.githubusercontent.com/60141836/209476276-84960f9a-c18b-4b6c-af77-c7ddc4fa5ec8.png)
