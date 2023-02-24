====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_LoadObject =

Dynamically load a shared object.

== Syntax ==

<syntaxhighlight lang='c'>
void* SDL_LoadObject(const char *sofile);
</syntaxhighlight>

== Function Parameters ==

{|
|'''sofile'''
|a system-dependent name of the object file
|}

== Return Value ==

Returns an opaque pointer to the object handle or NULL if there was an
error; call [[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 3.0.0.

== Code Examples ==

<syntaxhighlight lang='c++'>
#include "SDL.h"

/* Dynamically load mylib.so */
SDL_LoadObject("mylib.so");
</syntaxhighlight>

== Related Functions ==

:[[SDL_LoadFunction]]
:[[SDL_UnloadObject]]

----
[[CategoryAPI]], [[CategorySharedObject]]

