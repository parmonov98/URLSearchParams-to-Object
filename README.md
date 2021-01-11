# URLSearchParams-to-Object
URLSearchParams to object converter function is very handy in front-end. 
it can handle multilevel query params like param1[element][1]=value1&param1[element][2]=value2

```
var getParamsAsObject = function (url) {
        var res = {};
        
        for (let searchParam of url.searchParams.entries()) {
          res[i[0]] = i[1];
        }
        
        return res;

    };
```

```js

   var url = new URL(window.location.href);
                
   var obj = getParamsAsObject(url);
```
