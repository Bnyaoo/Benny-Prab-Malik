---
layout: default
title: Troubleshooting guide 
nav_order: 5
---

# Troubleshooting guide 

| **Symptoms** | **Probable Cause** | **Action** |
| ------------ | ------------------ | ---------- |
| PyCharm Editor restricts code editing. | You have installed the IdeaVim plugin and thus enabled the vim editing mode. | Deselect Vim Emulator on the Tools menu. See Using Vim Editor Emulation in PyCharm for more details |
|Python code is not highlighted in the Editor.| The PY files are associated with the text file format. | In the Settings/Preferences dialog (⌘ ,), navigate to Editor - File Types, select Text from the Recognized File Type list, select *.py from the File Name Patterns list, and click Remove.|
| A Python interpreter is marked as unsupported in the list of available interpreters in Preferences/Settings  - Project -  Python Interpreter. | The Python version of the marked interpreter is outdated and it is not supported in PyCharm | You can delete the unsupported interpreter from the list of the available interpreters. For more information about the supported Python versions, see Python Support.|
| Code completion action is not available. | Power Save Mode is enabled. | From the main menu, choose File and clear the Power Save Mode checkbox.|
| Unknown Scope error | The File Watcher uses a scope that is not defined in this project. | Double-click the watcher and select an available scope or create a new one. |
