====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GameControllerGetBindForButton =

Get the SDL joystick layer binding for a controller button mapping.

== Syntax ==

<syntaxhighlight lang='c'>
extern DECLSPEC SDL_GameControllerButtonBind SDLCALL
SDL_GameControllerGetBindForButton(SDL_GameController *gamecontroller,
           SDL_GameControllerButton button);
</syntaxhighlight>

== Function Parameters ==

{|
|'''gamecontroller'''
|a game controller
|-
|'''button'''
|an button enum value (an [[SDL_GameControllerButton]] value)
|}

== Return Value ==

Returns a [[SDL_GameControllerButtonBind]] describing the bind. On failure
(like the given Controller button doesn't exist on the device), its
<code>.bindType</code> will be
<code>[[SDL_CONTROLLER_BINDTYPE_NONE]]</code>.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GameControllerGetBindForAxis]]

----
[[CategoryAPI]]

