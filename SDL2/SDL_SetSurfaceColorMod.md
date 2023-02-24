====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_SetSurfaceColorMod =

Set an additional color value multiplied into blit operations.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_SetSurfaceColorMod(SDL_Surface * surface,
                           Uint8 r, Uint8 g, Uint8 b);
</syntaxhighlight>

== Function Parameters ==

{|
|'''surface'''
|the [[SDL_Surface]] structure to update
|-
|'''r'''
|the red color value multiplied into blit operations
|-
|'''g'''
|the green color value multiplied into blit operations
|-
|'''b'''
|the blue color value multiplied into blit operations
|}

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Remarks ==

When this surface is blitted, during the blit operation each source color
channel is modulated by the appropriate color value according to the
following formula:

<code>srcC = srcC * (color / 255)</code>

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GetSurfaceColorMod]]
:[[SDL_SetSurfaceAlphaMod]]

----
[[CategoryAPI]]

