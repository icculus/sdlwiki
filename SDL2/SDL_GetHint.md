====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GetHint =

Get the value of a hint.

== Syntax ==

<syntaxhighlight lang='c'>
const char * SDL_GetHint(const char *name);
</syntaxhighlight>

== Function Parameters ==

{|
|'''name'''
|the hint to query
|}

== Return Value ==

Returns the string value of a hint or NULL if the hint isn't set.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_SetHint]]
:[[SDL_SetHintWithPriority]]

----
[[CategoryAPI]]

