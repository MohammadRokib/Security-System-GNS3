### Firewall Configuration <br> <br><br>

The Firewall will have 2 interfaces s1/0 and s1/2. Interface **s1/0** will be connected to **Router-5** and Interface **s1/2** will be connected to **Router-2**.

Initial Firewall terminal commands are given below:
```
conf t

    int s1/0
        ip address 60.0.0.1 255.255.255.252
        no shut
        exit

    int s1/2
        ip address 50.0.0.1 255.255.255.252
        no shut
        exit

    router ospf 1

        network 50.0.0.0 0.0.0.3 area 0
        network 60.0.0.0 0.0.0.3 area 0
        end
```
<br><br>
```
show  ip int brief
```
![1](https://user-images.githubusercontent.com/60141836/209603479-140ddfe4-c14d-4532-83e5-0aa37af55731.png)

<br><br>
```
show  ip route
```
![2](https://user-images.githubusercontent.com/60141836/209603480-9dd6d54c-bfa1-46df-90de-acd763145395.png)

<br><br>
```
show  ip ospf route
```
![3](https://user-images.githubusercontent.com/60141836/209603482-402ca938-863a-49ab-ae9b-034f7b03f24f.png)

<br><br>
```
show  ip ospf int
```
![4](https://user-images.githubusercontent.com/60141836/209603475-4f6b538b-9ccf-431d-86f0-df975f8813a7.png)

<br><br>
```
show  ip ospf neigh detail
```
![5](https://user-images.githubusercontent.com/60141836/209603477-41b292ca-d2c5-45b7-84e7-f00d452236c3.png)

<br><br>


The user of the hacker PC is trying to hack into our Website using Burp Suite<br>
![6](https://user-images.githubusercontent.com/60141836/209617812-a5badce9-9879-4042-920d-fb680acc7004.png)

<br><br>

We can determine it by monitoring all the incoming and outgoing packets from our server PC. We can monitor the packets using Wireshark. To monitor the packets first I'll **Right click** on the link to the server and click on **Start capture**<br>
![7](https://user-images.githubusercontent.com/60141836/209617818-10175bbe-8752-4bed-a844-d2a66244fbde.png)

<br><br>

Click **OK**<br>
![8](https://user-images.githubusercontent.com/60141836/209617820-670bde7b-9d50-478c-b762-7a4ad56508b7.png)

<br><br>

Here we can see an icon looks like an magnifying glass<br>
![9](https://user-images.githubusercontent.com/60141836/209617821-e3904080-6c23-4f7d-aa4f-4011b6171949.png)

<br><br>

Wireshark will start up and we will be able watch all the incoming and outgoing packets<br>
![10](https://user-images.githubusercontent.com/60141836/209617822-00065ca5-bc3b-4f71-a9b6-8751732b487f.png)

<br><br>

Here we can see that a lot of TCP request is comming from **192.16.68.60**, that means this is the Hacker PC. We can filter by its IP address to see all the request coming from it. To do that I'll **Right click** on one request from **192.16.68.60** then click **Apply as filter**->**Selected**<br>
![11](https://user-images.githubusercontent.com/60141836/209617823-470fcbea-8d80-4d17-8ab1-113903b384dc.png)

<br><br>

Now I'll configure the Firewall to block the IP address **192.16.68.60**
```
conf t
    ip access-list extended BLOCK
        deny tcp host 192.16.68.60 host 172.16.68.50
        permit ip any any
        end

conf t
    int s1/0
        ip access-group BLOCK in
        end
```
![12](https://user-images.githubusercontent.com/60141836/209617824-d0a6feb7-81c7-4a5d-b2b7-9dba48acfacc.png)

<br><br>

We can verify the Access List by the command
```
show access-lists
```
![13](https://user-images.githubusercontent.com/60141836/209617827-b7e6eb58-d7d4-4091-adfc-7563b571bfd2.png)

<br><br>

After doing that we can see that there is no new incoming TCP request from the hacker PC<br>
![14](https://user-images.githubusercontent.com/60141836/209617831-8f283ab7-7984-44d8-8ba2-f3c2de248c64.png)
<br><br>

Also the hacker can no longer access our website<br>
![15](https://user-images.githubusercontent.com/60141836/209617835-5c06d585-5652-472b-95f4-c5f88ccc8e40.png)
<br><br>

Thus it can be said that our server is secure.