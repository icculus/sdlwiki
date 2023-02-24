====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetRenderer =

Get the renderer associated with a window.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Renderer* SDL_GetRenderer(SDL_Window *window);
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

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_CreateRenderer]]

----
[[CategoryAPI]], [[CategoryRender]]

