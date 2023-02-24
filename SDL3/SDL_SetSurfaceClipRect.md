====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_SetSurfaceClipRect =

Set the clipping rectangle for a surface.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_SetSurfaceClipRect(SDL_Surface *surface,
                         const SDL_Rect *rect);
</syntaxhighlight>

== Function Parameters ==

{|
|'''surface'''
|the [[SDL_Surface]] structure to be clipped
|-
|'''rect'''
|the [[SDL_Rect]] structure representing the clipping rectangle, or NULL to disable clipping
|}

== Return Value ==

Returns [[SDL_TRUE]] if the rectangle intersects the surface, otherwise
[[SDL_FALSE]] and blits will be completely clipped.

== Remarks ==

When <code>surface</code> is the destination of a blit, only the area
within the clip rectangle is drawn into.

Note that blits are automatically clipped to the edges of the source and
destination surfaces.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_BlitSurface]]
:[[SDL_GetSurfaceClipRect]]

----
[[CategoryAPI]]

