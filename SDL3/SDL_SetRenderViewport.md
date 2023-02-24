====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_SetRenderViewport =

Set the drawing area for rendering on the current target.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_SetRenderViewport(SDL_Renderer *renderer, const SDL_Rect *rect);
</syntaxhighlight>

== Function Parameters ==

{|
|'''renderer'''
|the rendering context
|-
|'''rect'''
|the [[SDL_Rect]] structure representing the drawing area, or NULL to set the viewport to the entire target
|}

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Remarks ==

When the window is resized, the viewport is reset to fill the entire new
window size.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetRenderViewport]]

----
[[CategoryAPI]]

