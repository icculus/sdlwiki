====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_hid_exit =

Finalize the HIDAPI library.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_hid_exit(void);
</syntaxhighlight>

== Return Value ==

Returns 0 on success and -1 on error.

== Remarks ==

This function frees all of the static data associated with HIDAPI. It
should be called at the end of execution to avoid memory leaks.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_hid_init]]

----
[[CategoryAPI]]

