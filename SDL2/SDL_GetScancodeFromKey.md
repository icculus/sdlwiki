====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GetScancodeFromKey =

Get the scancode corresponding to the given key code according to the current keyboard layout.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Scancode SDL_GetScancodeFromKey(SDL_Keycode key);
</syntaxhighlight>

== Function Parameters ==

{|
|'''key'''
|the desired [[SDL_Keycode]] to query
|}

== Return Value ==

Returns the [[SDL_Scancode]] that corresponds to the given [[SDL_Keycode]].

== Remarks ==

See [[SDL_Scancode]] for details.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GetKeyFromScancode]]
:[[SDL_GetScancodeName]]

----
[[CategoryAPI]]

