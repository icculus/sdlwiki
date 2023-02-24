====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_LogGetOutputFunction =

Get the current log output function.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_LogGetOutputFunction(SDL_LogOutputFunction *callback, void **userdata);
</syntaxhighlight>

== Function Parameters ==

{|
|'''callback'''
|an [[SDL_LogOutputFunction]] filled in with the current log callback
|-
|'''userdata'''
|a pointer filled in with the pointer that is passed to <code>callback</code>
|}

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_LogSetOutputFunction]]

----
[[CategoryAPI]]

