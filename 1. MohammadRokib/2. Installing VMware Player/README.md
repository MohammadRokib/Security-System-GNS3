### Installing VMware Workstation Player <br> <br>

VMware Workstation Player, formerly VMware Player, is a virtualization software package for x64 computers running Microsoft Windows or Linux, supplied free of charge by VMware, Inc., a company which was formerly a division of, and whose majority shareholder remains, Dell EMC.

We will use VMware Player to run GNS3 VM in it. We need GNS3 VM to use Windows and Kali Linux appliances. There is a more popular option to use virtual machines which is VirtualBox. But to use appliances in GNS3 we need KVM / nested virtualization support. Even though VirtualBox supports KVM but the support was given to it very recently. So it doesn't support it natively it just simulates it. As a result the appliaces runs very slow in it.

But VMware supports KVM natively thus the appliances runs in it smoothly. That's why we will be using VMware. To install VMware palyer first I will go to this link: [VMware Workstation Player](https://customerconnect.vmware.com/downloads/details?downloadGroup=WKST-PLAYER-1700&productId=1377&rPId=97014/)

Then a page like this will come up. I will download the windows version<br>
![Screenshot (16)](https://user-images.githubusercontent.com/60141836/209432653-a1a87b86-445c-4a29-9f1f-d63305df2bfb.png)
<br><br>

A download pop-up will come then I'll click **Save as** then files will come up and will select the desired folder to download and then click **Save**<br>
![Screenshot (17)](https://user-images.githubusercontent.com/60141836/209432655-b4631489-e3e9-4c2a-936e-0f33c17a461f.png)
<br><br>

This file will be downloaded. I'll double click on it to install it<br>
![Screenshot (18)](https://user-images.githubusercontent.com/60141836/209432656-18f77345-0931-4912-8409-aed7d22fbe63.png)
<br><br>

Installation prompt<br>
![Screenshot (19)](https://user-images.githubusercontent.com/60141836/209432657-70635e1c-9445-40d8-9e5e-3c6f31f659a8.png)
<br><br>

I'll click **Next** here<br>
![Screenshot (20)](https://user-images.githubusercontent.com/60141836/209432658-fdb9757e-4f4c-49d3-be67-f544329ffcd4.png)
<br><br>

Check the **I accept the terms in the license agreement** then click **Next**<br>
![Screenshot (21)](https://user-images.githubusercontent.com/60141836/209432659-9dddf0f1-e97c-44a9-b7bc-edde96ed63e3.png)
<br><br>

**Next**<br>
![Screenshot (22)](https://user-images.githubusercontent.com/60141836/209432660-b859b8d1-785d-414d-80f3-7d2ebfbe602e.png)
<br><br>

**Next**<br>
![Screenshot (23)](https://user-images.githubusercontent.com/60141836/209432662-c01947fb-59fd-4602-89c7-bd8c86e7f0ad.png)
<br><br>

**Next**<br>
![Screenshot (24)](https://user-images.githubusercontent.com/60141836/209432664-68c35f28-6220-417e-8333-e65e90d47094.png)
<br><br>

Then I'll click **Install**<br>
![Screenshot (25)](https://user-images.githubusercontent.com/60141836/209432668-74f85bc9-8c99-4253-be4f-010225a7f6b2.png)
<br><br>

Installing<br>
![Screenshot (26)](https://user-images.githubusercontent.com/60141836/209432671-c801bedb-b9c5-4b5e-a5c5-ddc645f4bba8.png)
<br><br>

After the installation is complete I'll click **Finish**<br> 
![Screenshot (27)](https://user-images.githubusercontent.com/60141836/209432672-07c8fe3c-cb9d-464a-b5a6-6d9f86ba8158.png)
<br><br>

I'll click on the VMware shortcut on the desktop. This window will come up. Here I have to select the first option where it says Use VMware Workstation 17 Player for free for non-commercial use, then click **Continue**<br>
![Screenshot (29)](https://user-images.githubusercontent.com/60141836/209432673-e4398608-03bf-44be-bac7-e28fbf34dca3.png)
<br><br>

Then click **Finish**<br>
![Screenshot (30)](https://user-images.githubusercontent.com/60141836/209432674-f08ece0e-2e68-4fc4-93f5-578c0e34f213.png)
<br><br>

After that the installation is complete. Now we can use VMware Player.<br>
![Screenshot (31)](https://user-images.githubusercontent.com/60141836/209432675-97344b99-66fe-497b-b06d-db998b7d328b.png)
