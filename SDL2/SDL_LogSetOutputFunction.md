====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_LogSetOutputFunction =

Replace the default log output function with one of your own.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_LogSetOutputFunction(SDL_LogOutputFunction callback, void *userdata);
</syntaxhighlight>

== Function Parameters ==

{|
|'''callback'''
|an [[SDL_LogOutputFunction]] to call instead of the default
|-
|'''userdata'''
|a pointer that is passed to <code>callback</code>
|}

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_LogGetOutputFunction]]

----
[[CategoryAPI]]

