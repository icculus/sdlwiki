====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_ConvertAudio =

Convert audio data to a desired audio format.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_ConvertAudio(SDL_AudioCVT * cvt);
</syntaxhighlight>

== Function Parameters ==

{|
|'''cvt'''
|an [[SDL_AudioCVT]] structure that was previously set up by [[SDL_BuildAudioCVT]]().
|}

== Return Value ==

Returns 0 if the conversion was completed successfully or a negative error
code on failure; call [[SDL_GetError]]() for more information.

== Remarks ==

This function does the actual audio data conversion, after the application
has called [[SDL_BuildAudioCVT]]() to prepare the conversion information
and then filled in the buffer details.

Once the application has initialized the <code>cvt</code> structure using
[[SDL_BuildAudioCVT]](), allocated an audio buffer and filled it with audio
data in the source format, this function will convert the buffer, in-place,
to the desired format.

The data conversion may go through several passes; any given pass may
possibly temporarily increase the size of the data. For example, SDL might
expand 16-bit data to 32 bits before resampling to a lower frequency,
shrinking the data size after having grown it briefly. Since the supplied
buffer will be both the source and destination, converting as necessary
in-place, the application must allocate a buffer that will fully contain
the data during its largest conversion pass. After [[SDL_BuildAudioCVT]]()
returns, the application should set the <code>cvt->len</code> field to the
size, in bytes, of the source data, and allocate a buffer that is
<code>cvt->len * cvt->len_mult</code> bytes long for the <code>buf</code>
field.

The source data should be copied into this buffer before the call to
[[SDL_ConvertAudio]](). Upon successful return, this buffer will contain
the converted audio, and <code>cvt->len_cvt</code> will be the size of the
converted data, in bytes. Any bytes in the buffer past
<code>cvt->len_cvt</code> are undefined once this function returns.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_BuildAudioCVT]]

----
[[CategoryAPI]]

