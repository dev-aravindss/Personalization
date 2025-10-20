Personalization Tools

This repository contains tools and scripts designed to introduce small, quality-of-life improvements to your system.

🚀 Windows Terminal Shortcut

This folder contains the AutoHotkey script (Windows Terminal Shortcut.ahk) to quickly launch the new Windows Terminal with a simple keyboard shortcut.

The Script (Windows Terminal Shortcut.ahk)

The script is simple and lightweight:

^!t::   ; Ctrl + Alt + T shortcut key
Run, wt ; Open Windows Terminal
return

This assigns the global shortcut Ctrl + Alt + T to execute the command wt, which is the alias for Windows Terminal.

🛠️ Prerequisites

To run the .ahk script, you must have AutoHotkey installed on your system.

[Download AutoHotkey](https://www.autohotkey.com/)

💻 How to Use and Add to Startup

Follow these steps to ensure the Windows Terminal shortcut is available every time you boot your computer.

Step 1: Place the Script

Download or clone this repository.

Place the Windows Terminal Shortcut.ahk file in a stable location on your computer where you won't accidentally delete it (e.g., in a dedicated C:\Scripts folder).

Step 2: Add to Windows Startup

We will use the Windows Startup Folder to automatically run the script when you log in.

Press Win + R to open the Run dialog.

Type shell:startup and press Enter. This will open the Startup folder in File Explorer.

Create a Shortcut to your .ahk file:

Navigate to where you saved the Windows Terminal Shortcut.ahk file.

Right-click the file and select Send to > Desktop (create shortcut).

Cut (Ctrl + X) the new shortcut from your desktop.

Paste (Ctrl + V) the shortcut into the Startup folder you opened in step 2.

The next time you log in, the script will automatically run in the background, enabling the Ctrl + Alt + T shortcut.

📦 Compiling the Script (Optional: For standalone use)

If you prefer to run the script without having AutoHotkey installed, you can convert the .ahk script into a standalone .exe using the Ahk2Exe utility that comes with AutoHotkey.

How to Compile

Ensure you have AutoHotkey installed.

Find and open the Ahk2Exe utility on your system (usually by searching the Start Menu for "Convert .ahk to .exe").

In the utility window:

Source: Select your Windows Terminal Shortcut.ahk file.

Destination: Choose the location and filename for your new .exe file (e.g., TerminalShortcut.exe).

Click Convert.

You can now use this compiled .exe file instead of the .ahk file for the Startup guide above.