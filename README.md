# plymouth-theme-arch-logo-symbol

A plymouth theme with the Archlinux logo

This theme is based off a similar theme that uses the debian logo:
https://www.gnome-look.org/p/1888173 which itself seems to be based off of
a theme that uses the ubuntu logo: https://www.gnome-look.org/p/1805336.

## process
The main [arch linux logo](https://archlinux.org/art/) was taken and cropped to
just the symbol then resized to a height of 120px and then the canvas resized
to a width of 133px with the image aligned to the right (to account for the TM
symbol). Then I opened all of the images in the GIMP and pasted the arch logo,
moved it up 45px (to the top of the debian logo) and then to the right 3px.
Then I merged the layers down into a single layer and exported over the
existing image.

After modifying the animation and progress images I ran them through `optipng`:

```shell
find . -type f -name '*.png' -exec optipng {} \;
```

## license

The debian theme claims to be MIT licensed however there is no LICENSE file in
the release notes. Similarly, the ubuntu logo theme from which the debian one
is based claims to be X11 license, but there is no also no LICENSE file.

It's also challenging to find who the actual authors are because the GNOME look
pages just include usernames and links to opencode.net pages. With this
information I have created license files in this repo using those usernames and
the publication dates.

For my own modifications on top I am using the MIT-0 license.
