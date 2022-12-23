### Security System for a Topology built in GNS3

Assalamu Alaikum everyone,
In this project We have built a security system on a topology/network inside GNS3 to prevent it from Cyber attack such as **SQL Injection** and so on.

Now a days all Website, Apps we use by connecting to the internet are vulnerable to many cyber attacks. As a result all our public and private data are going in the wrong hands. Data breach like these can cause many problems to us. So to prevent problems like these we have to take some masures.

So we have built a topology consists of 4 routers which contains their own network consisting one switch and a PC. One of the PC is acting as a Web Server.

![Screenshot (341)](https://user-images.githubusercontent.com/60141836/209249862-8caa91a6-0d15-4aeb-9875-f4f7729b685a.png)
<br><br>

The web server in the Windows 10 PC
![Screenshot (1)](https://user-images.githubusercontent.com/60141836/209259241-fd617943-fd10-458a-89aa-3df87c3b1399.png)
<br><br>

Then we hacked into an account. Using Burpsuite in Kali Linux
![Screenshot_2022-12-09_12_34_29](https://user-images.githubusercontent.com/60141836/209259394-a9f53a5d-61ad-4989-a7b2-ad2f14ef7cc1.png)
<br><br>

And lastly we blocked the hacker from using the server by TCP blocking with a router acting as Firewall
![Screenshot from 2022-12-23 08-35-06](https://user-images.githubusercontent.com/60141836/209259735-7615e7df-0343-40b7-a14f-da597e0f83ab.png)
<br><br>

Description of each step is given in the folders above.
<br>
<br> <br>

**Team: Elation** <br>
**Members:**
1. *Ali Khatami (Leader)* [Router configuration, Topology]
2. *Md. Rafidul Islam* [Hacking]
3. *Md. Hasanur Rohoman Khan* [Firewall]
4. *Md. Rokib Khan* [Initial setup, Connecting all portions together]
5. *Md. Arafatul Islam* [Website, Making the Website live]
