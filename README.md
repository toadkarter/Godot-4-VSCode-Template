# Godot 4 | VSCode Template

This repository contains the steps needed to enable debugging of Godot 4 projects with breakpoints in VSCode. I am largely using this to help myself remember what to do on future projects, but I'm making it public in case it helps others. 

The steps below are taken from this [GitHub issue](https://github.com/godotengine/godot-vscode-plugin/issues/389). It is assumed that you already have the [Godot VSCode Plugin](https://github.com/godotengine/godot-vscode-plugin/) installed. 

# Steps
## VSCode
1. Add `.vscode` to the `.gitignore` file of your project.
2. Copy the `.vscode` folder in this repository to the root of your project.

## Godot
1. In `Editor -> Editor Settings -> Text Editor -> External`, set `Use External Editor` to `On`, and point the path to your installed VSCode binary.
2. In `Editor -> Editor Settings -> Network -> Debug`, set the `Remote Port` value to `6007`.
3. In `Editor -> Editor Settings -> Network -> Debug Adapter` set the `Remote Port` value to `6008` and `Sync Breakpoints` to `On`.

With Godot Editor open, you should now be able to run the debug command in VSCode and hit breakpoints that you set throughout your code.  