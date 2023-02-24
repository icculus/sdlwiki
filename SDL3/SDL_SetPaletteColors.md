====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_SetPaletteColors =

Set a range of colors in a palette.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_SetPaletteColors(SDL_Palette * palette,
                         const SDL_Color * colors,
                         int firstcolor, int ncolors);
</syntaxhighlight>

== Function Parameters ==

{|
|'''palette'''
|the [[SDL_Palette]] structure to modify
|-
|'''colors'''
|an array of [[SDL_Color]] structures to copy into the palette
|-
|'''firstcolor'''
|the index of the first palette entry to modify
|-
|'''ncolors'''
|the number of entries to modify
|}

== Return Value ==

Returns 0 on success or a negative error code if not all of the colors
could be set; call [[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_CreatePalette]]
:[[SDL_CreateSurface]]

----
[[CategoryAPI]], [[CategoryPixels]]

