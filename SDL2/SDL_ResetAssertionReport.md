====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
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

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GetAssertionReport]]

----
[[CategoryAPI]]

