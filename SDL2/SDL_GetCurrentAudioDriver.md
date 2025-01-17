###### (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)
# SDL_GetCurrentAudioDriver

Get the name of the current audio driver.

## Header File

Defined in [SDL_audio.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_audio.h), but apps should _only_ `#include "SDL.h"`!

## Syntax

```c
const char* SDL_GetCurrentAudioDriver(void);

```

## Return Value

Returns the name of the current audio driver or NULL if no driver has been
initialized.

## Remarks

The returned string points to internal static memory and thus never becomes
invalid, even if you quit the audio subsystem and initialize a new driver
(although such a case would return a different static string from another
call to this function, of course). As such, you should not modify or free
the returned string.

## Version

This function is available since SDL 2.0.0.

## See Also

* [SDL_AudioInit](SDL_AudioInit)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction)

