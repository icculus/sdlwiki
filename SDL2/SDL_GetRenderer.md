====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GetRenderer =

Get the renderer associated with a window.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Renderer * SDL_GetRenderer(SDL_Window * window);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window to query
|}

== Return Value ==

Returns the rendering context on success or NULL on failure; call
[[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_CreateRenderer]]

----
[[CategoryAPI]]

