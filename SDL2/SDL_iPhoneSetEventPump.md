###### (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)
# SDL_iPhoneSetEventPump

Use this function to enable or disable the SDL event pump on Apple iOS.

## Header File

Defined in [SDL_system.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_system.h), but apps should _only_ `#include "SDL.h"`!

## Syntax

```c
void SDL_iPhoneSetEventPump(SDL_bool enabled);

```

## Function Parameters

|                 |                                                                                     |
| --------------- | ----------------------------------------------------------------------------------- |
| **enabled**     | [SDL_TRUE](SDL_TRUE) to enable the event pump, [SDL_FALSE](SDL_FALSE) to disable it |

## Remarks

This function is only available on Apple iOS.

This functions is also accessible using the macro
[SDL_iOSSetEventPump](SDL_iOSSetEventPump)() since SDL 2.0.4.

## Version

This function is available since SDL 2.0.0.

## See Also

* [SDL_iPhoneSetAnimationCallback](SDL_iPhoneSetAnimationCallback)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction)

