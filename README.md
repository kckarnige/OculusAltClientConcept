<br>
<h3 align="center"></h3>
<p align="center">
    <img alt="iCon" src="./oculusdummy-banner-readme.png" width="500px">
</p>
<br>

## Reasons to use Oculus Dummy

- When you use Link, the Oculus Client opens whether you like it or not, Oculus Dummy makes it a little less annoying, running as a tray application in the background.

- The Oculus Client runs on Electron, meaning _**ALL**_ UI uses system resources, even if it's the 1,000th time you've opened a page.

- The Oculus Client uses system resources that could be use for more important things:
    - It uses your GPU for a bit on startup.
        - This is more of a nitpick than anything impactful if I'll be honest, especially if you have an iGPU and have it set to use that anyway.
    - Sometimes it randomly decides to use your CPU.
        - This is just stupid, especially if you're playing a CPU intensive game like BaS or Bonelab.
    - It can use an average of 200mb of memory, even in the damn settings menu.
        - Personally, I've seen it use as low as 158mb, up to 267mb of memory.
- The Oculus Client, *with Oculus Dummy installed*, loads faster, doesn't randomly use your CPU or GPU power, and uses around 20mb of memory when idle.

## Installation

1. Open your file explorer and go to `C:\Program Files\Oculus\Support\oculus-client\resources`.

2. Rename the `app.asar` file to something else, I prefer "`app.asar.bak`" for clarity, though it doesn't matter.

3. Download [this](https://github.com/kckarnige/OculusDummy/releases/latest/download/app.asar), and move it to the same folder.

4. Enjoy the extra bit of performance! 😊

## Uninstallation

1. Open your file explorer and go to `C:\Program Files\Oculus\Support\oculus-client\resources`.

2. Delete the `app.asar` file.

3. Rename your backup file (`app.asar.bak`) back to "`app.asar`".

4. Make sure to give Oculus Dummy a kiss before you leave it, it still loves you! 😔💕

## Building from source (Windows Only)

1. Clone the repository, I prefer using GitHub Desktop to make things easier.

2. Open the directory in your terminal and run `pnpm i` or `npm i`.

3. Run `pnpm build` or `npm run build` and wait.

4. The result should be located in the `dist` folder, the built `app.asar` inside should work just like any other release build.
