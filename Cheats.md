## ByepassHub > Cheats | updated Jul 11
## If you like this, make sure to star it!
**Other Files**: <br>
**Unblocker(Proxies) links**: Go [here](https://github.com/wea-f/ByePassHub/blob/main/mainUnblockers.md) or go to the mainUnblockers.md file <br> 
**Exploits, Bypasses, Bookmarklets:** Go [here](https://github.com/wea-f/ByePassHub/blob/main/Exploits/README.md) <br>
**Main Games:** Go [here](https://github.com/wea-f/ByePassHub/blob/main/Games.md) or go to the Games.md file <br>
**Back to Main Hub:** Go [here](https://github.com/wea-f/ByePassHub/blob/main/README.md) or go to the main README.md file <br>

---

This is a collection of cheats for learning game platforms like Kahoot or Blooket. <br>
Also, I did not make these cheats, I found them through searching the web and repositories. <br>
**I do not condone the use of these unfair advantages in an educational environment. This can ruin the experience for others and it is best to play with integrity when learning.**

---

Try putting these links in a proxy if they are blocked. It probably won't work, but it's worth a try.
## **RECOMMENDED**: Cheat Hubs
The ultimate hub for every learning game platform, used for Kahoot, Gimkit, Blooket, Brainly (bypass exercise limit), and more! <br>
https://schoolcheats.net/dashboard <br>
https://cheatnetwork.eu/ <br>
https://quizit.online/ <br>

## Kahoot Cheats
https://kahoot.club/ <br>
https://mem.rip/kahoot/ <br>

## Blooket Cheats (You can use an unblocker and it still works) | You need to be able to execute bookmarklets
https://05konz.github.io/Blooket-Cheats/ <br>
https://github.com/05Konz/Blooket-Cheats <br>

## Quizlet Cheats
These are found from this repository: https://github.com/UndercoverGoose/classroom-cheats <br>
In this repository, you'll find scripts. You can execute this via bookmarklets or console. <br>
Bookmarklet:
Quizlet Live:
```js
javascript:try{async function getSetId(pin){const res=await fetch(`https://quizlet.com/webapi/3.8/multiplayer/game-instance?gameCode=${pin}`);const json=await res.json();if(json.error)throw new Error(json.error.message);return json.gameInstance.itemId;}async function getSetData(setId){const res=await fetch(`https://quizlet.com/${setId}`);const text=await res.text();const data=text.match(/\\"termIdToTermsMap\\":{.+?{.+?\\"termSort\\":/gi)?.[0];if(!data)throw new Error("Failed to parse set data.");const parsed=JSON.parse(data.slice(21,-14).replaceAll(`\\"`,`"`));return[Object.fromEntries(Object.values(parsed).map(({word, definition})=>[word, definition])),Object.fromEntries(Object.values(parsed).map(({word, definition})=>[definition, word]))];}function getActiveQuestion(){try{const question=document.querySelector(".StudentPrompt-text").textContent;const answers=Array.from(document.querySelectorAll(".StudentAnswerOption-text"));return[question, answers];}catch{}return[null,null];}(async()=>{const pin=prompt("Enter PIN, like: XXX-XXX","").match(/[0-9a-zA-Z]/g).join("");if(pin.length!==6)throw new Error("Pin must be 6 characters in length.");const setId=await getSetId(pin);const[term2Def, def2Term]=await getSetData(setId);setInterval(async function(){const[question,choices]=getActiveQuestion();if(!question||!choices)return;if(question in term2Def){choices.forEach((choice)=>{if(choice.textContent===term2Def[question])choice.style.fontWeight="bolder";});}else if(question in def2Term){choices.forEach((choice)=>{if(choice.textContent===def2Term[question])choice.style.fontWeight="bolder";});}else{choices.forEach((choice)=>{choice.style.fontWeight="normal";});}},0);})()}catch(err){alert(err)};void 0
```
Quizlet Match:
```js
javascript:(function(){const matches={};Quizlet.matchModeData.terms.forEach((term)=>{matches[term.word]=term.definition});let css='FormattedText notranslate TermText MatchModeQuestionGridTile-text';if(document.getElementsByClassName(css).length===0){css='MatchModeQuestionScatterTile'}const tiles=Array.from(document.getElementsByClassName(css));const colors=['#f93640','#f98836','#f9e936','#3df936','#36f9d9','#3650f9','#7e36f9','#dc36f9','#ffffff','#a3a3a3','#424242'];Array.from(document.getElementsByClassName('MatchModeQuestionGridTile-image')).forEach((image)=>{image.style.display='none'});let colorIndex=0;for(const term in matches){const definition=matches[term];tiles.forEach((tile)=>{if(tile.textContent===term){tiles.forEach((box)=>{if(box.textContent===definition){box.style.background=colors[colorIndex];box.style.color='black'}});tile.style.background=colors[colorIndex];tile.style.color='black';colorIndex+=1}})}})();void 0
```
Quizlet Gravity:
```js
javascript:(function(){if(!window.gooseGravity){window.gooseGravity=true;const matches={};Quizlet.gravityModeData.terms.forEach((term)=>{matches[term.word]=term.definition});const reversed={};for(const term in matches){reversed[matches[term]]=term}setInterval(function(){const asteroids=Array.from(document.querySelectorAll('.TermText'));if(asteroids.length===0){return}asteroids.forEach((asteroid)=>{const term=asteroid.textContent;if(asteroid.gooseAnswered){return}if(term in matches){asteroid.textContent=matches[term];asteroid.gooseAnswered=true}else if(term in reversed){asteroid.textContent=reversed[term];asteroid.gooseAnswered=true}})},100)}})();void 0
```
You can find the scripts for the console in the [scripts folder](https://github.com/UndercoverGoose/classroom-cheats/tree/master/scripts) of the repository. 

## Gimkit Cheats
Repository: https://github.com/bob486/quizlet/blob/master/gimkit/README.md <br>
Usage: https://github.com/bob486/quizlet/blob/master/gimkit/README.md#usage <br>
Bookmarklet:
```js
javascript:(function(){let l=document.createElement("script");l.src="https://undercovermoose.github.io/gimkitjs/gimkit.js";document.body.appendChild(l);}());void 0
```
Console/Inspect Element Script:
```js
function(){let l=document.createElement("script");l.src="https://undercovergoose.github.io/quizlet/gimkit/gimkit.js";document.body.appendChild(l);}();
```

## Quizizz Cheats
These are from this [repository](https://github.com/bob486/quizlet/blob/master/quizizz/README.md)
1. Join quizizz and go through questions, when finished, press "Study Flashcards" and **run the script.**
2. Then join the quizizz again, or start another attempt. **Run script** and you are done! <br>
Bookmarklet Script:
```js
javascript:(function(){let l=document.createElement("script");l.src="https://undercovergoose.github.io/quizlet/quizizz/script.js";document.body.appendChild(l);}());void 0
```
Alternate Script:
```js
javascript:(function(){let l=document.createElement("script");l.src="https://undercovermoose.github.io/quizizzjs/script.js";document.body.appendChild(l);}());void 0
```
You can run the above scripts in the console or in the inspect element, just remove the `javascript:` part and the `void 0` part at the end.
