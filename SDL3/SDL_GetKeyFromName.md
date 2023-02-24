====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======

== Draft ==

'''THIS PAGE IS A WORK IN PROGRESS''' ... Please make edits to this page to improve it!
= SDL_GetKeyFromName =

Get a key code from a human-readable name.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Keycode SDL_GetKeyFromName(const char *name);
</syntaxhighlight>

== Function Parameters ==

{|
|'''name'''
|the human-readable key name
|}

== Return Value ==

Returns key code, or <code>[[SDLK_UNKNOWN]]</code> if the name wasn't
recognized; call [[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetKeyFromScancode]]
:[[SDL_GetKeyName]]
:[[SDL_GetScancodeFromName]]

----
[[CategoryAPI]], [[CategoryKeyboard]], [[CategoryDraft]]

