### Installing Windows & Kali Linux appliances<br> <br><br>

After installing GNS3 and VMware Player and GNS3 VM now I'll install the appliances.
At first I'll install the Windows appliance. To do that first I'll open GNS3. After opening GNS3 click on the logo which looks like a monitor on the left. This is the **End devices** tab.

We can find a window like this. Click on the **+New template** button here<br>
![1](https://user-images.githubusercontent.com/60141836/209454941-651b04ba-0f0c-46e4-9925-c6bd737e75ca.png)
<br><br>

Click **Next**<br>
![2](https://user-images.githubusercontent.com/60141836/209454942-f120bad0-7fca-4627-83ae-7bd15e6b7a96.png)
<br><br>

Double click on the **Guests** options<br>
![3](https://user-images.githubusercontent.com/60141836/209454944-a5b2badb-79cc-4dd4-a235-119fe9a6fc50.png)
<br><br>

We can see all the guest appliances here<br>
![4](https://user-images.githubusercontent.com/60141836/209454946-a03bbe03-9d60-4f7f-b406-cf658342f787.png)
<br><br>

Then go down to find the Windows appliance and click **Install**<br>
![5](https://user-images.githubusercontent.com/60141836/209454947-a1c1b320-6a5b-4e2f-8228-0f7a5676e9f9.png)
<br><br>

Click **Next**<br>
![6](https://user-images.githubusercontent.com/60141836/209454949-819fe660-e646-47d3-92af-e916b8a4c919.png)
<br><br>

**Next**<br>
![7](https://user-images.githubusercontent.com/60141836/209454950-a2ab6b01-947c-4ec1-af27-18cdb4c3abcb.png)
<br><br>

We can see all the Windows versions here. We will download the first one. After selecting it I'll click **Download** on the bottom<br>
![8](https://user-images.githubusercontent.com/60141836/209454952-abb726f3-824c-44a2-bda7-f8c368779718.png)
<br><br>

Click **Ok**<br>
![9](https://user-images.githubusercontent.com/60141836/209454953-f71e7b70-2b50-4e18-8f0f-58d7c5a673bf.png)
<br><br>

This page will open. Select last one from the **Virtual Machines**<br>
![10](https://user-images.githubusercontent.com/60141836/209454956-9c2d618b-57cd-4f24-85b7-e433a2aeea75.png)
<br><br>

Then select **VMware** from **VM platform**<br>
![11](https://user-images.githubusercontent.com/60141836/209454957-e22ace75-32c5-4556-aead-ee72a6059280.png)
<br><br>

Then click **Download**<br>
![12](https://user-images.githubusercontent.com/60141836/209454958-2e44704f-32f8-4aef-8bc8-86b49eb8c443.png)
<br><br>

Download prompt will come up. Then click **Save as** and then choose the destination folder and click **Save**<br>
![13](https://user-images.githubusercontent.com/60141836/209454959-e808cd88-c5b3-4567-bbcb-c2d8337d883d.png)
<br><br>

This file will be downloaded. Then we will extract the file<br>
![14](https://user-images.githubusercontent.com/60141836/209454960-1aa7c449-1992-43d1-b600-9d9c0e98dc79.png)
<br><br>

Extracting<br>
![15](https://user-images.githubusercontent.com/60141836/209454961-460d7a96-3ab9-4d7a-85f1-06b674b95470.png)
<br><br>

We will get this file after extracting<br>
![16](https://user-images.githubusercontent.com/60141836/209454962-1788d61a-bce2-406a-a2eb-00134143969d.png)
<br><br>

The extracted file contains these 3 files. We just need the last one<br>
![17](https://user-images.githubusercontent.com/60141836/209454963-e599c33f-5cea-488f-8b62-67005e2cbd47.png)
<br><br>

Then I'll come back to this page, select the file we just downloaded then click **Import** in the bottom left corner<br>
![18](https://user-images.githubusercontent.com/60141836/209454964-c438dafc-e90e-4c6f-8dc0-0556109f4d36.png)
<br><br>

Then select the file I just downloaded and click **Open**
![19](https://user-images.githubusercontent.com/60141836/209454965-0fa6d919-6824-462d-88b8-6ff8838f14c0.png)
<br><br>

It will start importing in GNS3<br>
![20](https://user-images.githubusercontent.com/60141836/209454966-68a0135e-4ddb-40e7-86bb-975ee64ed8f5.png)
<br><br>

After completing the import we can see that Windows is ready to install. I'll click **Next**<br>
![21](https://user-images.githubusercontent.com/60141836/209454967-1f431125-68cb-4ba4-8d5c-f71676ce3869.png)
<br><br>

Click **Yes**<br>
![22](https://user-images.githubusercontent.com/60141836/209454968-ad820521-1286-4548-aa03-968fbb30caf2.png)
<br><br>

We can see the default username and password for the Windows appliance. Then click **Finish**<br>
![23](https://user-images.githubusercontent.com/60141836/209454970-be8d42a3-f13a-44dd-9f37-bcdc0516002a.png)
<br><br>

We can see the Windows appliance on the left in the **End devices** tab<br>
![24](https://user-images.githubusercontent.com/60141836/209454971-4e22c8cc-e3a5-49e2-bfa2-e023c7c4c6f9.png)
<br><br>


Similarly I'll install the Kali Linux appliance. I'll select Kali Linux appliance from the guest appliances and click **Install**<br>
![1](https://user-images.githubusercontent.com/60141836/209456061-2a4b8f69-3ec7-4457-b2d0-9c0c7033bc33.png)
<br><br>

Click **Next**<br>
![2](https://user-images.githubusercontent.com/60141836/209456064-97da3e5f-2039-4776-8b25-d4a4cf730b80.png)
<br><br>

**Next**<br>
![3](https://user-images.githubusercontent.com/60141836/209456065-ef9738d9-b43e-4df3-b94d-320f2a5053a1.png)
<br><br>

We need 2 files for the Kali Linux appliance. First I'll download them select the file and then click **Download** on the bottom<br>
![4](https://user-images.githubusercontent.com/60141836/209456066-4ecf2b21-936b-4d48-bc24-5278338d0c61.png)
<br><br>

**Save as**->**Select the destination folder**->**Save**<br>
![5](https://user-images.githubusercontent.com/60141836/209456068-fb74e4f3-77a3-4576-a08b-4413a44eb4d4.png)
<br><br>

Then I'll download the second file. Select the file and click **Download** on the bottom<br>
![6](https://user-images.githubusercontent.com/60141836/209456069-83594a24-e8cd-4963-be0e-498d49aeb19a.png)
<br><br>

It will land on then this page. Download will start automatically<br>
![7](https://user-images.githubusercontent.com/60141836/209456070-884f6f84-22cc-4731-88fe-aeb3c167da21.png)
<br><br>

**Save as**->**Select the destination folder**->**Save**<br>
![8](https://user-images.githubusercontent.com/60141836/209456071-1efd6e61-805b-4d48-9801-38fde435ea96.png)
<br><br>

These 2 files will be downloaded<br>
![9](https://user-images.githubusercontent.com/60141836/209456073-c2a90899-a5b6-4c9a-91a6-3b690dfb32ea.png)
<br><br>

Then I'll import the first file. Select the file and click **Import** on the bottom<br>
![10](https://user-images.githubusercontent.com/60141836/209456074-682855b4-546d-4456-9c93-69301512ada6.png)
<br><br>

Select the file  from files and click **Open**<br> 
![11](https://user-images.githubusercontent.com/60141836/209456075-dce8675b-7741-414a-bbd9-1f0062fe88d4.png)
<br><br>

The file will start importing<br>
![12](https://user-images.githubusercontent.com/60141836/209456076-9e20b973-6e32-4ca4-a6fd-56937f3f4363.png)
<br><br>

After the import is complete I'll import the second file<br>
![13](https://user-images.githubusercontent.com/60141836/209456077-9707d4ad-968a-493e-80a1-ae57be6f49fe.png)
<br><br>

Select the file and click **Import** on the bottom<br>
![14](https://user-images.githubusercontent.com/60141836/209456078-d3d5b694-f4cd-4bbe-8097-2243a7918abc.png)
<br><br>

Select the file from files and click **Open**<br>
![15](https://user-images.githubusercontent.com/60141836/209456079-8efcc492-438b-4c77-8f10-69ce3ffadfa0.png)
<br><br>

After importing both files we can see that Kali Linux is ready to install. Click **Next**<br>
![16](https://user-images.githubusercontent.com/60141836/209456080-fab7a914-ae4e-482e-96bc-c6dce4381f7f.png)
<br><br>

Click **Yes**<br>
![17](https://user-images.githubusercontent.com/60141836/209456081-a79d3bd6-5df3-46d5-b49d-f258a1384a82.png)
<br><br>

We can see  the default password for the Kali Linux appliance. Click **Finish**<br> 
![18](https://user-images.githubusercontent.com/60141836/209456082-74224f5f-d051-4bc9-9922-47377b9fe9fa.png)
<br><br>

Click **Ok**<br>
![19](https://user-images.githubusercontent.com/60141836/209456083-fa1717a3-2b10-4c04-95c3-36ac7873c78c.png)
<br><br>

We can see the Kali Linux appliance on the left in the **End devices** tab<br>
![20](https://user-images.githubusercontent.com/60141836/209456084-4e44e773-0023-4874-97eb-7383608db26d.png)
<br><br>

After installing both Windows and Kali Linux appliances we can use them in our topology.
