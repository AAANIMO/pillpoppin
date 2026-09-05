# Install

Download the latest build from the
[Releases](https://github.com/AAANIMO/pillpoppin/releases/latest) page.

| Platform | File |
|----------|------|
| macOS (Apple Silicon — M1/M2/M3/M4) | `Pillpoppin-arm64.dmg` |
| macOS (Intel) | `Pillpoppin-x64.dmg` |
| Windows | `Pillpoppin-x64.exe` |

Not sure which Mac you have? Apple menu →  **About This Mac**. "Apple M…" = arm64,
"Intel" = x64.

## macOS

1. Open the `.dmg` and drag **Pillpoppin** into Applications.
2. The app is **unsigned**, so the first launch needs a manual OK:
   - Right-click the app → **Open** → **Open**, or
   - System Settings → **Privacy & Security** → *Open Anyway*.
3. After the first launch it opens normally.

## Windows

1. Run `Pillpoppin-x64.exe`.
2. Windows SmartScreen may warn about an unknown publisher (the app is unsigned):
   click **More info → Run anyway**.
3. Follow the installer.

## Build it yourself

```bash
git clone https://github.com/AAANIMO/pillpoppin.git
cd pillpoppin
npm install
npm start          # run
npm run dist:mac   # or dist:win
```
