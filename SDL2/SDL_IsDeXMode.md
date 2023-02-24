====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_IsDeXMode =

Query if the application is running on a Samsung DeX docking station.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_IsDeXMode(void);
</syntaxhighlight>

== Return Value ==

Returns [[SDL_TRUE]] if this is a DeX docking station, [[SDL_FALSE]]
otherwise.

== Version ==

This function is available since SDL 2.0.9.

----
[[CategoryAPI]]

