modulas
=======

#### 1. Modulas example with table row color

```javascript

var colors = ['#999999','#000000','#cccccc'],
    myTrs = document.getElementsByTagName('tr');
	
for(i=0, len = myTrs.length; i < len; i++){
  myTrs[i].style.backgroundColor = colors[i % colors.length]
}
```

#### 2. Hack to mimic console within JSFiddle

```javascript
var consoleLine = "<div class=\"console-line\"></div>";
console = {
    log: function (text) {
        $("#console-log").append($(consoleLine).html(text));
    }
};
```

#### 3. Write a function translate() that will translate a text into "rövarspråket". That is, double every consonant and place an occurrence of "o" in between. For example, translate("this is fun") should return the string "tothohisos isos fofunon".

```javascript
function isVowel(param,o){
	var char = param.split("");
	for(var i = 0; i<char.length; i++){
	var newChar, charArr = char[i];

		if( !(/[aeiou]/i.test(charArr)) ) {
			if(!(/\s/.test(charArr))){
				 newChar = charArr + o + charArr;
			} else {
				 newChar = charArr;
			}
		} else{ newChar = charArr;}
		
		// Joining all splited text with code.
		document.getElementById("text").innerHTML += newChar;
		
	};
};

isVowel("This is fun",'o')
```
