# Bluetooth Speaker KeepAlive for Windows

A lightweight Windows tool to stop Bluetooth speakers from sleeping, turning off, or disconnecting when idle using a silent audio keep-alive.

Created by **Md. Mamun**  
GitHub: **https://github.com/MamunKhan71**

---

## Download

Download the latest version from the **Releases** page:

**[Download Latest Release](../../releases/latest)**

Download this file:

```text
BluetoothKeepAlive_Setup.exe
```

Then double-click it to install.

---

## Why this tool exists

Many Bluetooth speakers automatically go to sleep or disconnect when there is no audio playing.

This can be annoying when you are using a Bluetooth speaker with Windows and it keeps turning off after a short idle time.

**Bluetooth Speaker KeepAlive for Windows** helps prevent that by playing a tiny silent audio stream in the background. The speaker stays active, but you should not hear anything.

---

## Features

- Keeps Bluetooth speakers awake
- Helps prevent auto-disconnect
- Silent by default
- Lightweight Windows tool
- Simple `.exe` installer
- No admin permission required
- Auto-starts after Windows login
- User can choose ping interval
- User can choose ping length
- Includes silent and near-silent modes
- Includes status checker
- Easy uninstall option

---

## Quick Install

1. Download `BluetoothKeepAlive_Setup.exe` from the latest release.
2. Double-click `BluetoothKeepAlive_Setup.exe`.
3. Choose:

```text
1) Install / Update
```

4. Use the recommended settings:

```text
Ping interval: 30
Ping length: 2
Audio mode: 1
```

5. Done.

The app will start in the background and will also run automatically when you log in to Windows.

---

## Recommended Settings

For most Bluetooth speakers, use:

```text
Ping interval: 30 seconds
Ping length: 2 seconds
Audio mode: True silent
```

These settings are recommended for speakers that disconnect after about 1 minute of silence.

---

## What is Ping Interval?

The ping interval is how often the app sends a silent audio signal.

Example:

```text
30 seconds
```

This means the app plays a silent audio stream every 30 seconds.

---

## What is Ping Length?

The ping length is how long the silent audio stream lasts.

Example:

```text
2 seconds
```

This means the silent audio stream plays for 2 seconds each time.

---

## Audio Modes

### 1. True Silent

This is the recommended mode.

It plays digital silence, so you should not hear anything.

### 2. Near-Silent Fallback

Use this only if true silent mode does not keep your speaker awake.

Near-silent mode creates an extremely quiet signal. It is designed to be almost inaudible, but some speakers may react better to it than complete digital silence.

---

## How to Check If It Is Running

Run `BluetoothKeepAlive_Setup.exe` again and choose:

```text
2) Check status
```

The setup tool will show whether the background keep-alive process is running.

---

## Installed Location

The app installs to:

```text
%LOCALAPPDATA%\BluetoothKeepAlive
```

Installed files include:

```text
BluetoothKeepAlive.ps1
keepalive.wav
config.txt
keepalive.log
CREDIT.txt
```

---

## Auto-Start

Bluetooth Speaker KeepAlive adds a startup entry for the current Windows user.

It uses:

```text
HKCU\Software\Microsoft\Windows\CurrentVersion\Run
```

This means:

- No admin permission is required
- It starts after you log in to Windows
- It does not run before login

---

## Uninstall

Run `BluetoothKeepAlive_Setup.exe` again and choose:

```text
4) Uninstall
```

This will stop the background process and remove the installed files.

---

## Troubleshooting

### My speaker still turns off

Try installing again with a shorter interval:

```text
Ping interval: 15
Ping length: 2
Audio mode: 1
```

If that still does not work, try near-silent mode:

```text
Ping interval: 15
Ping length: 2
Audio mode: 2
```

---

### I hear a sound

Use true silent mode:

```text
Audio mode: 1
```

Also make sure Windows audio enhancements are disabled for your speaker.

---

### It is running, but my speaker still disconnects

Make sure your Bluetooth speaker is selected as the Windows output device:

```text
Settings → System → Sound → Output
```

Then choose your Bluetooth speaker.

---

### It does not start after reboot

Run the setup again and choose:

```text
1) Install / Update
```

Then check status:

```text
2) Check status
```

---

### Windows SmartScreen warning appears

Windows may show a warning because this is an unsigned custom app.

You may need to click:

```text
More info → Run anyway
```

Only do this if you downloaded the file from this GitHub repository.

---

## Who Should Use This?

This tool may help if your Bluetooth speaker:

- Turns off when no music is playing
- Disconnects after a short time of silence
- Sleeps too quickly
- Needs audio activity to stay connected
- Keeps disconnecting from Windows
- Requires a silent keep-alive signal

It may work with many Bluetooth speaker brands.

---

## Privacy

Bluetooth Speaker KeepAlive does not collect data.

It only creates local files on your computer and plays a local silent WAV file through your selected Windows audio output device.

---

## SEO Keywords

Bluetooth speaker keep alive, Bluetooth speaker auto disconnect fix, Windows Bluetooth speaker sleep fix, stop Bluetooth speaker from turning off, Bluetooth audio keep alive, silent audio ping, speaker standby fix, Bluetooth speaker disconnects when idle, Windows Bluetooth audio workaround, Bluetooth speaker idle disconnect fix.

---

## Credits

Created by **Md. Mamun**

GitHub: **https://github.com/MamunKhan71**

If this tool helped you, please consider giving this repository a ⭐ star.

---

## License

This project is licensed under the MIT License.

See the [LICENSE](LICENSE) file for details.
