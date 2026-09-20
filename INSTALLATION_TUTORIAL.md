# Pixilart-Image-Importer
Import Images into Pixilart.com with this lite chrome extension !  It allows you to import any image into the pixel art editor of Pixilart.com in order to create more easily. 

# How to Install an Unpacked Chrome Extension in Developer Mode

Follow these steps to extract a ZIP file and load the folder as an unpacked extension in Google Chrome.

### 1. Download the ZIP file

Download the `pixilart Image Importer.zip` file to your computer.

### 2. Extract the ZIP file

Locate the `Pixilart Image Importer ZIP` file and extract it.

* **Windows:** Right-click the ZIP file → **Extract All...**
* **macOS:** Double-click the ZIP file.
* **Linux:** Right-click the ZIP file → **Extract Here** (or use your preferred archive manager).

After extracting it, you should have a normal folder containing the extension files.

**Important:** Make sure you select the folder that directly contains the extension's `manifest.json` file.

### 3. Open Chrome's Extensions page

Open Google Chrome and go to:

`chrome://extensions/`

You can also open the menu and go to **Extensions → Manage Extensions**.

### 4. Enable Developer Mode

On the Extensions page, find the **Developer mode** switch, usually located in the top-right corner, and turn it on.

### 5. Load the unpacked extension

Once Developer mode is enabled, click **Load unpacked**.

A file browser will appear. Navigate to the folder you extracted from the ZIP file.

Select the folder containing `manifest.json`, then click **Select Folder**.

### 6. Verify the extension

Chrome should now add the extension to your extensions list.

If the extension appears without errors, it has been successfully loaded as an **unpacked extension**.

### If Chrome shows an error

Make sure that:

* You selected the correct folder.
* The selected folder contains a `manifest.json` file.
* You did not select the original `.zip` file.
* You did not accidentally select a folder containing another folder that contains the actual extension files.

For example, the correct structure should be :

```text
Pixilart Image Importer/
├── manifest.json
├── background.js
├── content.js
├── popup.html
├── popup.js
└── icons/
    └── icon.png
```

In this example, you should select **`Pixilart Image Importer`**, not the `icons` folder and not a parent folder containing `Pixilart Image Importer`.

### Updating the extension

If you modify the extension's files while it is loaded, return to:

`chrome://extensions/`

and click the **Reload** button for the extension to apply the changes.
