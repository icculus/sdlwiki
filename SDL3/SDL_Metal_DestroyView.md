====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
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

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_Metal_CreateView]]

----
[[CategoryAPI]]

