# Cyberpunk Themes for Atuin

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![Atuin](https://img.shields.io/badge/Atuin-%3E%3D18.4-cyan)](https://atuin.sh)

A collection of neon-drenched, futuristic color themes for [Atuin](https://atuin.sh) - the magical shell history tool.

## 🎨 Themes

### 🌃 Cyberpunk (Main)
Multi-color neon theme with a vibrant cyberpunk aesthetic featuring cyan, magenta, green, pink, and blue accents.

**Color Palette:**
- Base text: Neon Cyan
- Titles: Neon Magenta
- Important items: Neon Green
- Guidance/Help: Neon Pink
- Info alerts: Neon Blue

### 🟢 Cyberpunk Matrix
Matrix-inspired monochrome green theme for that authentic hacker feel.

**Color Palette:**
- Base text: Bright Green
- Everything: Various shades of green
- Standout items: Yellow accents

### 💖 Cyberpunk Vaporwave
Hot pink and cyan aesthetic with vaporwave vibes.

**Color Palette:**
- Base text: Hot Pink
- Guidance: Cyan
- Standout items: Yellow accents

## 📦 Installation

### Prerequisites
- [Atuin](https://atuin.sh) >= 18.4
- A terminal that supports 256 colors

### Quick Install

1. **Create the themes directory** (if it doesn't exist):
   ```bash
   mkdir -p ~/.config/atuin/themes
   ```

2. **Download the theme files**:
   ```bash
   cd ~/.config/atuin/themes
   
   # Download all three themes
   curl -O https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_REPO/main/cyberpunk.toml
   curl -O https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_REPO/main/cyberpunk-matrix.toml
   curl -O https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_REPO/main/cyberpunk-vaporwave.toml
   ```

3. **Enable a theme** by adding to `~/.config/atuin/config.toml`:
   ```toml
   [theme]
   name = "cyberpunk"
   ```
   
   Or choose a variant:
   - `name = "cyberpunk-matrix"`
   - `name = "cyberpunk-vaporwave"`

4. **Reload your shell**:
   ```bash
   source ~/.zshrc  # or ~/.bashrc for bash
   ```

5. **Test it out** by pressing `Ctrl+R` to open Atuin!

## 🎯 Usage

Once installed, the theme will automatically style your Atuin interface. Use Atuin as normal:

- `Ctrl+R` - Search shell history
- `Up Arrow` - Previous command (if configured)
- All the usual Atuin features with cyberpunk style!

## 🎨 Customization

Want to create your own variant? Copy one of the theme files and modify the colors:

```toml
[theme]
name = "my-custom-theme"

[colors]
Base = "@ansi_(51)"           # ANSI color code (0-255)
AlertInfo = "#00FF00"         # Hex color
Title = "cyan"                # Named color (from palette crate)
Important = "@rgb_(255,0,128)" # RGB values
```

### Available Color Meanings

- `Base` - Default text color
- `Title` - Section headers
- `Important` - Highlighted information
- `Guidance` - Help/instruction text
- `Annotation` - Secondary/supporting text
- `Muted` - Subtle text for contrast
- `AlertInfo` - Informational alerts
- `AlertWarn` - Warning messages
- `AlertError` - Error messages

### Color Format Options

Atuin supports multiple color formats:
- **Named colors**: `"cyan"`, `"magenta"`, `"teal"`, etc. ([see palette crate](https://docs.rs/palette/latest/palette/named/))
- **Hex codes**: `"#ff0088"`
- **ANSI codes**: `"@ansi_(51)"` (0-255) - [see cheat sheet](https://www.ditig.com/256-colors-cheat-sheet)
- **RGB values**: `"@rgb_(255, 128, 0)"`

See [Atuin's theming documentation](https://docs.atuin.sh/cli/guide/theming/) for more details.

## 🌈 ANSI Color Reference

The themes use these ANSI color codes:

| Code | Color | Usage |
|------|-------|-------|
| 51 | Neon Cyan | Primary text, accents |
| 201 | Neon Magenta | Titles, borders |
| 46 | Neon Green | Highlights, success |
| 226 | Neon Yellow | Warnings, matches |
| 213 | Neon Pink | Help text, guidance |
| 39 | Neon Blue | Info messages |
| 240 | Dark Gray | Muted/secondary text |
| 196 | Bright Red | Errors |

## 🎭 Matching Terminal Setup

For a complete cyberpunk terminal experience, pair these Atuin themes with:

- **Zsh**: [Oh My Zsh](https://ohmyz.sh/) cyberpunk prompt theme
- **Terminal colors**: Set your terminal to use a dark background
- **Font**: Consider a programming font like JetBrains Mono or Fira Code

## 📸 Screenshots

<!-- Add screenshots here showing the themes in action -->

```
# Coming soon! 
# Feel free to contribute screenshots via PR
```

## 🤝 Contributing

Found a bug or have a theme variant idea? Contributions are welcome!

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-theme`)
3. Commit your changes (`git commit -m 'Add amazing theme variant'`)
4. Push to the branch (`git push origin feature/amazing-theme`)
5. Open a Pull Request

## 📄 License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Atuin](https://github.com/atuinsh/atuin) - For the amazing shell history tool
- The cyberpunk aesthetic and all its neon glory

## 🔗 Links

- [Atuin Documentation](https://docs.atuin.sh)
- [Atuin Theming Guide](https://docs.atuin.sh/cli/guide/theming/)
- [256 Color Cheat Sheet](https://www.ditig.com/256-colors-cheat-sheet)
- [Report Issues](https://github.com/YOUR_USERNAME/YOUR_REPO/issues)

---

Made with 💖 and neon lights