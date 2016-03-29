#Simple Async Loop

```
npm install asyncinloop
```

```
var asyncLoop = require('asyncinloop)
asyncLoop({
    length : 5,
    functionToLoop : function(loop, i){
        setTimeout(function(){
            document.write('Iteration ' + i + ' <br>');
            loop();
        },1000);
    },
    callback : function(){
        document.write('All done!');
    }    
});
```
http://jsfiddle.net/NXTv7/8/
