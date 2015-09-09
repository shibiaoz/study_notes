> javascript 设计模式


> 单例模式

保证一个系统中一个类只有一个实例


// 第一种方式
```
function Mask () {
    var mask ;
    var _createMask = function () {
        var html = '<div class="mask-wraper"> <div class="mask-content"></div></div>';
        $(html).append($('body'));
    }
    return function() {
        return mask || (mask = _createMask())
    }();
}
 // test
    var modalMask =  Mask();
    var modalMask2 = Mask();
```
// 第二种方式

```
var Singleton = (function () {
    var instantiated;
    function init() {
        /*这里定义单例代码*/
        return {
            publicMethod: function () {
                console.log('hello world');
            },
            publicProperty: 'test'
        };
    }

    return {
        getInstance: function () {
            if (!instantiated) {
                instantiated = init();
            }
            return instantiated;
        }
    };
})();

/*调用公有的方法来获取实例:*/
Singleton.getInstance().publicMethod();
```

