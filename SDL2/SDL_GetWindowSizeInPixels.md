====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GetWindowSizeInPixels =

Get the size of a window in pixels.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_GetWindowSizeInPixels(SDL_Window * window,
                               int *w, int *h);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window from which the drawable size should be queried
|-
|'''w'''
|a pointer to variable for storing the width in pixels, may be NULL
|-
|'''h'''
|a pointer to variable for storing the height in pixels, may be NULL
|}

== Remarks ==

This may differ from [[SDL_GetWindowSize]]() if we're rendering to a
high-DPI drawable, i.e. the window was created with
<code>[[SDL_WINDOW_ALLOW_HIGHDPI]]</code> on a platform with high-DPI
support (Apple calls this "Retina"), and not disabled by the
<code>[[SDL_HINT_VIDEO_HIGHDPI_DISABLED]]</code> hint.

== Version ==

This function is available since SDL 2.26.0.

== Related Functions ==

:[[SDL_CreateWindow]]
:[[SDL_GetWindowSize]]

----
[[CategoryAPI]]

