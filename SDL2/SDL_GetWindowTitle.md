====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GetWindowTitle =

Get the title of a window.

== Syntax ==

<syntaxhighlight lang='c'>
const char* SDL_GetWindowTitle(SDL_Window * window);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window to query
|}

== Return Value ==

Returns the title of the window in UTF-8 format or "" if there is no title.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_SetWindowTitle]]

----
[[CategoryAPI]]

