====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_HasPrimarySelectionText =

Query whether the primary selection exists and contains a non-empty text string.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_HasPrimarySelectionText(void);
</syntaxhighlight>

== Return Value ==

Returns [[SDL_TRUE]] if the primary selection has text, or [[SDL_FALSE]] if
it does not.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetPrimarySelectionText]]
:[[SDL_SetPrimarySelectionText]]

----
[[CategoryAPI]]

