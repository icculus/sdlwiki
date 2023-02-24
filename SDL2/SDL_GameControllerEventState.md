====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GameControllerEventState =

Query or change current state of Game Controller events.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_GameControllerEventState(int state);
</syntaxhighlight>

== Function Parameters ==

{|
|'''state'''
|can be one of <code>[[SDL_QUERY]]</code>, <code>[[SDL_IGNORE]]</code>, or <code>[[SDL_ENABLE]]</code>
|}

== Return Value ==

Returns the same value passed to the function, with exception to -1
([[SDL_QUERY]]), which will return the current state.

== Remarks ==

If controller events are disabled, you must call
[[SDL_GameControllerUpdate]]() yourself and check the state of the
controller when you want controller information.

Any number can be passed to [[SDL_GameControllerEventState]](), but only
-1, 0, and 1 will have any effect. Other numbers will just be returned.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_JoystickEventState]]

----
[[CategoryAPI]]

