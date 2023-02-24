====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_IsTablet =

Query if the current device is a tablet.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_IsTablet(void);
</syntaxhighlight>

== Return Value ==

Returns [[SDL_TRUE]] if the device is a tablet, [[SDL_FALSE]] otherwise.

== Remarks ==

If SDL can't determine this, it will return [[SDL_FALSE]].

== Version ==

This function is available since SDL 2.0.9.

----
[[CategoryAPI]]

