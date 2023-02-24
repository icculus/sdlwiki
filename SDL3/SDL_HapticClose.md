====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======

== Draft ==

'''THIS PAGE IS A WORK IN PROGRESS''' ... Please make edits to this page to improve it!
= SDL_HapticClose =

Close a haptic device previously opened with [[SDL_HapticOpen]]().

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_HapticClose(SDL_Haptic * haptic);
</syntaxhighlight>

== Function Parameters ==

{|
|'''haptic'''
|the [[SDL_Haptic]] device to close
|}

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_HapticOpen]]

----
[[CategoryAPI]], [[CategoryForceFeedback]], [[CategoryDraft]]

