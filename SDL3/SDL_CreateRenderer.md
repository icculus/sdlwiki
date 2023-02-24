====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_CreateRenderer =

Create a 2D rendering context for a window.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Renderer* SDL_CreateRenderer(SDL_Window *window, const char *name, Uint32 flags);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window where rendering is displayed
|-
|'''name'''
|the name of the rendering driver to initialize, or NULL to initialize the first one supporting the requested flags
|-
|'''flags'''
|0, or one or more [[SDL_RendererFlags]] OR'd together
|}

== Return Value ==

Returns a valid rendering context or NULL if there was an error; call
[[SDL_GetError]]() for more information.

== Remarks ==

If you want a specific renderer, you can specify its name here. A list of
available renderers can be obtained by calling [[SDL_GetRenderDriver]]
multiple times, with indices from 0 to [[SDL_GetNumRenderDrivers]]()-1. If
you don't need a specific renderer, specify NULL and SDL will attempt to
chooes the best option for you, based on what is available on the user's
system.

== Version ==

This function is available since SDL 3.0.0.

== Code Examples ==

<syntaxhighlight lang='c++'>
#include <SDL3/SDL.h>
#include <SDL3/SDL_main.h>

int main(int argc, char *argv[])
{
    SDL_Window *win = NULL;
    SDL_Renderer *renderer = NULL;
    SDL_Texture *bitmapTex = NULL;
    SDL_Surface *bitmapSurface = NULL;
    int posX = 100, posY = 100, width = 320, height = 240;
    SDL_bool loopShouldStop = SDL_FALSE;

    SDL_Init(SDL_INIT_VIDEO);

    win = SDL_CreateWindow("Hello World", posX, posY, width, height, 0);

    renderer = SDL_CreateRenderer(win, NULL, SDL_RENDERER_ACCELERATED);

    bitmapSurface = SDL_LoadBMP("img/hello.bmp");
    bitmapTex = SDL_CreateTextureFromSurface(renderer, bitmapSurface);
    SDL_DestroySurface(bitmapSurface);

    while (!loopShouldStop)
    {
        SDL_Event event;
        while (SDL_PollEvent(&event))
        {
            switch (event.type)
            {
                case SDL_EVENT_QUIT:
                    loopShouldStop = SDL_TRUE;
                    break;
            }
        }

        SDL_RenderClear(renderer);
        SDL_RenderTexture(renderer, bitmapTex, NULL, NULL);
        SDL_RenderPresent(renderer);
    }

    SDL_DestroyTexture(bitmapTex);
    SDL_DestroyRenderer(renderer);
    SDL_DestroyWindow(win);

    SDL_Quit();

    return 0;
}
</syntaxhighlight>

== Related Functions ==

:[[SDL_CreateSoftwareRenderer]]
:[[SDL_DestroyRenderer]]
:[[SDL_GetNumRenderDrivers]]
:[[SDL_GetRenderDriver]]
:[[SDL_GetRendererInfo]]

----
[[CategoryAPI]], [[CategoryRender]]

