====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_HasLASX =

Determine whether the CPU has LASX (LOONGARCH SIMD) features.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_HasLASX(void);
</syntaxhighlight>

== Return Value ==

Returns [[SDL_TRUE]] if the CPU has LOONGARCH LASX features or
[[SDL_FALSE]] if not.

== Remarks ==

This always returns false on CPUs that aren't using LOONGARCH instruction
sets.

== Version ==

This function is available since SDL 2.24.0.

----
[[CategoryAPI]]

