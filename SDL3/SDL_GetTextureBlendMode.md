====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetTextureBlendMode =

Get the blend mode used for texture copy operations.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_GetTextureBlendMode(SDL_Texture *texture, SDL_BlendMode *blendMode);
</syntaxhighlight>

== Function Parameters ==

{|
|'''texture'''
|the texture to query
|-
|'''blendMode'''
|a pointer filled in with the current [[SDL_BlendMode]]
|}

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_SetTextureBlendMode]]

----
[[CategoryAPI]], [[CategoryRender]]

