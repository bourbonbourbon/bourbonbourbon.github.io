---
title: "Bookmarklets"
date: 2022-10-27T21:20:44+05:30
draft: false
tags: ['browsers', 'javascript', ]
---

## What are bookmarklets?

They are small snippets of JavaScript code that are in the form of a bookmark.
Since it is basically a JavaScript program, it is natively available in all major browsers, including Mozilla Firefox & Chromium-based browsers.  
  
We'll look at how to create bookmarklets in Firefox.


## How to Create Bookmarklets

In Mozilla Firefox, open your bookmarks toolbar by pressing __CTRL + B__, you can then right-click

![](/assets/img/bookmarkmenu.png)

 and click on "Add Bookmark..."

![](/assets/img/bookmarkdialog.png)

We can write a JS script in the URL section of the prompted dialog box.

```js
javascript: (() => {
    alert('Hello, World!');
})();
```

Give a name to the bookmarklet and click on Save.  
What this bookmarklet is going to do it open a alert window in the browser with the message "Hello World".  

Similarly, we can make another bookmarklet that would replace the domain in the URL with whatever we want.

```js
javascript: window.open(
    location.href.replace(/:\/\/([\w-]+.)?(reddit\.com)\//i, "://l.opnxng.com/"), 
    "_self"
    )
```

This will replace the host name "reddit.com" with an alternative front-end "l.opnxng.com"

There are many other bookmarklets that do a variety of things: 
- [agentcooper's youtube playlist sort](https://agentcooper.github.io/youtube-sort/) - which will sort a given youtube playlist by the number of views of the videos in it. 
- [Twitter keyword + Date search](https://github.com/B0sintBlanc/Osint-Bookmarklets/blob/main/Twitter/Twitter%20keyword%20%2B%20Date%20search#L9) - using this we can search for a keyword on Twitter within the given time period.
