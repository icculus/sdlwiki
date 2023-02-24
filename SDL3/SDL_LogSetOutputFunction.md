====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
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

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_LogGetOutputFunction]]

----
[[CategoryAPI]], [[CategoryLog]]

