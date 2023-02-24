====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_HasAltiVec =

Determine whether the CPU has AltiVec features.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_HasAltiVec(void);
</syntaxhighlight>

== Return Value ==

Returns [[SDL_TRUE]] if the CPU has AltiVec features or [[SDL_FALSE]] if
not.

== Remarks ==

This always returns false on CPUs that aren't using PowerPC instruction
sets.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_HasAVX]]
:[[SDL_HasAVX2]]
:[[SDL_HasMMX]]
:[[SDL_HasRDTSC]]
:[[SDL_HasSSE]]
:[[SDL_HasSSE2]]
:[[SDL_HasSSE3]]
:[[SDL_HasSSE41]]
:[[SDL_HasSSE42]]

----
[[CategoryAPI]], [[CategoryCPU]]

