###### (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)
# SDL_RenderSetIntegerScale

Set whether to force integer scales for resolution-independent rendering.

## Header File

Defined in [SDL_render.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_render.h), but apps should _only_ `#include "SDL.h"`!

## Syntax

```c
int SDL_RenderSetIntegerScale(SDL_Renderer * renderer,
                              SDL_bool enable);

```

## Function Parameters

|                  |                                                      |
| ---------------- | ---------------------------------------------------- |
| **renderer**     | the renderer for which integer scaling should be set |
| **enable**       | enable or disable the integer scaling for rendering  |

## Return Value

Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

This function restricts the logical viewport to integer values - that is,
when a resolution is between two multiples of a logical size, the viewport
size is rounded down to the lower multiple.

## Version

This function is available since SDL 2.0.5.

## See Also

* [SDL_RenderGetIntegerScale](SDL_RenderGetIntegerScale)
* [SDL_RenderSetLogicalSize](SDL_RenderSetLogicalSize)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction)

