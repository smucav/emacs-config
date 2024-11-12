
# Emacs Configuration for Go, Python, and C Development

This Emacs configuration is tailored for Go, Python, and C development, enhancing syntax highlighting, line numbering, automatic formatting, and efficient package management for a smooth coding experience across multiple programming languages.

## Features

### 1. Package Management
- Sets up package archives from **MELPA**, **GNU**, and **Org** repositories.
- Automatically installs and ensures required packages are available using **`use-package`**.

### 2. Custom Font and Theme
- Sets the default font to `Ubuntu Sans Mono-12` for a clean, readable text appearance.
- Uses a dark theme with custom colors for high-contrast visibility.
- Defines specific syntax highlighting colors for comments, constants, functions, keywords, strings, types, and variables.

### 3. Syntax Highlighting
- **Data Types** in Go (`int`, `float32`, etc.) are highlighted in bold with a custom color.
- **Booleans** (`true` and `false` in Go) are highlighted in red for quick recognition.

### 4. Relative Line Numbers
- Enables relative line numbers for efficient navigation in the code.

### 5. Auto-Pairing
- Activates **electric-pair-mode** for automatic closing of brackets, quotes, and parentheses as you type.

### 6. Whitespace Management
- Provides an option to visualize tabs, spaces, and trailing spaces (currently commented out but can be enabled if needed).

### 7. Auto-Formatting
- Uses **`format-all`** for consistent formatting across files, with automatic formatting applied on save in Go, Python, and C files.

### 8. Language-Specific Settings
#### Python
- Sets indentation to 4 spaces for Python, following PEP 8 standards.
- Disables auto-indentation to provide more control over spacing.

#### Go
- Configures `go-mode` with a tab width of 4 and enables `gofmt` on save to automatically format code.
- Adds Go environment paths (`GOPATH` and `GOROOT`) to `exec-path`.

#### C
- Configures C programming to follow the **BSD style** with a tab width of 8.
- Sets indentation to 8 spaces for consistent alignment in C programs.

### 9. Minimal Scrolling
- Configures Emacs to scroll one line at a time, avoiding disorienting jumps by half a screen.

### 10. Backup Files
- Disables backup file creation to prevent clutter in project directories.

## Installation and Setup

1. **Clone this repository** (or copy this configuration file into your Emacs setup).

2. **Ensure Go and Python** are installed, and set up the necessary environment variables for Go (`GOPATH`, `GOROOT`).

3. **Install C, Go, and Python Development Tools** if not already available:
   - Python interpreter (`python3`).
   - Go tools (via `go get` or package manager).
   - C compiler (e.g., `gcc`).

4. **Restart Emacs** for the configuration to take effect. Emacs will automatically install the necessary packages on startup.
