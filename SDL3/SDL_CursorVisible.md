====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_CursorVisible =

Return whether the cursor is currently being shown.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_CursorVisible(void);
</syntaxhighlight>

== Return Value ==

Returns <code>[[SDL_TRUE]]</code> if the cursor is being shown, or
<code>[[SDL_FALSE]]</code> if the cursor is hidden.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_HideCursor]]
:[[SDL_ShowCursor]]

----
[[CategoryAPI]]

