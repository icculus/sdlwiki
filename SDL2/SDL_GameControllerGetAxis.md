====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GameControllerGetAxis =

Get the current state of an axis control on a game controller.

== Syntax ==

<syntaxhighlight lang='c'>
extern DECLSPEC Sint16 SDLCALL
SDL_GameControllerGetAxis(SDL_GameController *gamecontroller, SDL_GameControllerAxis axis);
</syntaxhighlight>

== Function Parameters ==

{|
|'''gamecontroller'''
|a game controller
|-
|'''axis'''
|an axis index (one of the [[SDL_GameControllerAxis]] values)
|}

== Return Value ==

Returns axis state (including 0) on success or 0 (also) on failure; call
[[SDL_GetError]]() for more information.

== Remarks ==

The axis indices start at index 0.

The state is a value ranging from -32768 to 32767. Triggers, however, range
from 0 to 32767 (they never return a negative value).

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GameControllerGetButton]]

----
[[CategoryAPI]]

