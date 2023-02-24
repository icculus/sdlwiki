====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======

== Draft ==

'''THIS PAGE IS A WORK IN PROGRESS''' ... Please make edits to this page to improve it!
= SDL_GetRelativeMouseMode =

Query whether relative mouse mode is enabled.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_GetRelativeMouseMode(void);
</syntaxhighlight>

== Return Value ==

Returns [[SDL_TRUE]] if relative mode is enabled or [[SDL_FALSE]]
otherwise.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_SetRelativeMouseMode]]

----
[[CategoryAPI]], [[CategoryMouse]], [[CategoryDraft]]

