# PDF Data Extraction Tool / PDF-Datenextraktionstool

_________________________________________
## English

### Description
This Python script extracts tables from PDF files and saves them as CSV files. It processes multiple PDF files and creates separate CSV files for each table found in the PDFs.

### Features
- Extracts all tables from PDF files
- Saves each table as a separate CSV file
- Supports multiple PDF files processing
- UTF-8 encoding for proper character handling
- Error handling for missing files and processing errors

### Requirements
- Python 3.x
- tabula-py library
- Java Runtime Environment (JRE) - required by tabula-py

### Installation
```bash
pip install tabula-py
```

### Usage
1. Place your PDF files in the same directory as the script
2. Update the `pdf_files` list in `main.py` with your PDF filenames
3. Run the script:
```bash
python main.py
```

### Output
The script will create CSV files with the following naming convention:
- `{original_pdf_name}_table_{table_number}.csv`

### Example
For a PDF file named `document.pdf` with 2 tables, the output will be:
- `document_table_1.csv`
- `document_table_2.csv`

---

_________________________________________
## Deutsch

### Beschreibung
Dieses Python-Skript extrahiert Tabellen aus PDF-Dateien und speichert sie als CSV-Dateien. Es verarbeitet mehrere PDF-Dateien und erstellt separate CSV-Dateien für jede in den PDFs gefundene Tabelle.

### Funktionen
- Extrahiert alle Tabellen aus PDF-Dateien
- Speichert jede Tabelle als separate CSV-Datei
- Unterstützt die Verarbeitung mehrerer PDF-Dateien
- UTF-8-Kodierung für ordnungsgemäße Zeichenbehandlung
- Fehlerbehandlung für fehlende Dateien und Verarbeitungsfehler

### Anforderungen
- Python 3.x
- tabula-py Bibliothek
- Java Runtime Environment (JRE) - erforderlich für tabula-py

### Installation
```bash
pip install tabula-py
```

### Verwendung
1. Legen Sie Ihre PDF-Dateien im gleichen Verzeichnis wie das Skript ab
2. Aktualisieren Sie die `pdf_files` Liste in `main.py` mit Ihren PDF-Dateinamen
3. Führen Sie das Skript aus:
```bash
python main.py
```

### Ausgabe
Das Skript erstellt CSV-Dateien mit folgender Namenskonvention:
- `{original_pdf_name}_table_{tabellennummer}.csv`

### Beispiel
Für eine PDF-Datei namens `dokument.pdf` mit 2 Tabellen wird die Ausgabe sein:
- `dokument_table_1.csv`
- `dokument_table_2.csv`
