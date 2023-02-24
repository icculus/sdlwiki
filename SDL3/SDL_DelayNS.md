====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_DelayNS =

Wait a specified number of nanoseconds before returning.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_DelayNS(Uint64 ns);
</syntaxhighlight>

== Function Parameters ==

{|
|'''ns'''
|the number of nanoseconds to delay
|}

== Remarks ==

This function waits a specified number of nanoseconds before returning. It
waits at least the specified time, but possibly longer due to OS
scheduling.

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

