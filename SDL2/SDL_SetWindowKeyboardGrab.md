====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_SetWindowKeyboardGrab =

Set a window's keyboard grab mode.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_SetWindowKeyboardGrab(SDL_Window * window,
                               SDL_bool grabbed);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|The window for which the keyboard grab mode should be set.
|-
|'''grabbed'''
|This is [[SDL_TRUE]] to grab keyboard, and [[SDL_FALSE]] to release.
|}

== Remarks ==

Keyboard grab enables capture of system keyboard shortcuts like Alt+Tab or
the Meta/Super key. Note that not all system keyboard shortcuts can be
captured by applications (one example is Ctrl+Alt+Del on Windows).

This is primarily intended for specialized applications such as VNC clients
or VM frontends. Normal games should not use keyboard grab.

When keyboard grab is enabled, SDL will continue to handle Alt+Tab when the
window is full-screen to ensure the user is not trapped in your
application. If you have a custom keyboard shortcut to exit fullscreen
mode, you may suppress this behavior with
<code>[[SDL_HINT_ALLOW_ALT_TAB_WHILE_GRABBED]]</code>.

If the caller enables a grab while another window is currently grabbed, the
other window loses its grab in favor of the caller's window.

== Version ==

This function is available since SDL 2.0.16.

== Related Functions ==

:[[SDL_GetWindowKeyboardGrab]]
:[[SDL_SetWindowMouseGrab]]
:[[SDL_SetWindowGrab]]

----
[[CategoryAPI]]

