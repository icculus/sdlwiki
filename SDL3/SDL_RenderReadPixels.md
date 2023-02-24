====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_RenderReadPixels =

Read pixels from the current rendering target to an array of pixels.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_RenderReadPixels(SDL_Renderer *renderer,
                         const SDL_Rect *rect,
                         Uint32 format,
                         void *pixels, int pitch);
</syntaxhighlight>

== Function Parameters ==

{|
|'''renderer'''
|the rendering context
|-
|'''rect'''
|an [[SDL_Rect]] structure representing the area to read, or NULL for the entire render target
|-
|'''format'''
|an [[SDL_PixelFormatEnum]] value of the desired format of the pixel data, or 0 to use the format of the rendering target
|-
|'''pixels'''
|a pointer to the pixel data to copy into
|-
|'''pitch'''
|the pitch of the <code>pixels</code> parameter
|}

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Remarks ==

'''WARNING''': This is a very slow operation, and should not be used
frequently. If you're using this on the main rendering target, it should be
called after rendering and before [[SDL_RenderPresent]]().

<code>pitch</code> specifies the number of bytes between rows in the
destination <code>pixels</code> data. This allows you to write to a
subrectangle or have padded rows in the destination. Generally,
<code>pitch</code> should equal the number of pixels per row in the
<code>pixels</code> data times the number of bytes per pixel, but it might
contain additional padding (for example, 24bit RGB Windows Bitmap data pads
all rows to multiples of 4 bytes).

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]], [[CategoryRender]]

