====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GameControllerGetAxisFromString =

Convert a string into [[SDL_GameControllerAxis]] enum.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_GameControllerAxis SDL_GameControllerGetAxisFromString(const char *str);
</syntaxhighlight>

== Function Parameters ==

{|
|'''str'''
|string representing a [[SDL_GameController]] axis
|}

== Return Value ==

Returns the [[SDL_GameControllerAxis]] enum corresponding to the input
string, or <code>[[SDL_CONTROLLER_AXIS_INVALID]]</code> if no match was
found.

== Remarks ==

This function is called internally to translate [[SDL_GameController]]
mapping strings for the underlying joystick device into the consistent
[[SDL_GameController]] mapping. You do not normally need to call this
function unless you are parsing [[SDL_GameController]] mappings in your own
code.

Note specially that "righttrigger" and "lefttrigger" map to
<code>[[SDL_CONTROLLER_AXIS_TRIGGERRIGHT]]</code> and
<code>[[SDL_CONTROLLER_AXIS_TRIGGERLEFT]]</code>, respectively.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GameControllerGetStringForAxis]]

----
[[CategoryAPI]]

