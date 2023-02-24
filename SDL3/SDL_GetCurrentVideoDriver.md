====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetCurrentVideoDriver =

Get the name of the currently initialized video driver.

== Syntax ==

<syntaxhighlight lang='c'>
const char* SDL_GetCurrentVideoDriver(void);
</syntaxhighlight>

== Return Value ==

Returns the name of the current video driver or NULL if no driver has been
initialized.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetNumVideoDrivers]]
:[[SDL_GetVideoDriver]]

----
[[CategoryAPI]], [[CategoryVideo]]

