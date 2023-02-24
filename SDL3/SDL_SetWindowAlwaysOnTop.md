====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_SetWindowAlwaysOnTop =

Set the window to always be above the others.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_SetWindowAlwaysOnTop(SDL_Window *window, SDL_bool on_top);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|The window of which to change the always on top state
|-
|'''on_top'''
|[[SDL_TRUE]] to set the window always on top, [[SDL_FALSE]] to disable
|}

== Remarks ==

This will add or remove the window's
<code>[[SDL_WINDOW_ALWAYS_ON_TOP]]</code> flag. This will bring the window
to the front and keep the window above the rest.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetWindowFlags]]

----
[[CategoryAPI]]

