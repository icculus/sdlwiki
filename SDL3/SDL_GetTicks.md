====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetTicks =

Get the number of milliseconds since SDL library initialization.

== Syntax ==

<syntaxhighlight lang='c'>
Uint64 SDL_GetTicks(void);
</syntaxhighlight>

== Return Value ==

Returns an unsigned 64-bit value representing the number of milliseconds
since the SDL library initialized.

== Version ==

This function is available since SDL 3.0.0.

== Code Examples ==

<syntaxhighlight lang='c++'>
unsigned int lastTime = 0, currentTime;
while (!quit) {
  // do stuff
  // ...

  // Print a report once per second
  currentTime = SDL_GetTicks();
  if (currentTime > lastTime + 1000) {
    printf("Report: %d\n", variable);
    lastTime = currentTime;
  }
}
</syntaxhighlight>

----
[[CategoryAPI]], [[CategoryTimer]]

