### Hacking Portion of the project <br> <br><br>

Assalamualaikum, I'm Mohammad Rafidul Islam. We are working on a project where we are trying to build a security system on a topology inside GNS3 to protect it from **Cyber Attack**. I have performed the cyber attack portion of the project.<br><br>

I have used Kali Linux for the Cyber Attack.
![1  Kali Linux](https://user-images.githubusercontent.com/120240771/207899133-cdf52c0a-4af3-47e8-a3c7-9dff88113dcf.png)
<br><br>

The software which I have used for the attack is Burp suite community edition. It comes free with Kali Linux
![2  Burp Suite](https://user-images.githubusercontent.com/120240771/207899519-7c0a7e45-9682-4c4f-83e4-aab5fd9825e2.png)
<br><br>

I will go through the initial setup
![3   Bup Suite](https://user-images.githubusercontent.com/120240771/207903083-f13211ef-2f4e-4b35-9896-bbf18a7bf9b5.png)
<br>
![4  Burp Suite](https://user-images.githubusercontent.com/120240771/207903119-c592ad59-676d-4d73-9340-f23929d209f4.png)
<br><br><br>

After finishing up the initial setup we will go to the **Proxy** tab and click the orange **Open Browser** button.
![5  Proxy tab](https://user-images.githubusercontent.com/120240771/207903698-83e195c4-556a-4350-84e6-c486d720ce02.png)
<br><br>

Then a browser will open up, I will then give the address of the Website I want to hack which is **192.168.0.107/cn** in my case. A log in page will appear after giving this address.
![6  Log in](https://user-images.githubusercontent.com/120240771/207904339-16e432d0-a0d6-4962-ba8b-6ffb424d3672.png)
<br><br>

Then I will go to Burp Suite again and click the **Intercept On** button.
![7  Intercept on](https://user-images.githubusercontent.com/120240771/207904717-4711855f-68c5-4206-b387-56e4a6a34df7.png)
<br><br>

Then I will go back to the Log In page and give a legitimate Username and a random password as I don't know it.
![8  Random password](https://user-images.githubusercontent.com/120240771/207905153-36f42732-a807-4919-838c-feb046174370.png)
<br><br>

After that the site will be intercepted by burp suite. Burp suite will come up with the HTML code of the page.
![9  Site intercepted](https://user-images.githubusercontent.com/120240771/207906128-e1c6e5d0-aac2-4001-a5f9-98c81785f2de.png)
<br><br>

Then I will right click and from the options I will select **send to Repeater**. In the Burp Suite the Repeater tab will open with the HTML code of the Log In Page.
![10  Send to repeater](https://user-images.githubusercontent.com/120240771/207907025-f2876578-950b-4066-8058-49f9d91068b6.png)
<br><br>

In the code after password I will give the sql injection code and click the orange button in the upper left corner which says **Send**. But I will get wrong password message in the **Response** tab in the right.
![11  Trying injection](https://user-images.githubusercontent.com/120240771/207907909-69978ea0-42b3-4d29-8d84-14cd775269d4.png)
<br><br>

Since the injection code is not working I will test if the Page is injectable or not. To do that first I will copy the codes from the repeater tab of Burp suite.
![11  Copying the files](https://user-images.githubusercontent.com/120240771/207908377-9f9aa02c-c7a8-405a-bdbc-d011c4332eae.png)
<br><br>

Then I'll create a file named injection and open it with mousepad
![12  Injection file](https://user-images.githubusercontent.com/120240771/207908676-c4c214b6-2826-49dd-9758-aefa45f6aeee.png)
<br><br>

After that I'll paste the copied data in the injection file that I have just created.
![13  Pasting into injection](https://user-images.githubusercontent.com/120240771/207908981-6d9003d6-0c59-4949-a425-b68f665c02a4.png)
<br><br>

Then I'll type the command *"sqlmap -r injection -p username"* to check if the password is injectable. But I found that the username is not injectable.
![14  Testing if injectable](https://user-images.githubusercontent.com/120240771/207910703-51f36bd9-cfae-403b-b2ac-dab9a01961bd.png)
<br><br>

Then I'll type another command *"sqlmap -r injection -p password"* to check if the password is injectable.
![15  Testing if injectable](https://user-images.githubusercontent.com/120240771/207911092-88b296e0-57dd-4f80-8a12-0d292b673aef.png)
<br><br>

But I also found that the password is also not injectable.
![16  Testing if injectable](https://user-images.githubusercontent.com/120240771/207911285-9ae38063-3830-4600-9cb1-77784d08feba.png)
<br><br><br><br>

Not completed yet.....
