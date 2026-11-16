# Nightshift Forge

A polished, context-aware Oh My Posh theme for developers and infrastructure engineers. Nightshift Forge pairs a deep navy interface with restrained teal, amber, and muted language colors. It contains no personal name or machine-specific path.

## What appears in the prompt

- The active `user@host`, an SSH glyph for remote sessions, current directory, and Git branch/status
- Language badges for Node.js, Python, Rust, Go, Java, .NET, PHP, and Ruby when Oh My Posh detects that language in the current project or environment
- Previous command duration, local time, and exit status

Language badges are contextual, so unrelated runtimes stay out of the prompt. Python also shows an active virtual environment when Oh My Posh detects one.

## Requirements

- A current version of [Oh My Posh](https://ohmyposh.dev/docs/installation/windows) (the theme uses configuration schema version 3)
- A [Nerd Font](https://ohmyposh.dev/docs/installation/fonts) enabled in your terminal for the icons

## Download

Download [nightshift-forge.omp.json](https://raw.githubusercontent.com/al-amin-khan/nightshift-forge/main/nightshift-forge.omp.json) and save it in the location used below.

## Install in PowerShell

Place `nightshift-forge.omp.json` in a stable location, for example `$HOME\.config\oh-my-posh\`, then add this line to your PowerShell profile:

```powershell
oh-my-posh init pwsh --config "$HOME\.config\oh-my-posh\nightshift-forge.omp.json" | Invoke-Expression
```

Reload the profile or open a new terminal window.

## Install in Bash or Zsh

```sh
eval "$(oh-my-posh init bash --config ~/.config/oh-my-posh/nightshift-forge.omp.json)"
```

For Zsh, replace `bash` with `zsh`.

## Customize

Edit the JSON theme to adjust the color values, icons, or the language segments. Oh My Posh only displays language segments when their configured project or environment context is detected.

## License

[MIT](LICENSE). Free to use, modify, and redistribute.



## SSH sessions

The badge displays the account and hostname of the machine running the shell. Over SSH, this is the remote login account and remote host. Install Oh My Posh and initialize this theme on the remote host as well; the local prompt does not configure remote shells.

## Preview

The design images shared during development are illustrative mockups. Actual glyphs are monochrome Nerd Font characters, and spacing depends on terminal width and font.
