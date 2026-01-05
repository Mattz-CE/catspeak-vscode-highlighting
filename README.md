# 🐱 Catspeak Language - VS Code Extension

Syntax highlighting for **Catspeak** (`.meow` files) — the cross-platform modding language for GameMaker games.

Based on [Catspeak](https://github.com/katsaii/catspeak-lang) by Katsaii.

![Example](example.png)

## Features

- ✅ Keywords: `let`, `fun`, `if`, `else`, `while`, `for`, `return`, `break`, `continue`
- ✅ Comments: `--` and `//` line comments
- ✅ Strings: `"..."`, `'...'`, and verbatim `@'...'`
- ✅ Numbers: integers, floats, hex, binary, underscores (`1_000_000`)
- ✅ Logical operators: `and`, `or`, `not`
- ✅ Constants: `true`, `false`, `undefined`, `Pusto`
- ✅ Special variables: `self`, `global`
- ✅ Built-in GameMaker & STONKS-9800 mod functions

## Installation

### From VSIX

1. Download the `.vsix` from [Releases](https://github.com/matt-wai/catspeak-vscode-highlighting/releases)
2. In VS Code/Cursor: Extensions → `...` → **Install from VSIX**

### Manual

Copy this folder to your extensions directory:
- **Windows**: `%USERPROFILE%\.vscode\extensions\catspeak-language`
- **macOS/Linux**: `~/.vscode/extensions/catspeak-language`

## Example

```catspeak
-- Daily bonus mod
let mod = {
  name: "Daily Bonus",
  description: "Gives money every day",

  new_day: fun () {
    if global.money < 1_000_000 {
      global.money += 500_000
      mods_notify("Bonus!", "Here's some cash")
    }
  }
}

return mod
```

## Games Using Catspeak

- [STONKS-9800](https://store.steampowered.com/app/1539140/STONKS9800_Stock_Market_Simulator/)
- [Rusted Moss](https://store.steampowered.com/app/1772830/Rusted_Moss/)
- [Picayune Dreams](https://store.steampowered.com/app/2340350/Picayune_Dreams/)
- [ZERO Sievert](https://store.steampowered.com/app/1782120/ZERO_Sievert/)

## License

MIT
