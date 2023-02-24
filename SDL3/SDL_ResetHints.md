====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_ResetHints =

Reset all hints to the default values.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_ResetHints(void);
</syntaxhighlight>

== Remarks ==

This will reset all hints to the value of the associated environment
variable, or NULL if the environment isn't set. Callbacks will be called
normally with this change.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetHint]]
:[[SDL_SetHint]]
:[[SDL_ResetHint]]

----
[[CategoryAPI]]

