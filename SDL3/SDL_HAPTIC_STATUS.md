###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_HAPTIC_STATUS

Device can be queried for effect status.

## Header File

Defined in [SDL_haptic.h](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_haptic.h), but apps should _only_ `#include <SDL3/SDL.h>`!

## Syntax

```c
#define SDL_HAPTIC_STATUS     (1u<<18)
```

## Remarks

Device supports querying effect status.

## Version

This macro is available since SDL 3.0.0.

## See Also

* [SDL_GetHapticEffectStatus](SDL_GetHapticEffectStatus)

----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro)

