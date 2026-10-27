# Mozilla Apps Themes

## Firefox — ThinkPad

`userChrome.css` theme: pure black chrome, TrackPoint red (`#e2231a`) accents, square corners everywhere.

- black toolbar, url bar, vertical tabs sidebar, menus and panels
- selected tab marked with a red bar (left for vertical tabs, top for horizontal)
- red focus ring on the url bar, red highlight in menus and url bar suggestions
- no rounded corners on the url bar, its inner buttons and the content area

Tested on Firefox 158 (Linux, vertical tabs). The theme relies on internal Firefox
variables and selectors, so a Firefox update may break parts of it.

### Install

1. Find your profile folder: `about:support` → *Profile Folder* → *Open Folder*.
2. Copy `firefox/userChrome.css` to `<profile>/chrome/userChrome.css`.
3. Copy `firefox/user.js` to `<profile>/user.js`
   (or set `toolkit.legacyUserProfileCustomizations.stylesheets = true` in `about:config`).
4. Restart Firefox.

Works best on top of the built-in *Dark* theme or the system theme in dark mode.

### Debugging

Enable `devtools.chrome.enabled` and `devtools.debugger.remote-enabled`, then open
the Browser Toolbox (`Ctrl+Alt+Shift+I`) to inspect the browser UI.
