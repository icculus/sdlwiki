====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetSurfaceClipRect =

Get the clipping rectangle for a surface.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_GetSurfaceClipRect(SDL_Surface *surface,
                     SDL_Rect *rect);
</syntaxhighlight>

== Function Parameters ==

{|
|'''surface'''
|the [[SDL_Surface]] structure representing the surface to be clipped
|-
|'''rect'''
|an [[SDL_Rect]] structure filled in with the clipping rectangle for the surface
|}

== Remarks ==

When <code>surface</code> is the destination of a blit, only the area
within the clip rectangle is drawn into.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_BlitSurface]]
:[[SDL_SetSurfaceClipRect]]

----
[[CategoryAPI]]

