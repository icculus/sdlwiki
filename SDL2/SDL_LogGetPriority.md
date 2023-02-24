====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
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

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_LogSetPriority]]

----
[[CategoryAPI]]

