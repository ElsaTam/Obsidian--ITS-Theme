# Image Positions
> Move/position and re-size the images in notes

**⚠ Note:** 
- Obsidian internal images `![[` will change immediately, but for external images `![]()`, the page needs to be reopened to see the changes. 
- Might not be 100% compatible with [Lithou's Image Flags snippet.](https://github.com/Lithou/Sandbox/blob/main/.obsidian/snippets/pub-Image%20Flags.css)
- Image grid doesn't quite work with external images `[]()`as nicely as internally linked ones.

# Syntax
```md
![[Internal Image.png|attribute attribute2]]
![[Internal Image.png|sban cover hs-med]]

![External Image|attribute attribute2](.png)
![External Image|sban cover hs-med](.png)
```

# Attributes

### Clear

Attribute | Description |
---|---|
`clear` | `clear` will allow that image to sit below another image<br>If it's on the same side instead of sitting in the middle of the page.

### Image Grid

Attribute | Description |
---|---|
`grid` | Display image side-by-side in a grid

![](../Images/Image_Adjustments-Image-Grids.png)

### Cover (Mostly for Customizable Version)

Attribute | Description |
---|---|
`cover`| A resized image will maintain aspect ratio and avoid stretching.

### Sizing (Mostly for Customizable Version)

Attribute | Description |
---|---|
`loc\|sban\|200`| Place the `\|<numbers>` sizing at the *end* of the text and it will shrink the image to that size.


## Simplified Version

### Left/Right/Center

Attribute | Description |
---|---|
`left`| `left` will move the image to the left.
`right`| `right` will move the image to the right.
`ctr`| `ctr` will move the image to the center.

![](../Images/Image_Adjustments-Simple-Positions.png)


### Types

![](../Images/Image_Adjustments-Simple-Sizing.png)

#### Banner

Attribute | Description |
---|---|
`banner`| `banner` will crop the image height-wise to 150px while setting the width to cover the entire page.
`banner+small`| `banner+small` will crop the image height-wise to 100px while setting the width to cover the entire page.
`banner+tall`| `banner+tall` will crop the image height-wise to 500px while setting the width to cover the entire page.


#### Portrait

Attribute | Description |
---|---|
`portrait`| `portrait` will crop the image width-wise to 40% while setting the height to a standard of 400px.
`portrait+small`| `portrait+small` will crop the image width-wise to 20% while setting the height to a standard of 200px.
`portrait+tall`| `portrait+tall` will crop the image width-wise to 50% while setting the height to a standard of 500px.


#### Profile

Attribute | Description |
---|---|
`profile`| `profile` will round the borders of the image to create a round image and size it to 100px.
`profile+medium`| `profile+medium` will round the borders of the image to create a round image and resize it to 250px.


## Customizable Version
### Left/Right

Attribute | Description |
---|---|
`locl`| `locl` will move the image to the left.
`locr`| `locr` will move the image to the right.


### Inner Image Position

![](../Images/Image_Adjustments-Custom--Inner-Position-Precise.png)

Attribute | Description |
---|---|
`pl`| Move inside of the image to the left.
`pr`| Move inside of the image to the right.
`pt`| Move inside of the image to the top.
`pb`| Move inside of the image to the bottom.
`pc`| Move inside of the image to the center.


> These will inch the images around if the ^ above syntax isn't enough.

Attribute | Description |
---|---|
`p+cr`| `p+cr` will move the inside of the image to the center right.
`p+cl`| `p+cl` will move the inside of the image to the center left.
||
`p+ct`| `p+ct` will move the inside of the image to the center top of the image.
`p+cct`| `p+cct` will move the inside of the image to the center top, slightly higher than `p+ct`|
`p+tc`| `p+tc` will move the inside of the image to the center top, slightly lower than `pt`|
`p+tcc`| `p+tcc` will move the inside of the image to the center top, slightly lower than `p+tc`|
||
`p+cb`| `p+cb` will move the inside of the image to the center bottom of the image.
`p+ccb`| `p+ccb` will move the inside of the image to the center bottom, slightly lower than `p+cb`|
`p+bc`| `p+bc` will move the inside of the image to the center bottom, slightly higher than `pb`|
`p+bcc`| `p+bcc` will move the inside of the image to the center bottom, slightly higher than `p+bc`|

### Sizing
![](../Images/Image_Adjustments-Custom-Sizing.png)

Attributes | Resize Image to:  |
---|---|
`htiny`| 100px in height.
`hsmall`| 200px in height.
`hs-med`| 300px in height.
`hm-sm`| 400px in height.
`hmed`| 500px in height.
`hm-tl`| 600px in height.
`htall`| 700px in height.
||
`wtiny`| 100px in width.
`wsmall`| 200px in width.
`ws-med`| 300px in width.
`wm-sm`| 400px in width.
`wmed`| 500px in width.
`wm-tl`| 600px in width.
`wtall`| 700px in width.
