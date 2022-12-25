### Router 2 configuration <br> <br><br>

Router-2 will have 4 interfaces f0/0, s1/0, s1/1 and s1/2.  Interface **f0/0** will be connected to its internal network, **s1/0** will be connected to Router-2 and interface **s1/1** will be connected to Router-4 and interface **s1/2** will be connected to the firewall.

Router-2 terminal commands are given below:
```
conf t

	int f0/0
		ip address 172.16.68.65 255.255.255.192
		no shut
		exit

	int s1/0
		ip address 10.0.0.2 255.255.255.252
		no shut
		exit

	int s1/1
		ip address 20.0.0.2 255.255.255.252
		no shut
		exit

	int s1/2
		ip address 50.0.0.2 255.255.255.252
		no shut
		exit

	router ospf 1

		network 172.16.68.64 0.0.0.63 area 0
		network 10.0.0.0 0.0.0.3 area 0
		network 20.0.0.0 0.0.0.3 area 0
		network 50.0.0.0 0.0.0.3 area 0
		end

```
<br><br>
```
show  ip int brief
```
![1](https://user-images.githubusercontent.com/60141836/209475671-187256ab-92e3-43b7-91f4-583eea41cdf9.png)

<br><br>
```
show  ip route
```
![2](https://user-images.githubusercontent.com/60141836/209469402-6433cc8c-68f6-4f41-94a8-7c5bbf0ac3

<br><br>
```
show  ip ospf route
```
![3](https://user-images.githubusercontent.com/60141836/209475675-bebbd564-0ea5-4ebc-a767-3b438cae11a2.png)

<br><br>
```
show  ip ospf int
```
![4 1](https://user-images.githubusercontent.com/60141836/209475674-51c01e27-54d9-48bc-9f7a-d62cf92c7958.png)
<br>
![4 2](https://user-images.githubusercontent.com/60141836/209475673-fc4da810-14dc-416a-b2c6-4b0f5bd432eb.png)

<br><br>
```
show  ip ospf neigh detail
```
![5](https://user-images.githubusercontent.com/60141836/209475672-204af5b8-99c1-4e99-a2a4-84638128aa39.png)
