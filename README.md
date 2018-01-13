# Frame
Frame embeds sites in a full-page iframe, so you can go to a site, and it wont be logged in your history! Only Frame will be logged in the history. It defaults to Bing, so you can search for any site.

### Why is this useful?
Even if your administrators have disabled Private/Incognito mode and deleting your browser history, Frame will let you visit sites undetected.

### halp some sites are just showing a white screen whyyyyyyy
If sites have their X-Frame-Origins setting set to `deny` or `sameorigin`, it will not load. This is something set by the site owners. You can check in your browser's console:
![](https://i.dis.gg/nav8c7f.png)

### Why default to Bing and not Google?
Google has their X-Frame-Origins set to `sameorigin`.

### How can I change the URL and/or page title?
First, you must fork this repo.
You can change the page title in line 5 of index.html:
```html
  <title>Frame</title>
```
You can set the URL in the repo settings. Note that if you are using a custom domain, you must make a CNAME and point it to yourusername.github.io.
