====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetRenderViewport =

Get the drawing area for the current target.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_GetRenderViewport(SDL_Renderer *renderer, SDL_Rect *rect);
</syntaxhighlight>

== Function Parameters ==

{|
|'''renderer'''
|the rendering context
|-
|'''rect'''
|an [[SDL_Rect]] structure filled in with the current drawing area
|}

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_SetRenderViewport]]

----
[[CategoryAPI]]

