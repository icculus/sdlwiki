====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GetPerformanceFrequency =

Get the count per second of the high resolution counter.

== Syntax ==

<syntaxhighlight lang='c'>
Uint64 SDL_GetPerformanceFrequency(void);
</syntaxhighlight>

== Return Value ==

Returns a platform-specific count per second.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GetPerformanceCounter]]

----
[[CategoryAPI]]

