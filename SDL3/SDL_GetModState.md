====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======

== Draft ==

'''THIS PAGE IS A WORK IN PROGRESS''' ... Please make edits to this page to improve it!
= SDL_GetModState =

Get the current key modifier state for the keyboard.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Keymod SDL_GetModState(void);
</syntaxhighlight>

== Return Value ==

Returns an OR'd combination of the modifier keys for the keyboard. See
[[SDL_Keymod]] for details.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetKeyboardState]]
:[[SDL_SetModState]]

----
[[CategoryAPI]], [[CategoryKeyboard]], [[CategoryDraft]]

