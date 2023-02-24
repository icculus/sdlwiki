====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_SetHint =

Set a hint with normal priority.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_SetHint(const char *name,
                     const char *value);
</syntaxhighlight>

== Function Parameters ==

{|
|'''name'''
|the hint to set
|-
|'''value'''
|the value of the hint variable
|}

== Return Value ==

Returns [[SDL_TRUE]] if the hint was set, [[SDL_FALSE]] otherwise.

== Remarks ==

Hints will not be set if there is an existing override hint or environment
variable that takes precedence. You can use [[SDL_SetHintWithPriority]]()
to set the hint with override priority instead.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GetHint]]
:[[SDL_SetHintWithPriority]]

----
[[CategoryAPI]]

