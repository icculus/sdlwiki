====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_HasAVX512F =

Determine whether the CPU has AVX-512F (foundation) features.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_HasAVX512F(void);
</syntaxhighlight>

== Return Value ==

Returns [[SDL_TRUE]] if the CPU has AVX-512F features or [[SDL_FALSE]] if
not.

== Remarks ==

This always returns false on CPUs that aren't using Intel instruction sets.

== Version ==

This function is available since SDL 2.0.9.

== Related Functions ==

:[[SDL_HasAVX]]

----
[[CategoryAPI]]

