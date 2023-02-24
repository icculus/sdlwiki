====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_LoadDollarTemplates =

Load Dollar Gesture templates from a file.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_LoadDollarTemplates(SDL_TouchID touchId, SDL_RWops *src);
</syntaxhighlight>

== Function Parameters ==

{|
|'''touchId'''
|a touch id
|-
|'''src'''
|a [[SDL_RWops]] to load from
|}

== Return Value ==

Returns the number of loaded templates on success or a negative error code
(or 0) on failure; call [[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_SaveAllDollarTemplates]]
:[[SDL_SaveDollarTemplate]]

----
[[CategoryAPI]]

