====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_SetTextureScaleMode =

Set the scale mode used for texture scale operations.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_SetTextureScaleMode(SDL_Texture *texture, SDL_ScaleMode scaleMode);
</syntaxhighlight>

== Function Parameters ==

{|
|'''texture'''
|The texture to update.
|-
|'''scaleMode'''
|the [[SDL_ScaleMode]] to use for texture scaling.
|}

== Return Value ==

Returns 0 on success, or -1 if the texture is not valid.

== Remarks ==

If the scale mode is not supported, the closest supported mode is chosen.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetTextureScaleMode]]

----
[[CategoryAPI]]

