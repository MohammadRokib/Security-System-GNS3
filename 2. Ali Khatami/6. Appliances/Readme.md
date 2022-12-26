### Windows and Kali Linux configuration <br> <br><br>

The next part of our topology is to set up the appliances, give them static ip address. I'll start with the Windows appliance first.

At first go to GNS3 and open the project. **Right Click** on the Windows appliance and click **Start**. The appliance will turn on.<br>
![1](https://user-images.githubusercontent.com/60141836/209491615-387a3c25-fc1d-4907-8f46-5e467e453913.png)
<br><br>

Again **Right Click** on the Windows appliance and click **Console**.<br>
![2](https://user-images.githubusercontent.com/60141836/209491617-3996b8cd-3799-4f1c-a94a-1caf59363693.png)
<br><br>

The appliance will start running in VNC. Then click on the network logo in the bottom right corner.<br>
![3](https://user-images.githubusercontent.com/60141836/209491619-f10b62fe-1fcd-4daa-9859-0f4e1495197e.png)
<br><br>

A small window will come up. Then I'll click on **Network & Internet settings**<br>
![4](https://user-images.githubusercontent.com/60141836/209491621-925f12e1-37e5-4362-a03f-e1d9e2448d4b.png)
<br><br>

This page will come up. Now I'll click on **Change adapter options**<br>
![5](https://user-images.githubusercontent.com/60141836/209491599-5f7b1cbf-a979-45bd-8598-963e0b3debab.png)
<br><br>

Network connections page will come up. We can see our ethernet device. **Right Click** on it then click **Properties**<br>
![6](https://user-images.githubusercontent.com/60141836/209491605-c366a2b4-79a9-48c5-9584-56849ffdefc6.png)
<br><br>

Ethernet Properties window will come up. Here we will select **Internet Protocol Version 4(TCP/IPV4)** and click on **Properties**<br>
![7](https://user-images.githubusercontent.com/60141836/209491607-cd4694f3-3f30-4a4a-bfca-8878ae522011.png)
<br><br>

A new window will come up. We will select **Use the following IP address**.<br>
![8](https://user-images.githubusercontent.com/60141836/209491609-6f744b2c-3ec7-462c-9465-85901d5e2dc7.png)
<br><br>

And then we will give it a static IP address. I'll define the IP address, Subnet mask, Default gateway and the Preferred DNS server<br>
![9](https://user-images.githubusercontent.com/60141836/209491611-1221d9ce-02fd-47fe-861b-9061807e69a6.png)
<br><br>

Lastly I'll check the IP address through this command: ```ipconfig```<br>
![10](https://user-images.githubusercontent.com/60141836/209491613-076d6bee-cf77-4c52-848b-423006d242af.png)
<br><br>