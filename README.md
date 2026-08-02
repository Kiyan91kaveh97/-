# Pardis School System

Pardis School System is an Excel + VBA based solution for managing school data, reports, and administrative workflows. The primary workbook lives in Excel/Pardis.xlsm and the macros and forms are organized under the VBA/ directory for easier maintenance and versioning.

Repository layout

- Excel/
  - PardisSchool.xlsm         # Main macro-enabled workbook
  - Backup/                   # Workbook backups and exported versions
  - Database/                 # Local database files or exports

- VBA/
  - Forms/                    # UserForm definitions exported from the VBA editor
  - Modules/                  # Standard modules (.bas) with procedures and functions
  - Classes/                  # Class modules (.cls)

- Docs/
  - Requirements.md
  - Database.md
  - Changelog.md

- Assets/
  - Logo/
  - Icons/
  - Images/

- README.md

Quick start

1. Install prerequisites
   - Microsoft Excel (desktop) with macro support (xlsm).
   - (Optional) Rubberduck or another VBA development tool for advanced refactoring.

2. Open the workbook
   - Open `Excel/PardisSchool.xlsm` in Excel.
   - If prompted, enable macros (only if you trust this file).

3. Back up before use
   - Make a copy of the workbook (save in `Excel/Backup/`) before running any administrative macros or bulk imports.

Development & editing VBA code

- The VBA project is also exported into the `VBA/` folder for version control. Each module, form, and class should be stored as a text file (.bas, .frm, .cls) so they can be tracked in Git.
- To export modules from Excel:
  1. Open the Visual Basic Editor (Alt+F11).
  2. Right-click the module/UserForm and choose `Export File...`.
  3. Save into the appropriate folder under `VBA/`.
- To import modules back to the workbook, use `Import File...` from the same right-click menu.

Security notes

- Macros can run code with file system and network access. Only enable macros for files from trusted sources.
- Do not store sensitive credentials in plain text inside the workbook or VBA code.

Contributing

- Submit issues or PRs to propose changes to documentation, exported VBA code, or the workbook structure.
- When updating VBA code, export the changed modules into `VBA/` so diffs are visible.

License

- Add a LICENSE file to this repository and choose an appropriate license for your project.

Contact

- Maintainer: Kiyan (GitHub: @Kiyan91kaveh97)
