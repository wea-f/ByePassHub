  * **Wifi Password Finders (includes getting the school's wifi password)**
     - [Wifi Password | **Recommended**](#wifi-password)
     - [Wifi Password #2](#wifi-password-2)
---

## Wifi Password
**I am not reponsible for any illegal actions or trouble you get into doing this, stay cautious**
This may or may not work, depending if wifi is managed, if it doesn't work, do CAUB (above) first then try. 
1. Go to `https://cdn.3kh0.net/sipe`, use proxy if blocked.
2. Put the wifi name in the input box.
3. If you don't know the name, you can leave it blank, you'll have to guess it on step 10
4. Click the magic button. Remember what it tells you.
5. Go to `chrome://sync-internals/` in a new tab.
6. Click on `Trigger GetUpdates`
7. Click the Search tab.
8. Put in `wifi_` in the text box.
9. Click the search button.
10. Click the name of the wifi you got from step 3, guess the name of the wifi if you left it blank. Note: may be a longer string than what it says.
11. Copy all of the data.
12. Go back to the website.
13. Put the data in the text box.
14. Click the magic button.
12. It will say that the data is successfully found. It will tell you the wifi name and password.

## Wifi Password #2
1. Go to `chrome://net-export`
2. In options, set the option to `Include raw bytes`
3. Click `Start logging to Disk` and save the file.
4. Go to `chrome://policy` in a new tab.
5. Click Reload policies.
6. Go back to the net-export tab.
7. Stop logging.
8. Go to `https://luphoria.com/netlog-policy-password-tool`, use proxy if blocked.
9. Click Choose File.
10. Choose the file you saved in Step 3.
11. The credentials column is the wifi password!

## #3 - NEW Pull req #105 - Slideshow
It's a tutorial to open **another wifi** then the one imposed onto you by your chromebook manager with policies.
Preferably, you should open a wifi without DNS blocking, such as the guest wifi, like me.
Unfortunately, you need to know the password to the wifi you want to connect to, or hope the guest wifi password is free.
[Chromebook Wifi Unlock](https://docs.google.com/presentation/d/1v1bpEnvQ0OiZ-0-7t_n4VszUAArajypVp1A4A0JmYYI/edit?usp=sharing)
This exploit was performed on ChromeOS v138.

<br> **Back to [README file](https://github.com/wea-f/ByePassHub/blob/main/Exploits/README.md)** (The starting file)
