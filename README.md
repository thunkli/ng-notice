# ng-notice
![notice](https://user-images.githubusercontent.com/1193966/30494813-26a55408-9a7c-11e7-875b-ef8c59cd7302.png)

## Installation
### HTML:

## Usage
```js
import Notice from 'ng-notice/src/index.ts';
import 'ng-notice/src/style.css';
```

```js
//alert
Notice.alert({text:"Welcome!"});
Notice.alert({text:"Welcome!",time:10});
//force
Notice.force({text:"Welcome!"});
Notice.force({
    text: "Welcome!",
    callback() {
        console.log("callback")
    }
});
//confirm
Notice.confirm({
    text: "Welcome!",
    submitCallback() {
        console.log("submit")
    },
    cancelCallback() {
        console.log("cancel")
    }
});
```
## Browser Support
* IE 9+
* Chrome 11+
* Firefox 4+
* Safari 5.1+
* Opera 11.5+
