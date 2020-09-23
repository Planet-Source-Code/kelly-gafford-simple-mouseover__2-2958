<div align="center">

## Simple MouseOver


</div>

### Description

I was tired of reading incomprehensible scripts that used arrays to store the image names or people trying to get fancy. This script does simply what it says, a simple mouseover. Moving the mouse over, off of or clicking on the image changes it.
 
### More Info
 
No changes to the script are needed. The only thing you will need to change is the <a onmouse?=”(MseOvr(‘image_name’)> and the <img name=”image_name”> in the snippet.

A basic understanding of html tag attributes and how to set them up.

A new image is returned to the web page


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Kelly Gafford](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/kelly-gafford.md)
**Level**          |Beginner
**User Rating**    |3.7 (11 globes from 3 users)
**Compatibility**  |
**Category**       |[Internet/ Browsers/ HTML](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/internet-browsers-html__2-68.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/kelly-gafford-simple-mouseover__2-2958/archive/master.zip)





### Source Code

```
<script language="JavaScript1.2">
	function MseOvr(btnName) {
		// the btnName variable is received from the call in the <a href> tag.
		// the following line changes the image from the buttonnorm.gif to the buttonovr.gif.
		document.images[btnName].src = 'images/buttonovr.gif'
	}
	function MseDwn(btnName) {
		// the btnName variable is received from the call in the <a href> tag.
		// the following line changes the image from the buttonovr.gif to the buttondwn.gif.
		document.images[btnName].src='images/buttondwn.gif'
	}
	function MseOut(btnName) {
		// the btnName variable is received from the call in the <a href> tag.
		// the following line changes the image from the buttonovr.gif to the buttonnorm.gif.
		document.images[btnName].src='images/buttonnorm.gif'
	}
</script>
<body>
<!-- In the on mouseover attribute of this tag, I send the name of the image to the various functions. -->
<a href="#" onmouseover="MseOvr('button1')" onmousedown="MseDwn('button1')" onmouseout="MseOut('button1')">
<!-- To adjust this script to your page, change the name of the image "button1" in this case to something that
reflects your image to make it easier to understand. You'll also need to make sure the name of your image is in the
MseOvr(image_name) function call. -->
<img src="images/buttonnorm.gif" class="clsImage1" name="button1" border="0"></a>
</body>
```

