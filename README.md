modulas
=======

Modulas example with table row color

<pre>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title>Untitled Document</title>
</head>

<body>
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

</body>
<script type="text/javascript">
var colors = ['#999999','#000000','#cccccc'],
	myTrs = document.getElementsByTagName('tr');
	
for(i=0, len = myTrs.length; i < len; i++){
	myTrs[i].style.backgroundColor = colors[i % colors.length]
}
</script>
</html>

</pre>
