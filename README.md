# ide-key-bindings

Knowing your IDE keybindings is critical for productive coding. However, when working with multiple IDEs it can be challenging to remember differences in keybindings across IDEs. For this reason I have spent some time to organize keybindings across the IDEs to be more consistent and perhaps easier to remember. 

Obviously, key maps are very subjective but maybe somebody other than me will find this repo to be useful.

Covered IDEs:

* `IntelliJ IDEA`
* `Visual Studio`
* `Visual Studio Code`
* `Notepad++`

This repository contains:

* a spreadsheet with a mapping from `actions` to `("IDE action name", "IDE action keybind")`,
* importable keybind settings files for IDEs,

## Action selection

Different IDEs have different actions, GUIs and action names making it a non-trivial task to "unify" key bindings. Sometimes actions simply differ by name, sometimes the GUI to accomplish the same task is very different, and sometimes there is just no equivalent.

The spreadsheet contains an arbitrary set of **generic actions** (IDE agnostic) that I have found useful in my daily work. I have made my best effort to map them to the most meaningful IDE specific actions. However, there are generic actions that are simply not supported or not bindable in some IDEs in which case the spreadsheet contains a "FIXED" marker entry. Furthermore, some very sophisticated generic actions that are supported in only a single IDE have been generally (i.e. with exceptions) omitted.
