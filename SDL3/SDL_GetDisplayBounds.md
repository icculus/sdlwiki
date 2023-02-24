====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetDisplayBounds =

Get the desktop area represented by a display, in screen coordinates.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_GetDisplayBounds(SDL_DisplayID displayID, SDL_Rect *rect);
</syntaxhighlight>

== Function Parameters ==

{|
|'''displayID'''
|the instance ID of the display to query
|-
|'''rect'''
|the [[SDL_Rect]] structure filled in with the display bounds
|}

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Remarks ==

The primary display is always located at (0,0).

== Version ==

This function is available since SDL 3.0.0.

== Code Examples ==

<syntaxhighlight lang='c++'>
SDL_Rect r;
if (SDL_GetDisplayBounds(0, &r) != 0) {
    SDL_Log("SDL_GetDisplayBounds failed: %s", SDL_GetError());
    return 1;
}
</syntaxhighlight>

== Related Functions ==

:[[SDL_GetDisplayUsableBounds]]
:[[SDL_GetDisplays]]

----
[[CategoryAPI]], [[CategoryVideo]]

