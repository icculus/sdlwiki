====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_WaitEventTimeout =

Wait until the specified timeout (in milliseconds) for the next available event.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_WaitEventTimeout(SDL_Event * event,
                         int timeout);
</syntaxhighlight>

== Function Parameters ==

{|
|'''event'''
|the [[SDL_Event]] structure to be filled in with the next event from the queue, or NULL
|-
|'''timeout'''
|the maximum number of milliseconds to wait for the next available event
|}

== Return Value ==

Returns 1 on success or 0 if there was an error while waiting for events;
call [[SDL_GetError]]() for more information. This also returns 0 if the
timeout elapsed without an event arriving.

== Remarks ==

If <code>event</code> is not NULL, the next event is removed from the queue
and stored in the [[SDL_Event]] structure pointed to by <code>event</code>.

As this function may implicitly call [[SDL_PumpEvents]](), you can only
call this function in the thread that initialized the video subsystem.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_PollEvent]]
:[[SDL_PumpEvents]]
:[[SDL_WaitEvent]]

----
[[CategoryAPI]]

