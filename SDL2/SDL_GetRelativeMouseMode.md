====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GetRelativeMouseMode =

Query whether relative mouse mode is enabled.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_GetRelativeMouseMode(void);
</syntaxhighlight>

== Return Value ==

Returns [[SDL_TRUE]] if relative mode is enabled or [[SDL_FALSE]]
otherwise.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_SetRelativeMouseMode]]

----
[[CategoryAPI]]

