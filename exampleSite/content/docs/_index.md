---
title: 'Overview'
date: 2018-11-28T15:14:39+10:00
weight: 1
---

## Make Beautiful Docs

Whisper is a minimal documentation theme for Hugo. The design and functionality is intentionally minimal. We’re aiming for a similar feel to a Github readme.

```javascript
var body = document.querySelector('body');
var menuTrigger = document.querySelector('#toggle-main-menu-mobile');
var menuContainer = document.querySelector('#main-menu-mobile');

menuTrigger.onclick = function() {
  menuContainer.classList.toggle('open');
  menuTrigger.classList.toggle('is-active');
  body.classList.toggle('lock-scroll');
};
```
