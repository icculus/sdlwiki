====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======

== Draft ==

'''THIS PAGE IS A WORK IN PROGRESS''' ... Please make edits to this page to improve it!
= SDL_MouseIsHaptic =

Query whether or not the current mouse has haptic capabilities.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_MouseIsHaptic(void);
</syntaxhighlight>

== Return Value ==

Returns [[SDL_TRUE]] if the mouse is haptic or [[SDL_FALSE]] if it isn't.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_HapticOpenFromMouse]]

----
[[CategoryAPI]], [[CategoryForceFeedback]], [[CategoryDraft]]

