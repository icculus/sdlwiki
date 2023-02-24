====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetRenderClipRect =

Get the clip rectangle for the current target.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_GetRenderClipRect(SDL_Renderer *renderer, SDL_Rect *rect);
</syntaxhighlight>

== Function Parameters ==

{|
|'''renderer'''
|the rendering context from which clip rectangle should be queried
|-
|'''rect'''
|an [[SDL_Rect]] structure filled in with the current clipping area or an empty rectangle if clipping is disabled
|}

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_RenderClipEnabled]]
:[[SDL_SetRenderClipRect]]

----
[[CategoryAPI]]

