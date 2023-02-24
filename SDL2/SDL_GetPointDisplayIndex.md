====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GetPointDisplayIndex =

Get the index of the display containing a point 

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_GetPointDisplayIndex(const SDL_Point * point);
</syntaxhighlight>

== Function Parameters ==

{|
|'''point'''
|the point to query
|}

== Return Value ==

Returns the index of the display containing the point or a negative error
code on failure; call [[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 2.24.0.

== Related Functions ==

:[[SDL_GetDisplayBounds]]
:[[SDL_GetNumVideoDisplays]]

----
[[CategoryAPI]]

