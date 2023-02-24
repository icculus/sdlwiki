====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_SoftStretchLinear =

Perform bilinear scaling between two surfaces of the same format, 32BPP.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_SoftStretchLinear(SDL_Surface * src,
                    const SDL_Rect * srcrect,
                    SDL_Surface * dst,
                    const SDL_Rect * dstrect);
</syntaxhighlight>

== Version ==

This function is available since SDL 2.0.16.

----
[[CategoryAPI]]

