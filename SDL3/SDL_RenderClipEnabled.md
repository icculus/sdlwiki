====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_RenderClipEnabled =

Get whether clipping is enabled on the given renderer.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_RenderClipEnabled(SDL_Renderer *renderer);
</syntaxhighlight>

== Function Parameters ==

{|
|'''renderer'''
|the renderer from which clip state should be queried
|}

== Return Value ==

Returns [[SDL_TRUE]] if clipping is enabled or [[SDL_FALSE]] if not; call
[[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetRenderClipRect]]
:[[SDL_SetRenderClipRect]]

----
[[CategoryAPI]]

