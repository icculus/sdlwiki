###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_JoystickID

This is a unique ID for a joystick for the time it is connected to the system, and is never reused for the lifetime of the application.

## Header File

Defined in [SDL_joystick.h](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_joystick.h), but apps should _only_ `#include <SDL3/SDL.h>`!

## Syntax

```c
typedef Uint32 SDL_JoystickID;
```

## Remarks

If the joystick is disconnected and reconnected, it will get a new ID.

The ID value starts at 1 and increments from there. The value 0 is an
invalid ID.

## Version

This datatype is available since SDL 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIDatatype](CategoryAPIDatatype)

