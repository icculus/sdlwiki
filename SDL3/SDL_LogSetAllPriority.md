====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_LogSetAllPriority =

Set the priority of all log categories.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_LogSetAllPriority(SDL_LogPriority priority);
</syntaxhighlight>

== Function Parameters ==

{|
|'''priority'''
|the [[SDL_LogPriority]] to assign
|}

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_LogSetPriority]]

----
[[CategoryAPI]], [[CategoryLog]]

