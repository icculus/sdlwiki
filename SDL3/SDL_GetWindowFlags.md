====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetWindowFlags =

Get the window flags.

== Syntax ==

<syntaxhighlight lang='c'>
Uint32 SDL_GetWindowFlags(SDL_Window *window);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window to query
|}

== Return Value ==

Returns a mask of the [[SDL_WindowFlags]] associated with
<code>window</code>

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_CreateWindow]]
:[[SDL_HideWindow]]
:[[SDL_MaximizeWindow]]
:[[SDL_MinimizeWindow]]
:[[SDL_SetWindowFullscreen]]
:[[SDL_SetWindowGrab]]
:[[SDL_ShowWindow]]

----
[[CategoryAPI]], [[CategoryVideo]]

