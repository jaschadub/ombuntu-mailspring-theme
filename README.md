# Ombuntu Tokyo Night for Mailspring

A dark [Mailspring](https://getmailspring.com) theme matching Tokyo Night, the
default theme of the [Ombuntu](https://github.com/Ombuntu/Ombuntu) desktop.
Colors come from Omarchy's `themes/tokyo-night/colors.toml`: background
`#1a1b26`, text `#a9b1d6`, accent `#7aa2f7`.

It is Mailspring's built-in Dark theme recolored, so email bodies, icons and
labels are handled the same way as there.

## Install

In Mailspring, choose **Install New Theme...** and select this directory, then
pick **Ombuntu Tokyo Night** under Preferences, Appearance.

Or copy it into Mailspring's packages directory and restart Mailspring:

| Install      | Packages directory                         |
|--------------|--------------------------------------------|
| Snap         | `~/snap/mailspring/common/packages/`       |
| deb / native | `~/.config/Mailspring/packages/`           |

## Changing it

All colors are in `styles/ui-variables.less`; the `@tn-*` palette at the top
feeds everything else. `styles/index.less` holds the few rules variables cannot
reach. After an edit, reload from Developer Tools (Developer > Toggle Developer
Tools):

```
AppEnv.themes.setActiveTheme('ui-light');
AppEnv.themes.setActiveTheme('ombuntu-mailspring-theme');
```

Based on the [Mailspring Theme Starter](https://github.com/Foundry376/Mailspring-Theme-Starter).
