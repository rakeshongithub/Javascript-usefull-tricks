modulas
=======

Modulas example with table row color


<table width="200">
  <tr>
    <td>1</td>
    <td>2</td>
  </tr>
  <tr>
    <td>3</td>
    <td>4</td>
  </tr>
  <tr>
    <td>5</td>
    <td>6</td>
  </tr>
  <tr>
    <td>7</td>
    <td>8</td>
  </tr>
</table>

<pre>
var colors = ['#999999','#000000','#cccccc'],
	myTrs = document.getElementsByTagName('tr');
	
for(i=0, len = myTrs.length; i < len; i++){
	myTrs[i].style.backgroundColor = colors[i % colors.length]
}
</pre>
