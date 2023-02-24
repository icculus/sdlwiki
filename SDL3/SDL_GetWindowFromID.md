====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetWindowFromID =

Get a window from a stored ID.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Window* SDL_GetWindowFromID(SDL_WindowID id);
</syntaxhighlight>

== Function Parameters ==

{|
|'''id'''
|the ID of the window
|}

== Return Value ==

Returns the window associated with <code>id</code> or NULL if it doesn't
exist; call [[SDL_GetError]]() for more information.

== Remarks ==

The numeric ID is what [[SDL_WindowEvent]] references, and is necessary to
map these events to specific [[SDL_Window]] objects.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetWindowID]]

----
[[CategoryAPI]], [[CategoryVideo]]

