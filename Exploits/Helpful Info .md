# ByePassHub > Exploits > Helpful Info | Updated 4/5
**This is basic information that you need to know in order to perform some exploits included in this directory.**
## Table of Contents:
  * [**Finding the Extension ID**](#extension-id)
  * [**Finding your Chrome Version**](#chrome-version)
  * [**Getting your board name and model**](#board-name-and-model)
  * [**Exploit Collections/Guides**](#exploit-collections)
---
### Extension ID
To get extension ids, do the following:
1. Go to chrome://extensions/
2. Find the extension you want to use for the exploit you're going to do. 
3. Click on the details button.
4. Copy the part in the URL after ?id=
  > Example: `haldlgldplgnggkjaafhelgiaglafanh`

### Chrome Version
Go to `chrome://settings/help` to see your chrome version. Use this to find an exploit, since exploits get patched as chrome updates. 

### Board name and model
**Method A:**
1. Go to chrome://version/
2. Check the "Platform" section and look at the end. This is your board name.
> For example, it could be octopus or dedede.
3. Check the "Customization ID" section. This is your board model.
> For example, it could be phaser360 or boten.

**Method B:**
1. Go to `chrome://system/`
  > If that's blocked, do CTRL + SEARCH + I, enter anything in the description, click "Continue" then click the blue "System" and app info text.
2. Wait until it finishes loading.

To find your board name, check one of these sections: <br>
- CHROMEOS_RELEASE_BOARD (board name at start) <br>
- CHROMEOS_RELEASE_BUILDER_PATH (board name at start) <br>
- CHROMEOS_RELEASE_DESCRIPTION (board name at end) <br>
- platform_identity_name <br>

To find your board model, check one of these sections: <br>
- HWID (board model at start) <br>
- hardware_class (board model at start) <br>
- platform_identity_model <br>

### Exploit Collections
**These are other exploit collections that are actively updated, and probably better than mine lol. Use a proxy (mainUnblockers.md) if the sites are blocked. <br>
Titanium Network: https://docs.titaniumnetwork.org/guides/ (they also have a really good discord server!)<br>
Chromebook utilities: https://github.com/S-PScripts/chromebook-utilities/blob/main/Exploits/README.md <br>
Updated Chromebook utilities: https://github.com/Burvyn/Corellium/tree/main <br>
Chrose: https://chrose.netlify.app/ <br>
Mercury Workshop: https://mercurywork.shop/ <br>
Ext remover: https://github.com/3kh0/ext-remover <br>
Unenrolling guide: https://chromebook-guide.github.io/ <br>
