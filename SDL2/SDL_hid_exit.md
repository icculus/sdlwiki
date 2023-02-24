====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
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

This function is available since SDL 2.0.18.

== Related Functions ==

:[[SDL_hid_init]]

----
[[CategoryAPI]]

