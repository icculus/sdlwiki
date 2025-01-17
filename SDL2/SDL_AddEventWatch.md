###### (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)
# SDL_AddEventWatch

Add a callback to be triggered when an event is added to the event queue.

## Header File

Defined in [SDL_events.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_events.h), but apps should _only_ `#include "SDL.h"`!

## Syntax

```c
void SDL_AddEventWatch(SDL_EventFilter filter,
                       void *userdata);

```

## Function Parameters

|                  |                                                                               |
| ---------------- | ----------------------------------------------------------------------------- |
| **filter**       | an [SDL_EventFilter](SDL_EventFilter) function to call when an event happens. |
| **userdata**     | a pointer that is passed to `filter`                                          |

## Remarks

`filter` will be called when an event happens, and its return value is
ignored.

**WARNING**: Be very careful of what you do in the event filter function,
as it may run in a different thread!

If the quit event is generated by a signal (e.g. SIGINT), it will bypass
the internal queue and be delivered to the watch callback immediately, and
arrive at the next event poll.

Note: the callback is called for events posted by the user through
[SDL_PushEvent](SDL_PushEvent)(), but not for disabled events, nor for
events by a filter callback set with
[SDL_SetEventFilter](SDL_SetEventFilter)(), nor for events posted by the
user through [SDL_PeepEvents](SDL_PeepEvents)().

## Version

This function is available since SDL 2.0.0.

## See Also

* [SDL_DelEventWatch](SDL_DelEventWatch)
* [SDL_SetEventFilter](SDL_SetEventFilter)


## Example

```c
int MyEventFunction(void *userdata, SDL_Event *event) {
    // Do things with userdata and event

    return 0; // Value will be ignored
}

// ...
SDL_AddEventWatch(MyEventFunction, NULL);

```

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction)

