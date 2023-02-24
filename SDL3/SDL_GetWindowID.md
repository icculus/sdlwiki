====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetWindowID =

Get the numeric ID of a window.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_WindowID SDL_GetWindowID(SDL_Window *window);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window to query
|}

== Return Value ==

Returns the ID of the window on success or 0 on failure; call
[[SDL_GetError]]() for more information.

== Remarks ==

The numeric ID is what [[SDL_WindowEvent]] references, and is necessary to
map these events to specific [[SDL_Window]] objects.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetWindowFromID]]

----
[[CategoryAPI]], [[CategoryVideo]]

