# Capitalize prototype:
```js
String.prototype.capitalize = function () { 
    let stringArray = this.split(" ");
    
    for (let i = 0; i < stringArray.length; i++) {
        stringArray[i] = stringArray[i].charAt(0).toUpperCase() + stringArray[i].slice(1);
    }

    return stringArray.join(" ");
}
```

