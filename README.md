# Keyboard Shortcuts for VS Code in Linux for humans more familiar with VS Code in Windows
---

### aka, "unfortunately, yes, they're different."

#### Part two of my on-going text-editor keybinding series:

#### "Change is hard! For the love of god, make it stop!"

[part one](https://github.com/averyfreeman/vscode-keybindings-for-sublime)

We're staunch.  We're recalcitrant.  We are *totally* averse to change.  After all, we're only human.  

If your muscle memory has been deeply impacted by learning VS Code in Windows, fear not, you can switch to Linux and benefit from all its development environments provide without having to throw out countless months of threadbare kinetic familiarity.

**Purpose of this repo:** Currently, this repo is only meant for introducing keybindings to VS Code in Linux to make it feel more like using VS Code in Windows.  If you have more *default* keybindings you'd like to add, I'd rather you open an issue or PR so we can keep them all in one place.

Please fork if you intend to change the purpose of the repo.

It only makes sense to use these keybindings if you're using VS Code for Linux.  This file won't do much in VS Code for Windows, as it *emulates* the VS Code Windows defaults.

In Mac OS it'll have unpredictable effects, as it has not yet been tested, but feel free to try it and open an issue or PR with your findings. We could always add another file for Mac OS users, or create another repo.

**Tested/Developed:** `KDE Plasma v5.23.4 on Arch Linux X11`

Just copy the `keybindings.json` from this repo into your Linux VS Code `keybindings.json` file.  

**The easiest way to do this is:**

 - Open VS Code in your Linux environment
 - hit `ctrl+shift+p` and search for `Preferences: Keyboard Shortcuts (JSON)` (*not* `default` - this file is read-only)
 - Open this file and have it ready to receive new keybindings (you may want to cordon off any old modifications you have made with some empty lines, as to not overwrite them by accident)
 - Come back to this repo in your browser
 - Click on `keybindings.json` in the repo's list of files (above this `README.md`)
 - Click on `Raw` at the top right
 - Hit `ctrl+a` to select all the shortcuts in `keybindings.json`
 - and `ctrl+c` to copy them to your clipboard, then
 - `ctrl+v` to paste them 
 - Note: When you paste them in, make sure the `{ . . . }` curly braces are *inside* the `[ . . . ]` square brackets, and there is a `,` comma after every set of curly braces until the very last one, where there should be no comma, or it will give you an error (the file must adhere to `.json` file structure)

### Further Troubleshooting:
---

If any of these shortcuts don't start working right away after saving `keybindings.json` inside VS Code (`ctrl+s` while it's open), the first thing to check for is a conflict with your Desktop Environment. 

In KDE, for example, these are in `System Settings` under `Shortcuts`:

 - Click on `Application Launcher` (typically bottom left corner like the `Start Menu`)
 - Open `System Settings` 
 - Open `Shortcuts` 
 - Check for conflicts by searching for key combinations

Generally speaking, keyboard shortcuts are described in order from left to right, with a `+` sign as the separator, and no ` ` spaces.

**Example:** On my default installation of KDE, `ctrl+alt+up` and `ctrl+alt+down` were already mapped to `Open All Windows` and `Show Desktop`, respectively.  I remapped these to `ctrl+meta+up` and `ctrl+meta+down` so the system would even further follow the Windows standard.  

**Hint:** If you're confused by this `meta` key thing, it's *linux-speak* for your **Windows key**.

If you're still having issues after that, try searching [Stack Overflow](https://stackoverflow.com) or Googling for your specific problem.  

If you think it's an issue with the way the shortcut is written, please [open an issue](https://github.com/averyfreeman/vscode-windows-keybindings-for-linux-users/issues)

