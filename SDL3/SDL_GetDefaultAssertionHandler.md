====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetDefaultAssertionHandler =

Get the default assertion handler.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_AssertionHandler SDL_GetDefaultAssertionHandler(void);
</syntaxhighlight>

== Return Value ==

Returns the default [[SDL_AssertionHandler]] that is called when an assert
triggers.

== Remarks ==

This returns the function pointer that is called by default when an
assertion is triggered. This is an internal function provided by SDL, that
is used for assertions when [[SDL_SetAssertionHandler]]() hasn't been used
to provide a different function.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetAssertionHandler]]

----
[[CategoryAPI]], [[CategoryAssertions]]
<!-- #See the Style Guide for instructions on editing the footer. -->

