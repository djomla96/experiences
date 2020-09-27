# Everything in quotes
 ```js
 .replace(/height="(.+?")/g, '');
 ```


# Thousand separator
```js
.replace(/\B(?=(\d{3})+(?!\d))/g, ".");
```
