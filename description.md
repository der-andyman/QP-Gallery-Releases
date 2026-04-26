Fix GIF playback and hidden visibility reset on Alpha 2

This update provides an Alpha 2 APK with two fixes tested on a Samsung Galaxy S25:

- GIF playback now works on modern 64-bit Android devices.
- Hidden albums/folders are hidden again after leaving the app with the system back button and reopening it.

Technical notes:

- GIF playback first tries Android's `ImageDecoder` / `AnimatedImageDrawable` path on Android 9+.
- The legacy QuickPic GIF decoder remains as fallback.
- The hidden visibility flag is reset when the gallery exits via the system back path.

Tested on:

- Samsung Galaxy S25
- 64-bit only device
