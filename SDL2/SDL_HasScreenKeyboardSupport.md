====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_HasScreenKeyboardSupport =

Check whether the platform has screen keyboard support.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_HasScreenKeyboardSupport(void);
</syntaxhighlight>

== Return Value ==

Returns [[SDL_TRUE]] if the platform has some screen keyboard support or
[[SDL_FALSE]] if not.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_StartTextInput]]
:[[SDL_IsScreenKeyboardShown]]

----
[[CategoryAPI]]

