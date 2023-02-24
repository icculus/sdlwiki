====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_ClearError =

Clear any previous error message for this thread.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_ClearError(void);
</syntaxhighlight>

== Version ==

This function is available since SDL 3.0.0.

== Code Examples ==

<syntaxhighlight lang='c++'>
const char *error = SDL_GetError();
if (*error) {
  SDL_Log("SDL error: %s", error);
  SDL_ClearError();
}
</syntaxhighlight>

== Related Functions ==

:[[SDL_GetError]]
:[[SDL_SetError]]

----
[[CategoryAPI]], [[CategoryError]]

