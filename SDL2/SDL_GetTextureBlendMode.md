====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GetTextureBlendMode =

Get the blend mode used for texture copy operations.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_GetTextureBlendMode(SDL_Texture * texture,
                            SDL_BlendMode *blendMode);
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

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_SetTextureBlendMode]]

----
[[CategoryAPI]]

