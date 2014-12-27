gCube
==================

Have an online cubing tutorial page? Need an interactive, easy, 3D cube visualizer? Use gCube! All you need to do is to follow the steps below.

Using Google Chrome Cube Lab Code.

How to Use
==================

1. Include jQuery 1.11.1 (```<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>```) if you have not already done so.
2. Put ```<script src="http://molarmanful.github.io/gCube/gcube.js"></script>``` in the head tag, AFTER your jQuery script tag.
3. Put ```<g-cube></g-cube>``` in the body tag, where you want the cube. See jQuery attributes below to customize the cube.
4. Sit back and drag!

<cube> Attributes
==================
Example code:
```javascript
$('g-cube').gce({
	speed: 100,
	scramble: "RrLlUuDdFfBbMmEeSsXxYyZz",
	algorithm: "RUruRUruRUru",
	highlight: "flxcross"
}, callback());
```
| Attribute | Description |
|-----------|-------------|
| _speed_ | Number. Milliseconds needed to perform a turn. Defaults to `100`. |
| _scramble_ | String. See _Notation_ for more info. Using `/random` is also allowed, but another of these commands is required: `/2-genR`, `/2-genL`, `/2-genM`, `/3-genRF`, `/3-genLF`, and `/3-genRL`. Defaults to `''`. |
| _algorithm_ | String. If this is set, then mouse controls will be disabled unless `'/mouse'` is added to the end of the algorithm string. See _Notation_ for more info. Defaults to `''`. |
| _highlight_ | String. You can use one or more of these to hide all but some selected stickers: `onlyedges`, `onlycorners`, `onlycenters`, `flcross`, `flxcross`, `fl`, `flcorners`, `f2l`, `f2ll`, `llcross`, `llbar`, `llL`, `lldot`, `llcorners`, `2x2x2`, `2x2x3`, `eoline`, `roux1`, `roux2`, and `cmll`. Case-sensitive. Defaults to highlighting the whole cube. |
| _callback_ | Function to be called after options are initialized. |

CSS Defaults
==================
`Height` and `width` attributes are both `100%`.

`position` is set to `relative`.

`display` is set to `block`.

Notation
===================
Googlecubeembed notation is based on Singmaster notation, but instead of i, `, or ' suffixes to denote counterclockwise turns, lowercase letters are used. Rotations are uppercase unless turning counterclockwise. 180-degree turns are denoted as 2 uppercase/lowercase letters.

Examples:

R = R

Ri/R`/R' = r

R2 = RR/rr
