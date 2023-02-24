====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_HasARMSIMD =

Determine whether the CPU has ARM SIMD (ARMv6) features.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_HasARMSIMD(void);
</syntaxhighlight>

== Return Value ==

Returns [[SDL_TRUE]] if the CPU has ARM SIMD features or [[SDL_FALSE]] if
not.

== Remarks ==

This is different from ARM NEON, which is a different instruction set.

This always returns false on CPUs that aren't using ARM instruction sets.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_HasNEON]]

----
[[CategoryAPI]]

