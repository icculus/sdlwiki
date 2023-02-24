====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_ResetKeyboard =

Clear the state of the keyboard 

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_ResetKeyboard(void);
</syntaxhighlight>

== Remarks ==

This function will generate key up events for all pressed keys.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetKeyboardState]]

----
[[CategoryAPI]]

