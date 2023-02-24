====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_iconv_string =

This function converts a string between encodings in one pass, returning a string that must be freed with [[SDL_free]]() or NULL on error.

== Syntax ==

<syntaxhighlight lang='c'>
char* SDL_iconv_string(const char *tocode,
                       const char *fromcode,
                       const char *inbuf,
                       size_t inbytesleft);
</syntaxhighlight>

== Version ==

This function is available since SDL 2.0.0.

----
[[CategoryAPI]]

