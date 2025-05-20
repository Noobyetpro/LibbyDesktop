## 🛠️ How to Build the App (Using Electron Packager)

You can build LibbyDesktop for your platform using the following commands.

> 📁 `.` = source directory (current folder)  
> 📝 `LibbyDesktop` = output app name  
> 🎨 Make sure the correct icon file (`.ico`, `.icns`, `.png`) is in the root folder

---

### 🐧 Linux
```bash
npx electron-packager . LibbyDesktop --platform=linux --arch=x64 --icon=icon.png --overwrite
```

---

### 🍎 macOS
```bash
npx electron-packager . LibbyDesktop --platform=darwin --arch=x64 --icon=icon.icns --overwrite
```

---

### 🪟 Windows
```bash
npx electron-packager . LibbyDesktop --platform=win32 --arch=ia32 --icon=icon.ico --overwrite
```

> 💡 You can also use `--arch=x64` for 64-bit Windows builds

---

### ✅ Optional Flags
- `--asar` – bundle your app source into a single `.asar` file  
- `--prune=true` – remove dev dependencies from the final build  
- `--out=dist` – place all builds in a `dist/` folder

---

### 🚀 Running the App

After building, go into the output folder and run your app:

**Linux:**
```bash
./LibbyDesktop
```

**macOS:**
```bash
open LibbyDesktop.app
```

**Windows:**
```cmd
LibbyDesktop.exe
```
