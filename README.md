# PDF to Excel Converter

A simple Windows application that converts PDF files to Excel format, extracting tables and text content for easy data analysis.

## Features

- **Simple GUI Interface**: Easy-to-use graphical interface built with tkinter
- **Table Detection**: Automatically detects and extracts tables from PDF files
- **Text Extraction**: Extracts text content from PDF pages
- **Multiple Output Sheets**: Creates separate Excel sheets for each table found
- **Progress Tracking**: Real-time progress indication during conversion
- **Threading**: Non-blocking conversion process

## Requirements

- Python 3.7 or higher
- Windows operating system
- Required Python packages (see requirements.txt)

## Installation

1. **Clone or download this repository**
   ```bash
   git clone <repository-url>
   cd pdf-to-excel-converter
   ```

2. **Install required dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the application**
   ```bash
   python pdf_to_excel_converter.py
   ```

## Usage

1. **Launch the application** by running `pdf_to_excel_converter.py`

2. **Select PDF file**:
   - Click "Browse" next to "PDF File"
   - Choose your PDF file from the file dialog

3. **Choose output location**:
   - The Excel filename will be auto-generated based on the PDF name
   - You can modify the output path by clicking "Browse" next to "Output Excel File"

4. **Configure options**:
   - **Detect tables automatically**: Extracts tables from the PDF
   - **Extract text content**: Extracts plain text from PDF pages

5. **Start conversion**:
   - Click "Convert PDF to Excel"
   - Monitor progress in the progress bar
   - Wait for completion notification

## Output Format

The application creates an Excel file with the following structure:

- **Separate sheets for each table**: Tables are extracted to individual sheets named `Page_X_Table_Y`
- **Text content sheet**: All extracted text is saved to a "Text_Content" sheet
- **Summary sheet**: Created if no tables or text are found

## Supported File Types

- **Input**: PDF files (.pdf)
- **Output**: Excel files (.xlsx)

## Troubleshooting

### Common Issues

1. **"No tables found" message**:
   - The PDF might not contain structured tables
   - Try enabling "Extract text content" to get text data

2. **Conversion fails**:
   - Ensure the PDF file is not corrupted
   - Check if the output directory is writable
   - Verify all dependencies are installed

3. **Application won't start**:
   - Make sure Python is installed and in your PATH
   - Install all required packages: `pip install -r requirements.txt`

### Performance Tips

- For large PDF files, conversion may take several minutes
- The application uses threading to prevent UI freezing
- Progress is shown in real-time

## Dependencies

- `pandas`: Data manipulation and Excel file creation
- `pdfplumber`: PDF text and table extraction
- `openpyxl`: Excel file writing
- `tkinter`: GUI framework (usually included with Python)
- `Pillow`: Image processing support

## License

This project is open source and available under the MIT License.

## Contributing

Feel free to submit issues, feature requests, or pull requests to improve this application.

## Version History

- **v1.0.0**: Initial release with basic PDF to Excel conversion functionality 
