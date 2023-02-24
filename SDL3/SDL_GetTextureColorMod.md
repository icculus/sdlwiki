====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetTextureColorMod =

Get the additional color value multiplied into render copy operations.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_GetTextureColorMod(SDL_Texture *texture, Uint8 *r, Uint8 *g, Uint8 *b);
</syntaxhighlight>

== Function Parameters ==

{|
|'''texture'''
|the texture to query
|-
|'''r'''
|a pointer filled in with the current red color value
|-
|'''g'''
|a pointer filled in with the current green color value
|-
|'''b'''
|a pointer filled in with the current blue color value
|}

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetTextureAlphaMod]]
:[[SDL_SetTextureColorMod]]

----
[[CategoryAPI]], [[CategoryRender]]

