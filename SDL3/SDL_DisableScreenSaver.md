====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_DisableScreenSaver =

Prevent the screen from being blanked by a screen saver.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_DisableScreenSaver(void);
</syntaxhighlight>

== Remarks ==

If you disable the screensaver, it is automatically re-enabled when SDL
quits.

The screensaver is disabled by default since SDL 2.0.2. Before SDL 2.0.2
the screensaver was enabled by default.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_EnableScreenSaver]]
:[[SDL_ScreenSaverEnabled]]

----
[[CategoryAPI]], [[CategoryVideo]]

