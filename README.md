# Project Structure Generator

This Python script scans a directory and generates a JSON file representing the folder structure of the project. It's particularly useful for documenting the structure of large projects, such as Next.js applications.

## Features

- Recursively scans a directory to create a nested dictionary representation of the folder structure
- Excludes specified directories and files (e.g., `.git`, `node_modules`)
- Generates a JSON file with the project structure
- Prints a preview of the structure to the console

## Requirements

- Python 3.x

## Usage

1. Clone or download this script to your local machine.

2. Open the script in a text editor and modify the `project_path` variable in the `main()` function to point to your project's root directory:

   ```python
   project_path = r"INPUT PROJECT PATH HERE"
   ```

   Replace `"INPUT PROJECT PATH HERE"` with the actual path to your project.

3. Run the script:

   ```
   python project_structure_generator.py
   ```

4. The script will generate a file named `nextjs_project_structure.json` in the same directory as the script, containing the JSON representation of your project structure.

5. A preview of the structure will also be printed to the console.

## Customization

You can customize the script by modifying the following:

- **Output file name**: Change the `output_file` variable in the `main()` function.
- **Excluded directories**: Modify the `exclude` set in the `main()` function to add or remove directories/files you want to exclude from the scan.

## Functions

### `scan_directory(path, exclude=set())`

Recursively scans a directory and returns its structure as a dictionary.

- `path`: The directory path to scan
- `exclude`: A set of directory or file names to exclude from the scan

### `generate_structure_file(structure, output_file)`

Generates a JSON file representing the folder structure.

- `structure`: The dictionary representation of the folder structure
- `output_file`: The name of the output JSON file

### `main()`

The main function that orchestrates the scanning process and file generation.

## Note

This script is designed to work with local file systems. Make sure you have the necessary permissions to read the directory structure of your project.

## License

This script is provided as-is under the MIT License. Feel free to modify and distribute it as needed.
