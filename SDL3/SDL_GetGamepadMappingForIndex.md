====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetGamepadMappingForIndex =

Get the mapping at a particular index.

== Syntax ==

<syntaxhighlight lang='c'>
char * SDL_GetGamepadMappingForIndex(int mapping_index);
</syntaxhighlight>

== Return Value ==

Returns the mapping string. Must be freed with [[SDL_free]](). Returns NULL
if the index is out of range.

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

