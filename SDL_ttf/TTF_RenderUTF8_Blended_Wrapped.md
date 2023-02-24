====== (This function is part of SDL_ttf, a separate library from SDL.) ======
= TTF_RenderUTF8_Blended_Wrapped =

Render word-wrapped UTF-8 text at high quality to a new ARGB surface.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Surface * TTF_RenderUTF8_Blended_Wrapped(TTF_Font *font,
                const char *text, SDL_Color fg, Uint32 wrapLength);
</syntaxhighlight>

== Function Parameters ==

{|
|'''font'''
|the font to render with.
|-
|'''text'''
|text to render, in UTF-8 encoding.
|-
|'''fg'''
|the foreground color for the text.
|}

== Return Value ==

Returns a new 32-bit, ARGB surface, or NULL if there was an error.

== Remarks ==

This function will allocate a new 32-bit, ARGB surface, using alpha
blending to dither the font with the given color. This function returns the
new surface, or NULL if there was an error.

Text is wrapped to multiple lines on line endings and on word boundaries if
it extends beyond <code>wrapLength</code> in pixels.

If wrapLength is 0, this function will only wrap on newline characters.

You can render at other quality levels with
[[TTF_RenderUTF8_Solid_Wrapped]], [[TTF_RenderUTF8_Shaded_Wrapped]], and
[[TTF_RenderUTF8_LCD_Wrapped]].

== Version ==

This function is available since SDL_ttf 2.0.18.

== Related Functions ==

:[[TTF_RenderUTF8_Solid_Wrapped]]
:[[TTF_RenderUTF8_Shaded_Wrapped]]
:[[TTF_RenderUTF8_LCD_Wrapped]]

----
[[CategoryAPI]]

