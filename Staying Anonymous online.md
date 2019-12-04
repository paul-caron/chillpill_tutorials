Staying Anonymous online
========================
Why stay anonymous ?
----
<i>“Arguing that you don’t care about the right to privacy because you have nothing to hide is no different than saying you don’t care about free speech because you have nothing to say.”</i> `Edward Snowden` 
 
This quote makes you think about your right to privacy , and rightly so it should . The data is the new oil , whoever has information about you knows you 
more than you do yourself . They can analyze it and profile you and use it to influence you through targeted ad campaigns , political campaigns, persecute you.This is not far fetched but it is a reality that we might have not faced yet.

Apart from organizations , we might be stigmatized by the society . A teacher was forced to quit her job as she posted her pictures of vacation in Europe , where she was drinking alcohol in places that would be tame and acceptable yet she was forced to resign.
   
`DuckduckGo search : Ashley Payne - A Georgian Teacher forced to quit.`

This also means that protecting your identity online is your responsibility , share the pictures responsibly with close friends or not at all.

There have been incidents around the world where governments have tried to force shut the voices of opposition and free speech.

Did I not mention Internet censorship ? , well here is a link of blocked sites.  

See for yourself and decide.

[Blocked websites list in China](https://en.wikipedia.org/wiki/Websites_blocked_in_mainland_China)


How to be anonymous ?
==
Its recommended to use a `Virtual Machine` or a `live USB/CD of any linux distro` that are disposable in case someone (NOT YOU) has physical access to the device.

The advantage of using a linux system is that it does not have a lot of 
telemetry services that are tracking your usage continuously.You can always open up task manager in Windows and check for yourself , various telemetry services running.

You can also check how easy it is to track you by visiting following
link:		
[BrowserLeaks.com](https://browserleaks.com/ip)

Use TOR with proxychains
--
 1. **Install tor :**  
 `sudo apt-get install tor`
 2. **Install proxy-chains and configure proxychains:** 
  * Install proxychains :   
  `sudo apt-get install proxychains`
 3. **Configure proxychains:**
      1. Find proxychains config file : `locate proxychains.conf` then `sudo nano /etc/proxychains.conf`
      2. Uncomment the either the `dynamic_chain`  or  `random_chain` 
      3. At the end of the file is a list of proxies , by default `tor` will be listed , you can search online for `SOCKS5 proxies` , it is recommended to use SOCKS5 proxies as they have better performance than SOCKS4 or HTTP/HTTPS proxies , if you can't find any you can still use SOCKS4 proxies.
      4.  **`IMPORTANT`** Before adding proxies to the list , check whether they are running online using proxy checker , just search it.
      5. Once you have added proxies to the list ,save it and exit the editor.
 4. **Using proxychains**:  
 		   1. To use proxychains with browser , just type `proxychains firefox`  
    	 2.   **`IMPORTANT`** **Make sure you close all the browser windows absolutely before executing above command**. You can also check your IP before and after connecting to prexychains which should be different.  
    	[BrowserLeaks.com](https://browserleaks.com/ip)  

Use OpenVPN (free)
--
1. **Install openvpn :**  
`sudo apt-get install openvpn`
2. Visit [vpnbook.com](https://www.vpnbook.com/howto/setup-openvpn-on-ubuntu) and follow the tutorial steps.
3. **To connect to internet using openvpn:**  
`openvpn --config <enter the config filename ending with .ovpn>`
4. type in the username and password  and you are good to go...
5. Checkout [vpnbook.com](https://www.vpnbook.com/howto/setup-openvpn-on-ubuntu) from time to time in any updates of password and username, as this is done for avoiding misuse by the maintainers.

Anonsurf
--
With Anonsurf you can avoid much of the hassle of setting up proxychains , anonsurf can be described as tor wrapped with a gift wrapper that looks good and simple.This is a system wide anonymization.

**Installation process**  

1. Clone the repo  
`git clone https://github.com/Und3rf10w/kali-anonsurf.git`  
2. Set appropriate permissions  
`cd kali-anonsurf`  
`chmod +x ./installer.sh`  
3. Run the installer  
`sudo ./installer.sh`
4. After installation is complete  
`anonsurf help`  
`anonsurf start` - to start anonsurf , anonymize system wide data usage


Final thoughts
==
There are many ways to be anonymous online out of which few are listed here , but even when anonymous one needs to be vigilant on the internet , because there are more ways to compromise your security and identity. Stay anonymous, stay vigilant, be responsible.  
Your security is your own responsibility.

---
Author : Chinmay Moghe
This file is free for distribution , modification and personal use.
