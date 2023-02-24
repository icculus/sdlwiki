====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_WinRTRunApp =

Initialize and launch an SDL/WinRT application.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_WinRTRunApp(SDL_main_func mainFunction, void * reserved);
</syntaxhighlight>

== Function Parameters ==

{|
|'''mainFunction'''
|the SDL app's C-style main(), an [[SDL_main_func]]
|-
|'''reserved'''
|reserved for future use; should be NULL
|}

== Return Value ==

Returns 0 on success or -1 on failure; call [[SDL_GetError]]() to retrieve
more information on the failure.

== Version ==

This function is available since SDL 2.0.3.

----
[[CategoryAPI]]

