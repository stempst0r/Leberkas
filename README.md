# Leberkas - CSV to XLSX Converter and Data Management Tool

Leberkas is a Python application that allows you to import CSV files exported by Chainalysis Reactor, manage data, and generate XLSX files from the imported data for each service provider. It provides a graphical user interface (GUI) for ease of use.
## Features

* Select and import multiple CSV files.
* Manage/Store imported data in an SQLite database.
* Generate XLSX files from the imported data.
* Easily filter and export data by service provider.

## Prerequisites

Before using Leberkas, make sure you have the following dependencies installed:

* Python 3.x (created with 3.11)
* [tkinter](https://docs.python.org/3/library/tkinter.html) (usually included in Python standard library)
* [sqlite3](https://docs.python.org/3/library/sqlite3.html) (usually included in Python standard library)
* [openpyxl](https://openpyxl.readthedocs.io/en/stable/)
* [et-xmlfile](https://et-xmlfile.readthedocs.io/en/latest/)


You can install the required Python packages using pip by running:

`pip install -r requirements.txt`

## Usage

1. Run the application by executing the following command in your terminal:

    `python leberkas.py`

2. The Leberkas GUI window will appear, allowing you to perform the following actions:
    * Add CSV: Click this button to select and import one or more CSV files.
    * Remove CSV: Select files in the list and click this button to remove them from the import queue.
    * Import: Click this button to import the selected CSV files into the SQLite database.
    * Generate XLSX: Click this button to generate XLSX files from the imported data.
    * Terminal Output: The terminal output panel displays information and progress updates.

3. To filter and export data by service provider:
    * Click the "Generate XLSX" button to export all data. Exported data will be stored in `/export`

## Database

The application uses an SQLite database named data.db to store imported data. The database file is created automatically when you run the application for the first time. It will be deleted when closing the GUI.

## Contributing

If you would like to contribute to Leberkas, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Make your changes and commit them.
4. Push your changes to your fork.
5. Submit a pull request to the main repository.

## License

This project is licensed under the [GNU General Public License (GPL)](LICENSE).

* Permissions: The GPL is a copyleft license, which means that any derivative work, modifications, or extensions of this software must also be licensed under the GPL. Users are free to use, modify, and distribute this software, but they must share their modifications and derivative works under the same terms.
* Conditions: When you distribute this software or any derivative work, you are required to include the full text of the GPL license, along with the original copyright notices, and you must make the source code of the software available to anyone who receives it.
* Limitations: The GPL is designed to ensure that open-source software remains open source. It places restrictions on how the software and any derivative works can be distributed. If you plan to include GPL-licensed code in your own projects, be aware that those projects will also need to be GPL-licensed.

Please review the [LICENSE](LICENSE) file for the full text of the GNU General Public License (GPL).
