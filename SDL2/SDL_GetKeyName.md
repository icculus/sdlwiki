====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GetKeyName =

Get a human-readable name for a key.

== Syntax ==

<syntaxhighlight lang='c'>
const char* SDL_GetKeyName(SDL_Keycode key);
</syntaxhighlight>

== Function Parameters ==

{|
|'''key'''
|the desired [[SDL_Keycode]] to query
|}

== Return Value ==

Returns a pointer to a UTF-8 string that stays valid at least until the
next call to this function. If you need it around any longer, you must copy
it. If the key doesn't have a name, this function returns an empty string
("").

== Remarks ==

See [[SDL_Scancode]] and [[SDL_Keycode]] for details.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GetKeyFromName]]
:[[SDL_GetKeyFromScancode]]
:[[SDL_GetScancodeFromKey]]

----
[[CategoryAPI]]

