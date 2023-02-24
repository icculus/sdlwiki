====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_LogGetPriority =

Get the priority of a particular log category.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_LogPriority SDL_LogGetPriority(int category);
</syntaxhighlight>

== Function Parameters ==

{|
|'''category'''
|the category to query
|}

== Return Value ==

Returns the [[SDL_LogPriority]] for the requested category

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_LogSetPriority]]

----
[[CategoryAPI]], [[CategoryLog]]

