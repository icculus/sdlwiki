====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetGamepadAppleSFSymbolsNameForButton =

Return the sfSymbolsName for a given button on a gamepad on Apple platforms.

== Syntax ==

<syntaxhighlight lang='c'>
const char* SDL_GetGamepadAppleSFSymbolsNameForButton(SDL_Gamepad *gamepad, SDL_GamepadButton button);
</syntaxhighlight>

== Function Parameters ==

{|
|'''gamepad'''
|the gamepad to query
|-
|'''button'''
|a button on the gamepad
|}

== Return Value ==

Returns the sfSymbolsName or NULL if the name can't be found

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetGamepadAppleSFSymbolsNameForAxis]]

----
[[CategoryAPI]]

