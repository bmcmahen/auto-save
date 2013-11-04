
# auto-save

  A simple timer wrapper that is useful for implementing a delayed autosave in text-based applications, like Google Docs. 

## Installation

  Install with [component(1)](http://component.io):

    $ component install bmcmahen/auto-save

## API

```javascript
// 500 represents the timeout duration in ms.
var autosave = require('auto-save')(500);
var txt = document.getElementByTagName('textarea')[0];
txt.oninput = function(){
  interval(function(){
    console.log('do some saving.');
  });
};
```

## License

  MIT
