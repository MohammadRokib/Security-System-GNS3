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

Lastly I'll check the IP address through this command.
```ipconfig```<br>
![10](https://user-images.githubusercontent.com/60141836/209491613-076d6bee-cf77-4c52-848b-423006d242af.png)
<br><br>


Similarly I'll give the Kali Linux appliances static IP address. At first **Right Click** on the appliance then click **Start** to trun on tha appliance<br>
![1](https://user-images.githubusercontent.com/60141836/209498575-d33708c9-0467-4956-b74f-1bb48a8a4d65.png)
<br><br>

Then **Right Click** again and click **Console** to use the start up<br>
![2](https://user-images.githubusercontent.com/60141836/209498578-e29f8888-66ac-414d-9e3e-4710d94077f7.png)
<br><br>

A VNC window will come up. From here we have to choose the **Live USB Persistence** option and click **Enter**<br>
![3](https://user-images.githubusercontent.com/60141836/209498550-0e5dabf2-585e-4d58-8946-954a9e584428.png)
<br><br>

The Kali Linux appliance will start up. Here I'll click on the top right corner<br>
![4](https://user-images.githubusercontent.com/60141836/209498557-02193337-eabc-4f35-ae09-12a69bf217af.png)
<br><br>

A drop down menu will appear then click **Ethernet** and then click **Wired Settings** from the drop down menu<br>
![5](https://user-images.githubusercontent.com/60141836/209498560-dc7e3f92-5fc0-49c8-8039-79c6edae8362.png)
<br><br>

It will go to the network settings page. Here I'll click on the settings logo on right side of **Ethernet (eth0)**<br>
![6](https://user-images.githubusercontent.com/60141836/209498561-4fffde14-a05e-4a3a-b652-7ac0c31e2adb.png)
<br><br>

Go to **IPv4** tab on the new window. Here we can see **Automatic (DHCP)** is selected by default<br>
![7](https://user-images.githubusercontent.com/60141836/209498564-b32a2082-a841-476e-aed2-a87a8cd9b3d4.png)
<br><br>

I'll choose **Manual** and define the IP address, Netmask and Gateway<br>
![8](https://user-images.githubusercontent.com/60141836/209498566-d77b72f5-5b21-4431-b405-58762567a19e.png)
<br><br>

I can verify it by running the command ```ifconfig``` in the terminal<br>
![9](https://user-images.githubusercontent.com/60141836/209498568-e28e8e9e-e2a9-4a92-a7d1-4f632216cf0b.png)
<br><br>

I'll do the same for the second Kali Linux appliance and define IP address, Netmask and Gateway for it<br>
![10](https://user-images.githubusercontent.com/60141836/209498570-34f18cb9-5d1e-48e0-92ee-3d8caf4ff871.png)
<br><br>

Again I can verify it by the command ```ifconfig```<br>
![11](https://user-images.githubusercontent.com/60141836/209498573-9f9cc6f6-b617-4d9c-91d3-46a1e9d03fdb.png)
<br><br>