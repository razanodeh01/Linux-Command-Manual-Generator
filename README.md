# 📘 Linux Command Manual Generator (Shell Script)

## 🔍 Project Overview

This project automates the creation and validation of **Cisco-style man pages** for Linux/Unix commands using **Bash scripting**.

It consists of:
1. **Automated Generation** – Man pages are generated in a structured format.
2. **User-Driven Verification** – Command output and examples are verified and compared.
3. **Improved Usability** – A search function and recommendation system enhance user interaction.


## 🧰 Technologies Used
- 🐧 Bash scripting
- 📂 Shell utilities (`man`, `info`, `grep`, `awk`, `diff`, `compgen`).
- 🧪 Terminal-based CLI interaction.
- 📁 File I/O and directory manipulation.



## 📁 Features Breakdown

### 📄 Part 1 – Automated Manual Generation
- Creates a `GeneratedFiles/` folder.
- For each command:
  - Fetches description (via `man` or `info`).
  - Extracts version info (`uname -r`).
  - Adds example usage.
  - Lists related commands (via `compgen` and `grep`).
- Output is formatted in a Cisco-style template.

### ✅ Part 2 – Command Verification
- Re-generates data for any given command.
- Compares with the existing manual using `diff`.
- Highlights mismatches and confirms validated entries.

### 🔎 Part 3 – Extensions & Enhancements
- **Search** by:
  - Command name and section (e.g. Version, Example)
  - Topic across all generated manuals
- **Command Recommendation**:
  - Based on user history
  - Provides direct access to relevant command details.
  
## 🎥 Demo Video
Watch the video showing sample test cases and features in action:
https://github.com/razanodeh01/ENCS3130-LINUX-LABORATORY-/assets/133569873/858d7a2b-ff90-4e4c-8158-741646a22c57



