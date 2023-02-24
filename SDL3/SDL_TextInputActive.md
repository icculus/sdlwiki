====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_TextInputActive =

Check whether or not Unicode text input events are enabled.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_TextInputActive(void);
</syntaxhighlight>

== Return Value ==

Returns [[SDL_TRUE]] if text input events are enabled else [[SDL_FALSE]].

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_StartTextInput]]

----
[[CategoryAPI]]

