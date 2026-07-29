# Better YouTube Shorts

## Added more features to YouTube shorts, including:

- Automatic jump to the corresponding video screen
- Manual jump to the corresponding video screen using the shortcut Alt + W, for example, [https://www.youtube.com/shorts/9wRiG-A7K8A](https://www.youtube.com/shorts/9wRiG-A7K8A), pressing Alt + W will open [https://www.youtube.com/watch?v=9wRiG-A7K8A](https://www.youtube.com/watch?v=9wRiG-A7K8A), opening the current short in the video screen
- Progress bar (including time display, draggable)
- Volume control (including volume display)
- Playback speed control
- Auto-scroll control

### Script Recommendation: [Tabview](https://www.youtube.com/shorts/9wRiG-A7K8A) [YouTube](https://greasyfork.org/zh-CN/scripts/428651-tabview-youtube), its biggest advantage is that you can watch videos and read comments simultaneously without scrolling back and forth, which is very convenient.

## Script Features

- <h3>Avoids performance issues caused by setInterval, uses requestAnimationFrame, and only renders the necessary parts, greatly reducing performance consumption</h3>

## Optimizations

- <h3>Solves the problem of ad-blocking plugins and extensions failing when they are present</h3>
- <h3>Optimizes loading speed</h3>
- <h3>Solves the problem of shorter links not loading into the Better YouTube Shorts interface when accessed from other pages (such as the user's homepage, the shorts section of the homepage, etc.)</h3>

## Script Options (in the Tampermonkey / ViolentMonkey menu)

### 1. Option "Shorts Auto Switch To Video"

- off: Do not automatically switch to the video interface
- on: Automatically switch to the video interface

### 2. Option "Loop Playback" (This option only takes effect after autoscroll is turned off; otherwise, autoscroll takes precedence)

- off: Stops playback after a video finishes.
- on: Automatically loops indefinitely after a video finishes playing.

### 3. Option "Continue From Last Checkpoint"

- off: Default logic for shorts; each short starts playing from 0 seconds.
- temporary: Remembers the last position of each short; when returning to the same short, it continues from the last position (this memory is reset every time the page refreshes).
- permanent: This memory is not reset when the page refreshes.

### 4. Option "Constant Volume"

- off: Uses YouTube's default volume logic for shorts; each video has its own volume.
- on: All viewed shorts use the volume set by the user on the volume bar.

### 5. Option "Constant Speed"

- off: Using YouTube's default playback speed logic for shorts, each video has its own playback speed.
- on: All viewed shorts use the playback speed set by the user on the playback speed bar.

### 6. Option "Open Watch In Current Tab" (This option is only effective when ShortsAutoSwitchToVideo is off, i.e., when the user is on the shorts screen)

- off: Opens the watch window for the current short in a new tab.
- on: Opens the watch window for the current short in the current tab.

### 7. Option "Double Click To Fullscreen"

- off: Disables double-click to fullscreen (to ensure compatibility with other plugins' double-click operations on shorts).
- on: Enables double-click to fullscreen.

### 8. Option "Progress Bar Style"

- original: Uses YouTube's native progress bar.
- custom: Uses a custom progress bar from Better YouTube Shorts.

### 9. Option "Operation Mode"

- Video (Keyboard shortcuts used in YouTube videos, plus Shift to scroll)
  - Up/Down Arrow - Volume down/up
  - Left/Right Arrow - Back/Forward
  - Shift + Left/Shift + Right - Previous/Next Video
  - Shift + Up/Shift + Down - Previous/Next Video
  - Space - Play/Pause
  - Double-tap Video - Full Screen
  - Alt + Enter (including Enter on the numeric keypad) - Full Screen
  - Alt + W - Open the short's video view
  - 0~9 (including the numeric keypad) - Jump to the corresponding progress
  - C - Speed ​​up playback
  - X - Slow down playback
  - Z - Restore playback speed
  - V - Show/hide short's description
- Shorts (Keyboard shortcuts used in YouTube Shorts, plus Shift to control volume)
  - Up/Down Arrow - Previous/Next Video
  - Left/Right Arrow - Back/Forward
  - Shift + Left/Shift + Right - Volume down/up
  - Shift+Down/Shift+Up - Volume down/up
  - Space - Play/Pause
  - Double-click the video - Full screen
  - Alt + Enter (including Enter on the numeric keypad) - Full screen
  - Alt + W - Open the video interface corresponding to the short
  - 0~9 (including the numeric keypad) - Jump to the corresponding progress
  - C - Speed ​​up playback
  - X - Slow down playback
  - Z - Restore playback speed
  - V - Show/hide the short description
