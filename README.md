googlecubeembed
==================

Have an online cubing tutorial page? Need an interactive, easy, 3D cube visualizer? Embed this Javascript Rubik's Cube in HTML5! All you need to do is to follow the steps below.

Using Google Chrome Cube Lab Code.

How to Use
==================

1. Include jQuery 1.11.1 (```<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>```) if you have not already done so.
2. Put ```<script src="http://molarmanful.github.io/googlecubeembed/googlecubeembed.js"></script>``` in the head tag, AFTER your jQuery script tag.
3. Put ```<g-cube></g-cube>``` in the body tag, where you want the cube. See jQuery attributes below to customize the cube.
4. Sit back and cube on!

<cube> Attributes
==================
Example code:
```javascript
$('g-cube').gce({
	speed: 1000,
	scramble: "R U R' U' L",
	initcontrols: true,
	algorithm: "R U R' U' "
}, callback());
```
| Attribute | Description |
|-----------|-------------|
| _speed_ | Number. Milliseconds needed to perform a turn. Defaults to 1000. |
| _initcontrols_ | Boolean. Whether to include "Play algorithm" button. Must be set to true to use _algorithm_ attribute. |
| _scramble_ | String. Use Singmaster notation, and put spaces between moves. Brackets, curly brackets, and parentheses are allowed. Rotations must be uppercase. |
| _algorithm_ | String. Use Singmaster notation, and put spaces between moves. Brackets, curly brackets, and parentheses are allowed. Rotations must be uppercase. |
| _callback_ | String. Use Singmaster notation, and put spaces between moves. Brackets, curly brackets, and parentheses are allowed. |

CSS Defaults
==================
```Height``` and ```width``` attributes are both ```100%```. You can change this if you want but use ```!important```.

```position``` is set to ```absolute```. Do not change this; instead, make a parent element if you really need to.

```display``` is set to ```block```. Do not change this.

You may want to set ```top```, ```left```, ```right```, ```bottom``` CSS attributes.
