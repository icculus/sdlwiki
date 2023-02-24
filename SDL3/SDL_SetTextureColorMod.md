====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_SetTextureColorMod =

Set an additional color value multiplied into render copy operations.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_SetTextureColorMod(SDL_Texture *texture, Uint8 r, Uint8 g, Uint8 b);
</syntaxhighlight>

== Function Parameters ==

{|
|'''texture'''
|the texture to update
|-
|'''r'''
|the red color value multiplied into copy operations
|-
|'''g'''
|the green color value multiplied into copy operations
|-
|'''b'''
|the blue color value multiplied into copy operations
|}

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Remarks ==

When this texture is rendered, during the copy operation each source color
channel is modulated by the appropriate color value according to the
following formula:

<code>srcC = srcC * (color / 255)</code>

Color modulation is not always supported by the renderer; it will return -1
if color modulation is not supported.

== Version ==

This function is available since SDL 3.0.0.

== Code Examples ==

<syntaxhighlight lang='c++'>
...
SDL_Texture* pTexture = SDL_CreateTextureFromSurface( renderer, loadedSurface );
SDL_SetTextureColorMod( pTexture, 64, 64, 64 );
...
</syntaxhighlight>

== Related Functions ==

:[[SDL_GetTextureColorMod]]
:[[SDL_SetTextureAlphaMod]]

----
[[CategoryAPI]], [[CategoryRender]]

