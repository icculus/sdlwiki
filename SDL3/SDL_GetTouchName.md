====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetTouchName =

Get the touch device name as reported from the driver or NULL if the index is invalid.

== Syntax ==

<syntaxhighlight lang='c'>
const char* SDL_GetTouchName(int index);
</syntaxhighlight>

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

