====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_AndroidShowToast =

Shows an Android toast notification.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_AndroidShowToast(const char* message, int duration, int gravity, int xoffset, int yoffset);
</syntaxhighlight>

== Function Parameters ==

{|
|'''message'''
|text message to be shown
|-
|'''duration'''
|0=short, 1=long
|-
|'''gravity'''
|where the notification should appear on the screen.
|-
|'''xoffset'''
|set this parameter only when gravity >=0
|-
|'''yoffset'''
|set this parameter only when gravity >=0
|}

== Return Value ==

Returns 0 if success, -1 if any error occurs.

== Remarks ==

Toasts are a sort of lightweight notification that are unique to Android.

https://developer.android.com/guide/topics/ui/notifiers/toasts

Shows toast in UI thread.

For the <code>gravity</code> parameter, choose a value from here, or -1 if
you don't have a preference:

https://developer.android.com/reference/android/view/Gravity

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]], [[CategoryAndroid]]

