====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_UnlockJoysticks =

Unlocking for atomic access to the joystick API 

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_UnlockJoysticks(void) SDL_RELEASE(SDL_joystick_lock);
</syntaxhighlight>

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

