====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GetMemoryFunctions =

Get the current set of SDL memory functions 

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_GetMemoryFunctions(SDL_malloc_func *malloc_func,
                            SDL_calloc_func *calloc_func,
                            SDL_realloc_func *realloc_func,
                            SDL_free_func *free_func);
</syntaxhighlight>

== Version ==

This function is available since SDL 2.0.7.

----
[[CategoryAPI]]

