# AuditData Parser - Changelog

All notable changes to this project will be documented in this file.

The format is based on [Semantic Versioning](https://semver.org/), and this project adheres to it.

---

## [1.1.0] - 2025-06-25

### Added

- Full graphical user interface (GUI) using Tkinter
- File chooser dialogs for input and output paths
- Logging system with timestamped messages to both GUI and log file
- SHA256 hashing of input and output files
- Large file detection and warning popup (>200MB)
- Overall progress bar and active processing phase label
- Cancel button with graceful thread termination
- Timestamp tracking:
  - Start time
  - Finish time
  - Elapsed duration (shown in GUI and logged)
- Multiprocessing JSON parsing for faster performance
- Summary report displaying total rows processed and JSON parsing errors
- Robust error handling with GUI notifications
- Export to CSV instead of Excel by default
- Support for creating a standalone EXE via PyInstaller

---

## [1.0.0] - Initial release

### Features

- Console-based script  
- Reads `.xlsx` or `.csv` files  
- Parses JSON from the `AuditData` column  
- Appends flattened JSON fields as new columns  
- Drops the original `AuditData` column  
- Exports to CSV in `~/Documents/ParsedAuditData`  
