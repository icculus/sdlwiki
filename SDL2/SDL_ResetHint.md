====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_ResetHint =

Reset a hint to the default value.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_ResetHint(const char *name);
</syntaxhighlight>

== Function Parameters ==

{|
|'''name'''
|the hint to set
|}

== Return Value ==

Returns [[SDL_TRUE]] if the hint was set, [[SDL_FALSE]] otherwise.

== Remarks ==

This will reset a hint to the value of the environment variable, or NULL if
the environment isn't set. Callbacks will be called normally with this
change.

== Version ==

This function is available since SDL 2.24.0.

== Related Functions ==

:[[SDL_GetHint]]
:[[SDL_SetHint]]

----
[[CategoryAPI]]

