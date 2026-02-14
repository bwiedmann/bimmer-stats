# Bimmer Stats

Forked from https://github.com/liz3/bimmer-stats

A visualization tool for reading and displaying CSV files produced by the BimmerLink app in an interactive graph view.

## Prerequisites

This application requires the following dependencies:

- **SDL2** - Simple DirectMedia Layer 2
- **SDL2_ttf** - TrueType font support for SDL2
- **Go 1.16 or later**
- **Roboto-Regular.ttf** font file in the project root directory

### Installing Dependencies

**macOS:**
```bash
brew install sdl2 sdl2_ttf
```

**Ubuntu/Debian:**
```bash
sudo apt-get install libsdl2-dev libsdl2-ttf-dev
```

**Windows:**
Follow the installation instructions at [go-sdl2](https://github.com/veandco/go-sdl2)

## Compiling

```bash
go build
```

This will create a `bimmer_stats` executable in the current directory.

## Usage

```bash
./bimmer_stats
```

The application will open a window. Use keyboard shortcuts to interact with the visualizer.

### Keyboard Shortcuts

#### File Operations
| Key | Action |
|-----|--------|
| `O` | Open file dialog |
| `Enter` | Load file (when in file dialog) |
| `Backspace` | Delete character from path (in file dialog) |
| `Ctrl + Backspace` | Clear entire path (in file dialog) |
| `Ctrl + V` | Paste path from clipboard (in file dialog) |
| `Escape` | Close file dialog |
| `Ctrl + E` | Close current file |

#### Navigation & Zoom
| Key | Action |
|-----|--------|
| `E` | Zoom in (scale factor +1) |
| `Q` | Zoom out (scale factor -1) |
| `W` | Scroll graphs up |
| `S` | Scroll graphs down |
| `A` | Offset left |
| `D` | Offset right |

#### View Options
| Key | Action |
|-----|--------|
| `L` | Toggle time line visibility |

## File Format

The application reads CSV files produced by the BimmerLink app. Place your CSV files in the project directory or provide the full path when opening files.

## License

Free software under GPL 2.0