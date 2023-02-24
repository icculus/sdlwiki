====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_Metal_DestroyView =

Destroy an existing [[SDL_MetalView]] object.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_Metal_DestroyView(SDL_MetalView view);
</syntaxhighlight>

== Remarks ==

This should be called before [[SDL_DestroyWindow]], if
[[SDL_Metal_CreateView]] was called after [[SDL_CreateWindow]].

== Version ==

This function is available since SDL 2.0.12.

== Related Functions ==

:[[SDL_Metal_CreateView]]

----
[[CategoryAPI]]

