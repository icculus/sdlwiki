====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_SoftStretchLinear =

Perform bilinear scaling between two surfaces of the same format, 32BPP.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_SoftStretchLinear(SDL_Surface *src,
                    const SDL_Rect *srcrect,
                    SDL_Surface *dst,
                    const SDL_Rect *dstrect);
</syntaxhighlight>

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

