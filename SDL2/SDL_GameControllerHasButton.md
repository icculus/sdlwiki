====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GameControllerHasButton =

Query whether a game controller has a given button.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_GameControllerHasButton(SDL_GameController *gamecontroller,
                                     SDL_GameControllerButton button);
</syntaxhighlight>

== Function Parameters ==

{|
|'''gamecontroller'''
|a game controller
|-
|'''button'''
|a button enum value (an [[SDL_GameControllerButton]] value)
|}

== Return Value ==

Returns [[SDL_TRUE]] if the controller has this button, [[SDL_FALSE]]
otherwise.

== Remarks ==

This merely reports whether the controller's mapping defined this button,
as that is all the information SDL has about the physical device.

== Version ==

This function is available since SDL 2.0.14.

----
[[CategoryAPI]]

