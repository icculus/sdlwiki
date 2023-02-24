====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_AndroidRequestPermission =

Request permissions at runtime.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_AndroidRequestPermission(const char *permission);
</syntaxhighlight>

== Function Parameters ==

{|
|'''permission'''
|The permission to request.
|}

== Return Value ==

Returns [[SDL_TRUE]] if the permission was granted, [[SDL_FALSE]]
otherwise.

== Remarks ==

This blocks the calling thread until the permission is granted or denied.

== Version ==

This function is available since SDL 2.0.14.

----
[[CategoryAPI]]

