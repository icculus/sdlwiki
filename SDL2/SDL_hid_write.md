###### (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)
# SDL_hid_write

Write an Output report to a HID device.

## Header File

Defined in [SDL_hidapi.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hidapi.h), but apps should _only_ `#include "SDL.h"`!

## Syntax

```c
int SDL_hid_write(SDL_hid_device *dev, const unsigned char *data, size_t length);

```

## Function Parameters

|                |                                                                  |
| -------------- | ---------------------------------------------------------------- |
| **dev**        | A device handle returned from [SDL_hid_open](SDL_hid_open)().    |
| **data**       | The data to send, including the report number as the first byte. |
| **length**     | The length in bytes of the data to send.                         |

## Return Value

Returns the actual number of bytes written and -1 on error.

## Remarks

The first byte of `data` must contain the Report ID. For devices which only
support a single report, this must be set to 0x0. The remaining bytes
contain the report data. Since the Report ID is mandatory, calls to
[SDL_hid_write](SDL_hid_write)() will always contain one more byte than the
report contains. For example, if a hid report is 16 bytes long, 17 bytes
must be passed to [SDL_hid_write](SDL_hid_write)(), the Report ID (or 0x0,
for devices with a single report), followed by the report data (16 bytes).
In this example, the length passed in would be 17.

[SDL_hid_write](SDL_hid_write)() will send the data on the first OUT
endpoint, if one exists. If it does not, it will send the data through the
Control Endpoint (Endpoint 0).

## Version

This function is available since SDL 2.0.18.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction)

