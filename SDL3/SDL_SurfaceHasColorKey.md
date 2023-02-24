====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_SurfaceHasColorKey =

Returns whether the surface has a color key 

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_SurfaceHasColorKey(SDL_Surface *surface);
</syntaxhighlight>

== Function Parameters ==

{|
|'''surface'''
|the [[SDL_Surface]] structure to query
|}

== Return Value ==

Return [[SDL_TRUE]] if the surface has a color key, [[SDL_FALSE]]
otherwise.

== Remarks ==

It is safe to pass a NULL <code>surface</code> here; it will return
[[SDL_FALSE]].

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_SetSurfaceColorKey]]
:[[SDL_GetSurfaceColorKey]]

----
[[CategoryAPI]]

