# ide-key-bindings

Knowing your IDE keybindings is critical for productive coding. However, when working with multiple IDEs it can be challenging to remember differences in keybindings across IDEs. For this reason, I have spent some time organizing keybindings across the IDEs to be more consistent and perhaps easier to remember. 

Obviously, key maps are very subjective but maybe somebody other than me will find this repo to be useful.

Covered IDEs:

* `IntelliJ IDEA`
* `Visual Studio`
* `Visual Studio Code`
* `Notepad++`

This repository contains:

* a spreadsheet with a mapping from `actions` to `("IDE action name", "IDE action keybind")`,
* importable keybind settings files for IDEs,

## Importing

* `IntelliJ IDEA` - Use the "File > Manage IDE Settings > Import Settings" action to import the `exports/intellij.zip` file.

* `Visual Studio` - Use the "Tools > Import and Export Settings" action to import the `exports/visual_studio.vssettings` file.

* `Visual Studio Code` - Replace the content of your current `keybindings.json` with the content of the `exports/visual_studio_code.json` file.
  
  You can find the location of your current `keybindings.json` file by using the "Help > Show All Commands" action and searching for "Preferences: Open Keyboard Shortcuts (JSON)" command. Once opened, right-click on the tab of the file and choose "Copy Path".

* `Notepad++` - Replace the content of your current `shortcuts.xml` file with the content of the `exports/notepad++.xml`.

  On Windows, you can find the location of your current `shortcuts.xml` file by pressing `Win + R` and opening `%APPDATA%/Notepad++`.

## Action selection rationale

Different IDEs have different actions, GUIs, and action names making it a non-trivial task to "unify" key bindings. Sometimes actions simply differ by name, sometimes the GUI to accomplish the same task is very different, and sometimes there is just no equivalent.

The spreadsheet contains an arbitrary set of **generic actions** (IDE agnostic) that I have found useful in my daily work. I have made my best effort to map them to the most meaningful IDE-specific actions. However, there are generic actions that are simply not supported or not bindable in some IDEs in which case the spreadsheet contains a "FIXED" marker entry. Furthermore, some very sophisticated generic actions that are supported in only a single IDE have been generally (i.e. with exceptions) omitted.

## Keybindings rationale

The following are general rules I have tried to follow but some exceptions have been made.

* Frequently used actions (e.g. editing, navigating) should have a fast and convenient shortcut.
* Combinations with `Shift` should have an effect that is similar to or reverses the combination without shift.
* Combinations with `Ctrl+Alt` are for more advanced actions that work on the entire file or IDE.
* Combinations `Alt+<somekey>` are avoided because MS Windows uses them to select menu items and jump to dialog fields. Exceptions are made for `Alt+<number>` and `Alt+<arrowkey>`.
* IDE's side panels are opened by combinations with `Alt+<number>`, possibly with additional modifiers for logically similar panels.
