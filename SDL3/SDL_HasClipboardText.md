====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_HasClipboardText =

Query whether the clipboard exists and contains a non-empty text string.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_HasClipboardText(void);
</syntaxhighlight>

== Return Value ==

Returns [[SDL_TRUE]] if the clipboard has text, or [[SDL_FALSE]] if it does
not.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetClipboardText]]
:[[SDL_SetClipboardText]]

----
[[CategoryAPI]], [[CategoryClipboard]]

