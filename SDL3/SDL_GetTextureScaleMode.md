====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetTextureScaleMode =

Get the scale mode used for texture scale operations.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_GetTextureScaleMode(SDL_Texture *texture, SDL_ScaleMode *scaleMode);
</syntaxhighlight>

== Function Parameters ==

{|
|'''texture'''
|the texture to query.
|-
|'''scaleMode'''
|a pointer filled in with the current scale mode.
|}

== Return Value ==

Return 0 on success, or -1 if the texture is not valid.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_SetTextureScaleMode]]

----
[[CategoryAPI]]

