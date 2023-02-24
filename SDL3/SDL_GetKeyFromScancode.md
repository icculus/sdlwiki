====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======

== Draft ==

'''THIS PAGE IS A WORK IN PROGRESS''' ... Please make edits to this page to improve it!
= SDL_GetKeyFromScancode =

Get the key code corresponding to the given scancode according to the current keyboard layout.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Keycode SDL_GetKeyFromScancode(SDL_Scancode scancode);
</syntaxhighlight>

== Function Parameters ==

{|
|'''scancode'''
|the desired [[SDL_Scancode]] to query
|}

== Return Value ==

Returns the [[SDL_Keycode]] that corresponds to the given [[SDL_Scancode]].

== Remarks ==

See [[SDL_Keycode]] for details.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetKeyName]]
:[[SDL_GetScancodeFromKey]]

----
[[CategoryAPI]], [[CategoryKeyboard]], [[CategoryDraft]]

