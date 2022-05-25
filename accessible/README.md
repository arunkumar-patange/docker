```
        ._
                |
                |
                |L___,
              .' '.  T
             :  *  :_|
              '._.'   L
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


