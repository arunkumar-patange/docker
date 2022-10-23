```
    ⠊ ⠺⠊⠇⠇ ⠎⠑⠑
```

## Install Plugin
* https://chrome.google.com/webstore/detail/run-javascript/lmilalhkkdhfieeienjbiicclobibjao

## Copy Script 
```
function nativeTreeWalker() {
    var walker = document.createTreeWalker(
        document.body, 
        NodeFilter.SHOW_TEXT, 
        null, 
        false
    );

    var node;
    var textNodes = [];

    while(node = walker.nextNode()) {
        textNodes.push(node);
    }
    return textNodes;}
    dd=nativeTreeWalker();
    dd.forEach(e => e.parentNode && e.parentNode.setAttribute("tabIndex", 0));
```

https://gist.github.com/gregsadetsky/d20b325a1848dd6009503b08f711c266
```
javascript:(function() {var s=document.createElement('script');s.src='https://cdn.jsdelivr.net/gh/ranbuch/accessibility@master/dist/main.bundle.js';document.body.append(s);s.onload=function() {new Accessibility()}})()
```

## Demo
https://drive.google.com/file/d/1FODCcv6sI4OxRMiWwMiiLO2-pUrIFHVQ/view?usp=sharing

