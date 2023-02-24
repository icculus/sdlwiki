====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GameControllerGetBindForAxis =

Get the SDL joystick layer binding for a controller axis mapping.

== Syntax ==

<syntaxhighlight lang='c'>
extern DECLSPEC SDL_GameControllerButtonBind SDLCALL
SDL_GameControllerGetBindForAxis(SDL_GameController *gamecontroller,
         SDL_GameControllerAxis axis);
</syntaxhighlight>

== Function Parameters ==

{|
|'''gamecontroller'''
|a game controller
|-
|'''axis'''
|an axis enum value (one of the [[SDL_GameControllerAxis]] values)
|}

== Return Value ==

Returns a [[SDL_GameControllerButtonBind]] describing the bind. On failure
(like the given Controller axis doesn't exist on the device), its
<code>.bindType</code> will be
<code>[[SDL_CONTROLLER_BINDTYPE_NONE]]</code>.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GameControllerGetBindForButton]]

----
[[CategoryAPI]]

