====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_HasAVX2 =

Determine whether the CPU has AVX2 features.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_HasAVX2(void);
</syntaxhighlight>

== Return Value ==

Returns [[SDL_TRUE]] if the CPU has AVX2 features or [[SDL_FALSE]] if not.

== Remarks ==

This always returns false on CPUs that aren't using Intel instruction sets.

== Version ==

This function is available since SDL 2.0.4.

== Related Functions ==

:[[SDL_Has3DNow]]
:[[SDL_HasAltiVec]]
:[[SDL_HasAVX]]
:[[SDL_HasMMX]]
:[[SDL_HasRDTSC]]
:[[SDL_HasSSE]]
:[[SDL_HasSSE2]]
:[[SDL_HasSSE3]]
:[[SDL_HasSSE41]]
:[[SDL_HasSSE42]]

----
[[CategoryAPI]]

