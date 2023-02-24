====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_ResetAssertionReport =

Clear the list of all assertion failures.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_ResetAssertionReport(void);
</syntaxhighlight>

== Remarks ==

This function will clear the list of all assertions triggered up to that
point. Immediately following this call, [[SDL_GetAssertionReport]] will
return no items. In addition, any previously-triggered assertions will be
reset to a trigger_count of zero, and their always_ignore state will be
false.

== Version ==

This function is available since SDL 3.0.0.

== Code Examples ==

<syntaxhighlight lang='c++'>
SDL_assert(1+1 == 3);  // trigger an assertion.
printf("%p\n", SDL_GetAssertionReport());  // not NULL.
SDL_ResetAssertionReport();
printf("%p\n", SDL_GetAssertionReport());  // NULL.
</syntaxhighlight>

== Related Functions ==

:[[SDL_GetAssertionReport]]

----
[[CategoryAPI]], [[CategoryAssertions]]

