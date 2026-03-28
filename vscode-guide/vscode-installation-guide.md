# Visual Studio Code Installation Guide for Windows

A step-by-step guide to downloading and installing Visual Studio Code (VSCode) on Windows, starting from scratch.

---

## Step 1: Open the VSCode Website

Open your web browser (Chrome, Firefox, Edge, etc.) and go to:

```
https://code.visualstudio.com
```

You will see the VSCode homepage. The page auto-detects your operating system and shows the appropriate download button. Since we want the Windows installer, we will go to the download page to pick the correct version.

Click the **"Download"** button in the top-right corner of the page.

![VSCode Homepage - Click the Download button in the top-right corner](screenshots/01-vscode-homepage.png)

---

## Step 2: Choose the Windows Installer

After clicking **Download**, you will be taken to the download page showing installers for all platforms: Windows, Linux, and Mac.

![VSCode Download Page - All platform options](screenshots/02-download-page.png)

Locate the **Windows** section on the left side of the page. It is highlighted below:

![Windows section highlighted on the download page](screenshots/03-windows-card-highlighted.png)

Click the blue **Windows** button to download the recommended **User Installer (x64)** for Windows 10 or 11.

![Windows download button close-up](screenshots/03-windows-download-button.png)

### Which installer type should you choose?

Below the main Windows button, you will see additional options:

| Installer Type | Description |
|---|---|
| **User Installer** (Recommended) | Installs for the current user only. No admin rights needed. |
| **System Installer** | Installs for all users on the machine. Requires administrator rights. |
| **.zip** | Portable version. No installation needed - just extract and run. |
| **CLI** | Command-line interface only. |

> **Tip:** If you are unsure, just click the main blue **Windows** button. It downloads the User Installer (x64), which works for the vast majority of Windows PCs.

> **Note:** If you have a Windows on ARM device (e.g. Surface Pro X, Snapdragon-based laptop), click the **Arm64** link next to "User Installer" instead.

---

## Step 3: Save the Installer

When you click the download button, your browser will prompt you to save the file.

- In **Firefox**: A download dialog appears. Click **Save File**.
- In **Chrome/Edge**: The download starts automatically and appears at the bottom of the browser window.

The file will be saved to your **Downloads** folder with a name like:

```
VSCodeUserSetup-x64-1.99.0.exe
```

Wait for the download to complete before proceeding.

---

## Step 4: Run the Installer

1. Open your **Downloads** folder in File Explorer, or click the completed download in your browser's download bar.
2. Double-click the file **`VSCodeUserSetup-x64-<version>.exe`** to launch the installer.
3. If Windows shows a **"Windows protected your PC"** SmartScreen warning:
   - Click **More info**
   - Then click **Run anyway**
4. If prompted by **User Account Control (UAC)**, click **Yes**.

---

## Step 5: Complete the Installation Wizard

The installer wizard will walk you through several screens:

### 5.1 License Agreement

- Read the license agreement
- Select **"I accept the agreement"**
- Click **Next**

### 5.2 Destination Location

- The default install location is fine for most users
- Click **Next**

### 5.3 Start Menu Folder

- Accept the default or customize the Start Menu folder name
- Click **Next**

### 5.4 Additional Tasks (Important!)

Check the boxes for the features you want. **Recommended selections:**

- [x] **Add "Open with Code" action to Windows Explorer file context menu** - Right-click any file to open it in VSCode
- [x] **Add "Open with Code" action to Windows Explorer directory context menu** - Right-click any folder to open it in VSCode
- [x] **Register Code as an editor for supported file types** - Associate common file types with VSCode
- [x] **Add to PATH** - Allows you to run `code` from the command line to open VSCode

> **Important:** Make sure **"Add to PATH"** is checked. This lets you open VSCode from any terminal by simply typing `code`.

### 5.5 Install

- Review your selections and click **Install**
- Wait for the installation to complete (usually takes less than a minute)

### 5.6 Finish

- Check **"Launch Visual Studio Code"** if you want to open it immediately
- Click **Finish**

---

## Step 6: Verify the Installation

After installation, VSCode will launch and show the **Welcome** tab. You can also verify it works by:

1. **From the Start Menu**: Search for **"Visual Studio Code"** and click to open it.

2. **From the Command Line**: Open Command Prompt or PowerShell and run:

```
code --version
```

If installed correctly, this will print the version number, e.g.:

```
1.99.0
<commit-hash>
x64
```

---

## Next Steps

The official VSCode documentation provides a comprehensive guide for getting started on Windows:

![VSCode Windows Documentation - Getting started steps](screenshots/05-windows-install-docs.png)

After installation, consider these next steps:

1. **Install Git** - Required for version control. Download from [git-scm.com](https://git-scm.com/).
2. **Install extensions** - Open the Extensions panel (`Ctrl+Shift+X`) and search for extensions for your programming language.
3. **Enable GitHub Copilot** - AI-powered code completion (free tier available with a GitHub account).
4. **Follow the Getting Started tutorial** - Available from the Welcome tab in VSCode.

For the full Windows setup guide, visit: https://code.visualstudio.com/docs/setup/windows

---

## Troubleshooting

| Issue | Solution |
|---|---|
| Download doesn't start | Right-click the download button and select "Save Link As..." |
| Installer blocked by antivirus | Temporarily disable your antivirus or add an exception for the installer |
| "Windows protected your PC" SmartScreen warning | Click **More info**, then **Run anyway** |
| `code` command not found in terminal | Restart your terminal after installation. If still not working, re-run the installer and make sure **"Add to PATH"** is checked. |
| VSCode won't launch after install | Try restarting your computer, then launch from the Start Menu |

---

*Guide created on 2026-03-28. Screenshots captured from Firefox browser on the official VSCode website (code.visualstudio.com).*
