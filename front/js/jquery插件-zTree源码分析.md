<h3>deepCopy深拷贝：</h3>
<pre>function deepCopy(obj){
    if (obj === null) return null;
    var o = Object.prototype.toString.apply(obj) === "[object Array]" ? [] : {};
    for (var i in obj) {
        o[i] = (obj[i] instanceof Date) ? new Date(obj[i].getTime()) : (typeof obj[i] === "object" ? clonee(obj[i]) : obj[i]);
    }
    return o;
}</pre>
<h3>jquery继承的方法</h3>
<pre>当多个object要合并时可以使用$.extend去合并得到结果
var result=$.extend({},{name:"Tom",age:21},{name:"Jerry",sex:"Boy"})
result={name:"Jerry",age:21,sex:"Boy"}
该方法将src合并到jquery的实例对象中去，如:
$.fn.extend({
    hello:function(){alert('hello');}
});

多重继承apply和call：
Function.apply(obj, args)方法能接收两个参数，obj：这个对象将代替Function类里this对象；args：这个是数组，它将作为参数传给Function内部的参数
而call和apply的区别只是将后面的args的参数列表展示不一样，call是Function.call(obj, [param1[,param2[,...]]])params是一个参数列表

jquery.clone(boolean):为true时，会拷贝dom内继承的事件，默认的false只会继承dom</pre>