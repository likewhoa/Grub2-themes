## Installation

**Using git:**
<code>$ git clone git://github.com/likewhoa/Grub2-themes.git
 \# cp -r Grub2-themes/GenGrub /boot/grub/themes/</code>

**Edit your /etc/default/grub and change line:**
<code>\#GRUB_THEME="/path/to/gfxtheme"
to
GRUB_THEME="/boot/grub/themes/GenGrub/theme.txt"
</code>

**The resolution the theme was designed to show best at 1024x768:**
<code>GRUB_GFXMODE=auto
to
GRUB_GFXMODE=1024x768</code>

**Update grub configuration:**
<code>\# grub-mkconfig -o /boot/grub/grub.cfg</code>

**Screenshots**
<a href="https://github.com/likewhoa/Grub2-themes/blob/master/Preview/GenGrub_preview.png"><img height=300 src="https://github.com/likewhoa/Grub2-themes/blob/master/Preview/GenGrub_preview.png?raw=true"></a> <a href="https://github.com/likewhoa/Grub2-themes/blob/master/Preview/GenGrub_preview.png"><img height=300 src="https://github.com/likewhoa/Grub2-themes/blob/master/Preview/GenGrub_preview.png?raw=true"></a>

## FAQ

**Can I change the background or color of the theme?**
Yes, choose an image, convert and resize to 1024x768 in PNG
Copy the image to */boot/grub/themes/THEME/*
Edit */boot/grub/themes/THEME/theme.txt*:
<code>desktop-image: "background.png" # Theme background image
desktop-color: "#000000" # Theme color</code>


**How can I change the logo theme?**
Copy your logo image to */boot/grub/themes/THEME/* (must be in PNG)
Edit */boot/grub/themes/THEME/theme.txt*:
<code>\+ image {
id = "\__archlogo__"
left = 30%
width = 10%
top = 2%
height = 12%
file = "archlogo.png" \# distribution logo</code>

**Why the menus are so slow?**
Grub2 has some keyboard lag using themes, as referred on "[The Definitive Guide To Theming GRUB 2 v1.99](https://docs.google.com/open?id=0B82343FTJphIbElHUGVac1hBZnc)" pag 73

## References:
[GNU GRUB Manual 1.99](http://www.gnu.org/software/grub/manual/grub.html#Theme-file-format)
[GRUB Graphical Menus Project](http://grub.gibibit.com/Theme_format)
[The Definitive Guide To Theming GRUB 2 v1.99](https://docs.google.com/open?id=0B82343FTJphIbElHUGVac1hBZnc)


## Ideas or suggestions to share in:
[github issues](https://github.com/likewhoa/Grub2-themes/issues)

