# App launcher icon

`flutter_launcher_icons` needs a **PNG** at `app_icon.png` (it does not use SVG). You have `app_icon.svg` — convert it to PNG first.

## Option A: Online (fast)

1. Open **https://cloudconvert.com/svg-to-png**
2. Upload **`assets/icon/app_icon.svg`**
3. Set dimensions **1024** × **1024**
4. Convert and **download**
5. Save the file as **`assets/icon/app_icon.png`**

## Option B: Command line (if you have Node.js)

```bash
npx --yes svg-render assets/icon/app_icon.svg assets/icon/app_icon.png --width 1024 --height 1024
```

## Then generate launcher icons

From project root:

```bash
dart run flutter_launcher_icons
```

Then rebuild/reinstall the app to see the new icon.
