====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_RenderGeometry =

Render a list of triangles, optionally using a texture and indices into the vertex array Color and alpha modulation is done per vertex ([[SDL_SetTextureColorMod]] and [[SDL_SetTextureAlphaMod]] are ignored).

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_RenderGeometry(SDL_Renderer *renderer,
                       SDL_Texture *texture,
                       const SDL_Vertex *vertices, int num_vertices,
                       const int *indices, int num_indices);
</syntaxhighlight>

== Function Parameters ==

{|
|'''renderer'''
|The rendering context.
|-
|'''texture'''
|(optional) The SDL texture to use.
|-
|'''vertices'''
|Vertices.
|-
|'''num_vertices'''
|Number of vertices.
|-
|'''indices'''
|(optional) An array of integer indices into the 'vertices' array, if NULL all vertices will be rendered in sequential order.
|-
|'''num_indices'''
|Number of indices.
|}

== Return Value ==

Return 0 on success, or -1 if the operation is not supported

== Version ==

This function is available since SDL 2.0.18.

== Related Functions ==

:[[SDL_RenderGeometryRaw]]
:[[SDL_Vertex]]

----
[[CategoryAPI]]

