modulas
=======

<p>Modulas example with table row color</p>


```javascript

var colors = ['#999999','#000000','#cccccc'],
    myTrs = document.getElementsByTagName('tr');
	
for(i=0, len = myTrs.length; i < len; i++){
  myTrs[i].style.backgroundColor = colors[i % colors.length]
}
```

<p>Hack to mimic console within JSFiddle</p>

```javascript
var consoleLine = "<div class=\"console-line\"></div>";
console = {
    log: function (text) {
        $("#console-log").append($(consoleLine).html(text));
    }
};
```
