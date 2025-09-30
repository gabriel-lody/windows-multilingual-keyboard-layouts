# German QWERTZ Multilingual Keyboard Layout

A custom German QWERTZ keyboard layout for Windows that enables typing in French, Catalan, Portuguese, and Spanish while maintaining the familiar German layout.

## Overview

This layout extends the standard German QWERTZ keyboard with additional dead keys and character combinations, allowing users to type in multiple Romance languages without switching keyboard layouts or memorizing complex Alt codes.

**Target audience:** Native speakers of French, Catalan, Portuguese, Spanish, and other Romance languages living in Germany who need to type both in German and their native language.

## Supported Languages

- **German** - Full native support (standard QWERTZ)
- **French** - All accents including ë, ï, ç
- **Catalan** - Including punt volat (·), ï, ç, and all accents  
- **Portuguese** (Brazilian & European) - Including ã, õ, ç, and all accents
- **Spanish** - Including ñ and all accents

## Key Features

### New Dead Keys
- **Tilde (~)** - AltGr + Plus (+): Creates ã, Ã, ñ, Ñ, õ, Õ
- **Diaeresis (¨)** - AltGr + Quote ("): Creates ë, Ë, ï, Ï

### Enhanced Existing Dead Keys  
- **Acute (´)** - Now also creates ç, Ç (cedilla)

### Direct Characters
- **Middle dot (·)** - AltGr + Period (.) for Catalan "punt volat"

## Character Map

### Tilde combinations (AltGr + Plus, then letter)
| Key | Result | Unicode |
|-----|--------|---------|
| a | ã | U+00E3 |
| A | Ã | U+00C3 |
| n | ñ | U+00F1 |
| N | Ñ | U+00D1 |
| o | õ | U+00F5 |
| O | Õ | U+00D5 |

### Diaeresis combinations (AltGr + ", then letter)
| Key | Result | Unicode |
|-----|--------|---------|
| e | ë | U+00EB |
| E | Ë | U+00CB |
| i | ï | U+00EF |
| I | Ï | U+00CF |

### Acute combinations (´ key, then letter) - *Enhanced*
| Key | Result | Unicode |
|-----|--------|---------|
| c | ç | U+00E7 |
| C | Ç | U+00C7 |
| *...and all existing acute accents (á, é, í, ó, ú, ý)* |

### Direct access
| Combination | Result | Unicode | Usage |
|-------------|--------|---------|--------|
| AltGr + . | · | U+00B7 | Catalan middle dot |

## Installation

### Requirements
- Windows 10/11
- Administrator privileges for installation
- Microsoft Keyboard Layout Creator (MSKLC)

### Steps
1. **Download MSKLC**: Get the [Microsoft Keyboard Layout Creator](https://www.microsoft.com/en-us/download/details.aspx?id=102134) from Microsoft's official website and install it

2. **Download the layout file**: Download `GerLinux.klc` from this repository

3. **Load the layout in MSKLC**:
   - Open Microsoft Keyboard Layout Creator
   - Go to File → Load Source File...
   - Select the downloaded `GerLinux.klc` file

4. **Build and install**:
   - In MSKLC, go to Project → Build DLL and Setup Package
   - When prompted about viewing logs, click "No"
   - Click "Yes" to open the output folder
   - Run the generated `setup.exe` as administrator
   - Follow the installation wizard

5. **Activate the layout in Windows**:
   - Go to Settings → Time & Language → Language
   - Select your language → Options → Add a keyboard
   - Choose "German Linux Deadkeys"

### Customization
The .klc source file allows you to modify the layout before installation. You can adjust key combinations, add new characters, or change dead key behaviors using the MSKLC interface.

## Usage Examples

### Catalan
- **intel·ligent** - i, n, t, e, l, AltGr+., l, i, g, e, n, t
- **països** - p, a, AltGr+", then i, s, o, s

### French  
- **Citroën** - C, i, t, r, o, AltGr+", then e, n
- **français** - f, r, a, n, ´, then c, a, i, s

### Portuguese
- **caminhões** - c, a, m, i, n, h, AltGr+Plus, then o, e, s
- **coração** - c, o, r, a, ´, then c, AltGr+Plus, then a, o

### Spanish
- **mañana** - m, a, AltGr+Plus, then n, a, n, a

## Design Rationale

### Why these key combinations?

- **AltGr + Plus for tilde**: The Plus (+) and Tilde (~) share the same physical key, making this intuitive
- **AltGr + Quote for diaeresis**: German keyboards have dedicated ä, ö, ü keys, so the quote (") key is repurposed for the similar diaeresis function
- **Acute + C for cedilla**: Leverages the existing acute dead key, since cedilla and acute are both diacritical marks
- **AltGr + Period for middle dot**: Simple and direct access for the Catalan "punt volat"

### Advantages over standard layouts
- **No layout switching required**: Type German and Romance languages seamlessly
- **Familiar QWERTZ**: All existing German keys remain in their expected positions
- **Intuitive combinations**: Dead key choices follow logical associations

## Compatibility

- Tested on Windows 11
- Works with all applications that support Unicode input
- Compatible with both 32-bit and 64-bit systems

## Troubleshooting

### Layout not appearing in Windows Settings
1. Restart your computer after installation
2. Try logging out and back in
3. Check if installation completed successfully (no error messages)

### Dead keys not working
1. Ensure you're using the correct key combinations
2. Try in a Unicode-aware application like Notepad
3. Verify the layout is selected as your active keyboard

### Uninstallation
Run the original setup.exe and choose "Remove" option, or use Windows Apps & Features to uninstall "German Linux Deadkeys".

## Contributing

Issues and suggestions are welcome. Please include:
- Your Windows version
- Specific use case or language requirement
- Steps to reproduce any problems

## License

This keyboard layout is provided as-is for public use. Based on the standard German keyboard layout.

---

**Note**: This layout maintains full compatibility with standard German typing while adding multilingual capabilities. All original German functionality is preserved.
