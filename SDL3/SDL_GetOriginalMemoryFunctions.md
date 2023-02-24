====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetOriginalMemoryFunctions =

Get the original set of SDL memory functions 

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_GetOriginalMemoryFunctions(SDL_malloc_func *malloc_func,
                                    SDL_calloc_func *calloc_func,
                                    SDL_realloc_func *realloc_func,
                                    SDL_free_func *free_func);
</syntaxhighlight>

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

