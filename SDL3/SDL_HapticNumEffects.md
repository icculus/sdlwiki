====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======

== Draft ==

'''THIS PAGE IS A WORK IN PROGRESS''' ... Please make edits to this page to improve it!
= SDL_HapticNumEffects =

Get the number of effects a haptic device can store.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_HapticNumEffects(SDL_Haptic * haptic);
</syntaxhighlight>

== Function Parameters ==

{|
|'''haptic'''
|the [[SDL_Haptic]] device to query
|}

== Return Value ==

Returns the number of effects the haptic device can store or a negative
error code on failure; call [[SDL_GetError]]() for more information.

== Remarks ==

On some platforms this isn't fully supported, and therefore is an
approximation. Always check to see if your created effect was actually
created and do not rely solely on [[SDL_HapticNumEffects]]().

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_HapticNumEffectsPlaying]]
:[[SDL_HapticQuery]]

----
[[CategoryAPI]], [[CategoryForceFeedback]], [[CategoryDraft]]

