love2d_gametemplate
===================

This is a gametemplate for LÖVE engine using middleclass, stateful, love-loader, TESound and cron libraries.

The base of this template is copied from kikito.

Features
==========
- The aim of this template is to seperate ressource loading from scenes.
- A ressource reference is submitted to a Loading State and the ressources are loaded via 'love-loader' library.
- Loading of ressources is visualised via 'love-loader' library.
- After all Ressources are loaded, the Loading State switches to a Next-State.
- All ressources are accessed via the global variable 'media'.
- All ressources share the same naming ... so you can overwrite existing ones using the same name.
- You can add additional ressources during any state switch.
- 'TESound' library is enhanced to also play sounddata.
- Images can be used raw or as Texture-Atlas without changing the drawing code
- Tweening library 'flux' is included.

Sample
==========
```
media.quads['left-hand-climber-hi']:draw(0,0) -- single file image (no Quad)
media.quads['left-hand-climber-hi3']:draw(love.mouse.getX(), love.mouse.getY()) --from texture atlas (image with Quads)
```

Script for TexturePacker (http://www.codeandweb.com/texturepacker) included!
or use https://github.com/Bradshaw/Fudge

more Infos here: http://love2d.org/forums/viewtopic.php?f=5&t=77918

License
==========
This gametemplate is distributed under the zlib/libpng License (http://opensource.org/licenses/Zlib)

All libraries used by this game_template are licensed under thier own licenses! 
