### Installing GNS3 VM<br> <br><br>

After installing GNS3 and VMware Player we will need GNS3 VM to run the Windows and Kali Linux appliances. To download GNS3 VM first go to this link: [GNS3 VM](https://www.gns3.com/software/download-vm/)<br><br>

After going to this page this page will come up. Here I'll select VMware Workstation and Fusion Download<br>
![1](https://user-images.githubusercontent.com/60141836/209441437-eba2871f-1368-44c2-8515-d4b8d892b383.png)
<br><br>

A download popup will come. I'll click save as and choose the directory where I want to install the file. Then click **Save**<br>
![2](https://user-images.githubusercontent.com/60141836/209441439-82467094-1c6c-4b97-91b7-7f357fadd463.png)
<br><br>

A zip file will be downloaded. I'll extract it by right clicking on it and then **Extract Here** from 7-Zip<br>
![3](https://user-images.githubusercontent.com/60141836/209441441-f3c7b7b3-acc4-4044-8a0c-69f1c0c7db53.png)
<br><br>

Unzipping the zip file<br>
![4](https://user-images.githubusercontent.com/60141836/209441442-27792dcd-9d20-4ed6-a94a-07d6e0fac0ea.png)
<br><br>

After unzipping a file named **GNS3 VM** will be found<br>
![5](https://user-images.githubusercontent.com/60141836/209441445-aaec958f-07ca-48ca-b2aa-78c97abedf37.png)
<br><br>

Then open VMware Player<br>
![6](https://user-images.githubusercontent.com/60141836/209441446-b2e94df7-6b68-4dc4-8dea-f3015fd00166.png)
<br><br>

Click **Player**->**File**->**Open**<br>
![7](https://user-images.githubusercontent.com/60141836/209441448-04beaa17-9b4f-456d-a29b-0366f010ecb7.png)
<br><br>

Then select the GNS3 VM file that has just been extracted, then click **Open**<br>
![8](https://user-images.githubusercontent.com/60141836/209441449-1f77fda5-0049-4a57-9192-857b205117dd.png)
<br><br>

Type **GNS3 VM** in the Name for the new virtual machine field<br>
![9](https://user-images.githubusercontent.com/60141836/209441450-47faa530-3035-4fc3-a96b-3a7d1cb44724.png)
<br><br>

Then GNS3 VM will be imported in VMware. Upon completing we will GNS3 VM in VMware<br>
![10](https://user-images.githubusercontent.com/60141836/209441451-0951088c-4ce6-4344-a0cd-4a5db9fecdbc.png)
<br><br>

Then I'll open GNS3. Here we can see that, there is only one option in Server Summary which is my local pc<br>
![11](https://user-images.githubusercontent.com/60141836/209441452-67893474-634b-4e1a-a1df-5a6f517c81b3.png)
<br><br>

To connect GNS VM with GNS3 first I'll go to **Edit**->**Preferences**<br>
![12](https://user-images.githubusercontent.com/60141836/209441453-fcda9a34-47da-4009-b865-185f6412af88.png)
<br><br>

Then go to GNS3 VM<br>
![13](https://user-images.githubusercontent.com/60141836/209441458-1ec0143c-4f7c-448c-a41b-78cf89dfb127.png)
<br><br>

First check the **Enable the GNS3 VM** option<br>
![14](https://user-images.githubusercontent.com/60141836/209441459-afe3ba2a-3b2c-49df-86ca-315d295f1e67.png)
<br><br>

Then select **VMware Workstation** in **Virtualization engine**<br>
![15](https://user-images.githubusercontent.com/60141836/209441460-35531abb-e6ca-445f-8894-5ceccb02a17d.png)
<br><br>

Select **GNS3 VM** in **Settings** and allocate vCPUs and RAM as per our need then click **Apply**<br>
![16](https://user-images.githubusercontent.com/60141836/209441461-1d2bce65-bb6e-458d-a442-c9e575598ef6.png)
<br><br>

Then we can see that, GNS3 VM in the Servers Summary. Which means our GNS3 VM is successfully connected to GNS3<br>
![17](https://user-images.githubusercontent.com/60141836/209441463-0e63ff14-0f3e-4105-8da8-4922d5ae9461.png)
<br><br>

And now if we go to VMware Player we can see all the information of our GNS3 VM. Here one option says **KVM support available: TRUE**<br>
![18](https://user-images.githubusercontent.com/60141836/209441465-92662c3f-b57a-4a0e-9adf-9ea3a759a9e0.png)
<br><br>
KVM will allow us to run the Windows and Kali Linux appliances in GNS3. But in some installation it might show FALSE for KVM support. This problem specifically occurs in Windows. Because, windows uses Hyper-V for virtualization. But VMware uses VT-x/EPT for virtualization. Hyper-v is normally disabled and VT-x/EPT is enabled or installed while installing VMware. But if it is not then, we have to disable it manually.

To do that, at first we have to search for Turn windows features on or off and open the first option. This page will come up. We can see that Hyper-V is enabled. We have to uncheck this option and click **Ok**<br>
![19](https://user-images.githubusercontent.com/60141836/209441466-54aa445c-74a7-4365-8b87-2f113cf9322b.png)
<br><br>

And then we have to run cmd or powershell as administrator then run this command and restart our computer<br>
![20](https://user-images.githubusercontent.com/60141836/209441468-796624b6-d9c2-44d6-93d0-f116cb22ca05.png)
<br><br>

Finally, after doing all these we can use GNS3 VM inside GNS3 to run Windows and Kali Linux appliances inside GNS3.
