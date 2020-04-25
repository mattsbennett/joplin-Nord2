# joplin-Nord2

A sub-theme of [Joplin](https://joplinapp.org/)'s built-in `Nord` theme.

## Screenshot

![Nord2.png](/img/Nord2.png)

## Setup

`Nord2` is a sub-theme intended for use alongside the `Nord` theme built into Joplin.

### 1. Install fonts (optional)

`Nord2` requires a `sans-serif` and `monospace` system font. It will work just fine with system defaults, or your own preferred fonts however, it will default to using the following fonts, if installed on your system:

#### `sans-serif` (one of the following in priority order)

* `SF Pro Text`
  * `macOS` system font available [from Apple](https://developer.apple.com/fonts/) for macOS users (and Windows/Linux with a bit of work) as part of the "SF Pro" Family.

* `Roboto`
  * Open source font easily available for any platform from [Google Fonts](https://fonts.google.com/specimen/Roboto).

#### `monospace`

* `Fira Code`
  * Open source monospace font with software-development-centric ligatures available [on Github](https://github.com/tonsky/FiraCode).

> Note that you can also easily modify the theme to use your preferred `sans-serif` and `monospace` fonts installed on your system by making appropriate changes to the following lines of [userchrome.css](/src/userchrome.css) and [userstyle.css](/src/userstyle.css):

```CSS
:root {
    ...
    --font-sans: "SF Pro Text", "Roboto", sans-serif;
    --font-mono: "Fira Code", monospace;
    ...
}
```

### 2. Install theme

* Go to `Joplin > Preferences`.
* Click `Appearance`.
* Select `Nord` from the "Theme" dropdown.
* Select your preferred "Editor font size." `13` works well for me.
* Click `Show Advanced Settings`.
* Click `Edit` for "Custom stylesheet for rendered Markdown." The CSS file will open in your configured editor (or system default). Paste the CSS from [userstyle.css](/src/userstyle.css) and save the file.
* Repeat for "Custom stylesheet for Joplin-wide app styles," pasting and saving the CSS from [userchrome.css](/src/userchrome.css).
* Close and reopen Joplin to apply the changes.

> To remove the theme, just repeat the above process, but delete the contents of the opened files, save them, and reopen Joplin.
