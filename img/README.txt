SVG hack to get fonts working
=============================

`xyz-src.svg` is the Inkscape master file. Open with Inkscape, edit and save it as "Inkscape SVG". When it's ready, also save a copy as "Plain SVG", without the `-src` bit (`xyz.svg`). Open the plain SVG in text mode (in emacs, hit C-c C-c to switch from image viewing mode) and add the following tag after the metadata one:

```
  <style type="text/css"><![CDATA[
  @import url(../lib/font/source-sans-pro/source-sans-pro.css);
  ]]></style>
```

This latter file is the one that gets included in the slides.
