====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_RemoveTimer =

Remove a timer created with [[SDL_AddTimer]]().

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_RemoveTimer(SDL_TimerID id);
</syntaxhighlight>

== Function Parameters ==

{|
|'''id'''
|the ID of the timer to remove
|}

== Return Value ==

Returns [[SDL_TRUE]] if the timer is removed or [[SDL_FALSE]] if the timer
wasn't found.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_AddTimer]]

----
[[CategoryAPI]]

