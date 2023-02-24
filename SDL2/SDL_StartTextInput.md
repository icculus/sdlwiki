====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_StartTextInput =

Start accepting Unicode text input events.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_StartTextInput(void);
</syntaxhighlight>

== Remarks ==

This function will start accepting Unicode text input events in the focused
SDL window, and start emitting [[SDL_TextInputEvent]] ([[SDL_TEXTINPUT]])
and [[SDL_TextEditingEvent]] ([[SDL_TEXTEDITING]]) events. Please use this
function in pair with [[SDL_StopTextInput]]().

On some platforms using this function activates the screen keyboard.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_SetTextInputRect]]
:[[SDL_StopTextInput]]

----
[[CategoryAPI]]

