====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GetScancodeFromName =

Get a scancode from a human-readable name.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Scancode SDL_GetScancodeFromName(const char *name);
</syntaxhighlight>

== Function Parameters ==

{|
|'''name'''
|the human-readable scancode name
|}

== Return Value ==

Returns the [[SDL_Scancode]], or <code>[[SDL_SCANCODE_UNKNOWN]]</code> if
the name wasn't recognized; call [[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GetKeyFromName]]
:[[SDL_GetScancodeFromKey]]
:[[SDL_GetScancodeName]]

----
[[CategoryAPI]]

