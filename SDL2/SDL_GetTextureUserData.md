###### (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)
# SDL_GetTextureUserData

Get the user-specified pointer associated with a texture

## Header File

Defined in [SDL_render.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_render.h), but apps should _only_ `#include "SDL.h"`!

## Syntax

```c
void * SDL_GetTextureUserData(SDL_Texture * texture);

```

## Function Parameters

|                 |                       |
| --------------- | --------------------- |
| **texture**     | the texture to query. |

## Return Value

Return the pointer associated with the texture, or NULL if the texture is
not valid.

## Version

This function is available since SDL 2.0.18.

## See Also

* [SDL_SetTextureUserData](SDL_SetTextureUserData)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction)

