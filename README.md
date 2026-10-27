# FPS Meter

A small overlay that sits on top of the game. No frame, and it does not steal focus. It shows the FPS of the app in front, not a hard-coded list of titles.

CPU and GPU load are optional. Turn them on in settings if you want them.

## What it does

- FPS comes from PresentMon, for the process that owns the foreground window.
- You can switch the counter: presented frames, frames that reached the display, the whole desktop, or one window.
- Clicks go through to the game until you point at the overlay.
- Drag it by the FPS number. Opacity, size, dark theme, snap to screen edges.
- Language is Russian or English. If you have not picked one, it follows the Windows UI language.
- Mic button: mute every active microphone, or put the old levels back.
- Pin programs on the overlay. Click starts the app, or brings its window forward if it is already open. You can set process priority.
- Autostart is a logon task, if you turn it on in settings.
- When a newer build is on GitHub, the widget downloads it on its own.

Windows asks for administrator rights once. PresentMon needs ETW to read frame times.

## Install

1. Get `fps_meter_i.exe` from [Releases](https://github.com/aakraykov-maker/fps-meter-app/releases).
2. Run it. It downloads the zip, checks it, unpacks the files, and puts a shortcut on the desktop.
3. After that, updates arrive when the widget starts.

The zip only has `FpsMeter.exe`, `PresentMon.exe`, `fps.ico`, and `Start.bat`.

PresentMon is Intel's tool, not this overlay. See [THIRD-PARTY](THIRD-PARTY.md).
