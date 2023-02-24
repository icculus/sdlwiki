====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_LogSetPriority =

Set the priority of a particular log category.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_LogSetPriority(int category,
                        SDL_LogPriority priority);
</syntaxhighlight>

== Function Parameters ==

{|
|'''category'''
|the category to assign a priority to
|-
|'''priority'''
|the [[SDL_LogPriority]] to assign
|}

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_LogGetPriority]]
:[[SDL_LogSetAllPriority]]

----
[[CategoryAPI]], [[CategoryLog]]

