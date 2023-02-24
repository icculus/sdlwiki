====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetTicksNS =

Get the number of nanoseconds since SDL library initialization.

== Syntax ==

<syntaxhighlight lang='c'>
Uint64 SDL_GetTicksNS(void);
</syntaxhighlight>

== Return Value ==

Returns an unsigned 64-bit value representing the number of nanoseconds
since the SDL library initialized.

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

