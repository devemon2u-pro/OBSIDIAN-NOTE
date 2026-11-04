# Offline Learning Website Builder — Obsidian Plugin

Export your Obsidian notes as a full offline HTML website.

---

## 🚀 Build the Plugin

### Prerequisites
- [Node.js](https://nodejs.org/) (v16 or higher)
- npm (comes with Node.js)

### Steps

1. **Extract the zip**
   - Unzip `Offline-Learning-Website-Builder.zip` into a folder

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Build the plugin**
   ```bash
   npm run build
   ```

4. After building, you will get **3 files** in the output folder:
   - `main.js`
   - `styles.css`
   - `manifest.json`

---

## 🗂️ Install into Obsidian

1. **Open Obsidian** and locate your vault folder using **File Browser**

2. **Navigate to your vault folder** — this is the root folder you opened in Obsidian

3. **Find the `.obsidian` folder**
   - It may be hidden. If you can't see it:
     - **Windows**: Open File Explorer → View → check **Hidden items**
     - **Mac**: Press `Cmd + Shift + .` to toggle hidden files

4. **Open the `.obsidian/plugins/` folder**
   - If `plugins` folder doesn't exist, create it manually

5. **Create a new folder** inside `plugins/` — name it something like:
   ```
   offline-learning-website-builder
   ```

6. **Paste the 3 built files** into that folder:
   ```
   .obsidian/
   └── plugins/
       └── offline-learning-website-builder/
           ├── main.js
           ├── styles.css
           └── manifest.json
   ```

7. **Open Obsidian**
   - Go to **Settings** → **Community plugins**
   - Toggle off **Restricted mode** if prompted
   - Find **Offline Learning Website Builder** in the list
   - Enable it ✅

8. You will now see an **Export to HTML** option in Obsidian — use it to export your notes as an offline website!

---

## 📁 File Structure

```
Offline-Learning-Website-Builder.zip
├── src/           # Plugin source code
├── package.json   # npm config
├── manifest.json  # Obsidian plugin manifest
└── ...
```

---

## 💡 Tips

- Make sure **Community plugins** are enabled in Obsidian settings
- The exported HTML files work fully offline — no internet needed
- You can open the exported `index.html` in any browser
