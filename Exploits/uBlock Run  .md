  * **uBlock extension Run bypasses - allows you to run bookmarklets:**
     - [uBlock Run | Able to run bookmarklets if blocked](#ublock-run--able-to-run-bookmarklets-if-blocked)
     - [uBlock Run 2 | Able to run bookmarklets if blocked](#ublock-run-2--able-to-run-bookmarklets-if-blocked)
  ---

  These do not work as of Oct 24, since uBlock Origin does not work on Chrome. According to [https://github.com/3kh0/ext-remover?tab=readme-ov-file#ublock-run-run-code-on-pages](https://github.com/3kh0/ext-remover?tab=readme-ov-file#ublock-run-run-code-on-pages)
  ### uBlock Run | Able to run bookmarklets if blocked
1. You must have the uBlock Origin extension installed for this to work.
2. Go to the extension's settings (press the puzzle icon next to the url, press the 3 dots corresponding to the extension, and press "Manage Extension")
3. Under the settings tab, check the "I am an advanced user" box, then click on the small cog icon.
4. Find "userResourcesLocation" and change it from `unset` to
```js
https://raw.githubusercontent.com/3kh0/ext-remover/main/ublockExec.js
```
5.Go to the My filters tab of the settings and add the following line:
```js
*##+js(execute_script.js)
```
6. Now press ctr+alt+tilde (~) to run code on the current page, and you are done!

### uBlock Run 2 | Able to run bookmarklets if blocked
1. Open uBlock settings
2. Enable advanced settings, and click the gear ⚙️ button
Caution! DON'T MODIFY ANYTHING ELSE ON THIS PAGE, if you mess up, go to the home of settings and at the bottom click reset to default settings.
3. Add the script
Change `userResourcesLocation unset` (ctrl f it if needed)
to
```js
userResourcesLocation https://inglan2.github.io/uRun/urun.js
```
4. After closing the advanced settings tab, go to the filters tab and add this:
```js
*##+js(urun.js)
```
How to use: <br>
Simply press Ctrl + Shift + ` to open the menu and from there you can run and create scripts. To add a script, press the "+" button up the top right, and enter the code you would like to add (without the javascript: part).

<br> **Back to [README file](https://github.com/wea-f/ByePassHub/blob/main/Exploits/README.md)** (The starting file)
