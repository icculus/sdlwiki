====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======

== Draft ==

'''THIS PAGE IS A WORK IN PROGRESS''' ... Please make edits to this page to improve it!
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

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetKeyFromScancode]]
:[[SDL_GetScancodeName]]

----
[[CategoryAPI]], [[CategoryKeyboard]], [[CategoryDraft]]

