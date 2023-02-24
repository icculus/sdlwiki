====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetDesktopDisplayMode =

Get information about the desktop's display mode.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_GetDesktopDisplayMode(SDL_DisplayID displayID, SDL_DisplayMode *mode);
</syntaxhighlight>

== Function Parameters ==

{|
|'''displayID'''
|the instance ID of the display to query
|-
|'''mode'''
|an [[SDL_DisplayMode]] structure filled in with the current display mode
|}

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Remarks ==

There's a difference between this function and
[[SDL_GetCurrentDisplayMode]]() when SDL runs fullscreen and has changed
the resolution. In that case this function will return the previous native
display mode, and not the current display mode.

== Version ==

This function is available since SDL 3.0.0.

== Code Examples ==

<syntaxhighlight lang='c++'>
SDL_DisplayMode dm;
if (SDL_GetDesktopDisplayMode(0, &dm) != 0) {
    SDL_Log("SDL_GetDesktopDisplayMode failed: %s", SDL_GetError());
    return 1;
}
</syntaxhighlight>

== Related Functions ==

:[[SDL_GetCurrentDisplayMode]]
:[[SDL_GetDisplayMode]]
:[[SDL_SetWindowDisplayMode]]

----
[[CategoryAPI]], [[CategoryVideo]]

