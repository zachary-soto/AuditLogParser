AuditData Parser

AuditData Parser is a desktop utility that reads .xlsx or .csv files containing an AuditData column with JSON-encoded values, parses the JSON content, and exports a new spreadsheet with the JSON fields flattened into columns.

🔧 Features
✅ Parse and flatten JSON stored in an AuditData column
✅ Support for .xlsx and .csv input files
✅ Graphical User Interface (GUI) using Tkinter
✅ SHA256 hashing of input and output files
✅ Log output (GUI and .log file)
✅ Overall progress bar and active task phase label
✅ Cancel operation gracefully
✅ Tracks start time, finish time, and duration
✅ Large file warning (over 200MB)
✅ Multiprocessing JSON parsing for faster performance
✅ Summary report with JSON error counts
✅ Error handling with GUI notifications

📦 Installation
This tool runs on Python 3.9 or higher. To get started:

pip install pandas openpyxl

🚀 Usage
Run the application via:

python AuditDataParser.py

From the GUI:

Click Browse File to select your spreadsheet
Click Save As to choose the output location and filename
Click Parse and Export to run
Monitor logs and progress in real time

🧱 EXE Distribution
A standalone EXE file is available in the `dist` folder.  
The EXE can be run on Windows machines without Python installed.  
Make sure to provide input files separately when running the EXE.

🧪 Example
Input file:

| ID | AuditData                             |
|----|-------------------------------------|
| 1  | {"User":"alice","Action":"Login"}   |

Output file:

| ID | User  | Action |
|----|-------|--------|
| 1  | alice | Login  |

📜 License
This project is licensed for internal or investigative use. Contact the author for redistribution permissions.

📘 Changelog
See CHANGELOG.md for version history.
