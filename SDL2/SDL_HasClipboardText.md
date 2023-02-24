====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
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

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GetClipboardText]]
:[[SDL_SetClipboardText]]

----
[[CategoryAPI]]

