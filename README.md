# MuseLink

Keep the music on your Android devices in step with a computer, over Wi-Fi. No cable and no account.

MuseLink has two parts: a small program on the computer that holds your music library, and an app on each Android device.

## Download

Downloads are published on the [Releases](../../releases) page:

- `MuseLink-Windows-x64.exe` for the computer (Windows 10 or 11, 64-bit)
- `MuseLink-Android.apk` for each device (Android 11 or newer)

The current version is [v0.6.0](../../releases/tag/v0.6.0), a pre-release: it passed its automated builds and tests, but has not yet been tried on a real Android device or through the Windows firewall.

## What it does

- Shows your MP3 and FLAC library by album, with covers, in a page on the computer.
- Sends the songs you choose to a device the next time that device syncs.
- Works with several devices. Each one has its own name and its own list of songs.
- Edits tags on the computer, for one song or for many at once, and brings the changes to your devices without downloading the songs again.
- Finds album covers online and stores them in the files.
- Plays your music, on the computer and on the devices.

## Set up

1. On the computer, run `MuseLink-Windows-x64.exe`. A page opens in your browser and asks for a name for the computer and for your music folder. If Windows asks whether MuseLink may use the network, allow it on private networks; otherwise your devices cannot reach it.
2. On each device, install `MuseLink-Android.apk`. The app asks for a name for the device, for access to its music files, and for the address of the computer. The address is shown in the Devices window on the computer and looks like `192.168.1.20:8765`.
3. On the computer, choose albums or songs and press **Send to device**. On the device, open **Sync** and press **Sync now**.

After you edit tags or covers on the computer, press **Sync metadata** on the device.

## Good to know

- The computer and the devices must be on the same network, and MuseLink must be running on the computer while a device syncs.
- There is no login. Any device on your network can reach the library while MuseLink is running, so use it on a network you trust.
- Windows and Android show a warning before the first run, because the files do not come from a store.
- The cover search needs internet. Everything else stays on your network.
- This repository holds the downloads only. The source code is not published here.
