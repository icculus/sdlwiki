====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetWindowKeyboardGrab =

Get a window's keyboard grab mode.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_GetWindowKeyboardGrab(SDL_Window *window);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window to query
|}

== Return Value ==

Returns [[SDL_TRUE]] if keyboard is grabbed, and [[SDL_FALSE]] otherwise.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_SetWindowKeyboardGrab]]
:[[SDL_GetWindowGrab]]

----
[[CategoryAPI]]

