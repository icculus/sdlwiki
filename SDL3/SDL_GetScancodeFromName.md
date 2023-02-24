====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======

== Draft ==

'''THIS PAGE IS A WORK IN PROGRESS''' ... Please make edits to this page to improve it!
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

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetKeyFromName]]
:[[SDL_GetScancodeFromKey]]
:[[SDL_GetScancodeName]]

----
[[CategoryAPI]], [[CategoryKeyboard]], [[CategoryDraft]]

