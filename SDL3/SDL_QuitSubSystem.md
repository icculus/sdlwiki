====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_QuitSubSystem =

Shut down specific SDL subsystems.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_QuitSubSystem(Uint32 flags);
</syntaxhighlight>

== Function Parameters ==

{|
|'''flags'''
|any of the flags used by [[SDL_Init]](); see [[SDL_Init]] for details.
|}

== Remarks ==

You still need to call [[SDL_Quit]]() even if you close all open subsystems
with [[SDL_QuitSubSystem]]().

== Version ==

This function is available since SDL 3.0.0.

== Code Examples ==

<syntaxhighlight lang='c++'>
#include "SDL.h"

/* ... */

int main(int argc, char **argv) {
    int sdl_initialized = 0;
    sdl_initialized = !SDL_Init(0);

    /* ... console stuff ... */

    if (sdl_initialized && SDL_InitSubSystem(SDL_INIT_VIDEO)) {
        display_graph();
        SDL_QuitSubSystem(SDL_INIT_VIDEO);
    }

    /* ... more console stuff ... */

    if (sdl_initialized) SDL_Quit();
    return 0;
}
</syntaxhighlight>

== Related Functions ==

:[[SDL_InitSubSystem]]
:[[SDL_Quit]]

----
[[CategoryAPI]], [[CategoryInit]]

