#  DOCX to Excel Converter

A simple Python utility that automatically reads all `.docx` files from a folder, extracts their content (paragraphs and tables), and converts each document into a separate `.xlsx` file.

---

##  Features

-  Reads all `.docx` files from a specified input folder.
-  Extracts:
  - Paragraphs
  - Tables
-  Creates one Excel (`.xlsx`) file for each Word document.
-  Automatically creates an output folder if it doesn't exist.
-  Preserves the original filename.
-  Fast and easy to use.

---

##  Project Structure

```
docx-to-excel/
│
├── project/                 # Input folder containing DOCX files
│   ├── file1.docx
│   ├── file2.docx
│   └── ...
│
├── output/                  # Generated automatically
│   ├── file1.xlsx
│   ├── file2.xlsx
│   └── ...
│
├── docx_to_excel.py         # Main Python script
├── requirements.txt
└── README.md
```

---

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/docx-to-excel.git
cd docx-to-excel
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

or

```bash
pip install python-docx openpyxl
```

---

## ▶️ Usage

### Step 1

Place all your Word documents inside the **project** folder.

Example:

```
project/
│
├── University_A.docx
├── University_B.docx
├── University_C.docx
└── ...
```

### Step 2

Run the script.

```bash
python docx_to_excel.py
```

### Step 3

The script automatically creates an **output** folder.

```
output/
│
├── University_A.xlsx
├── University_B.xlsx
├── University_C.xlsx
└── ...
```

---

## 📋 Example

### Input

```
project/
├── Aligarh Muslim University Online MBA Details.docx
├── Amity University Online MBA Course Details.docx
├── Andhra University Online Course.docx
```

### Output

```
output/
├── Aligarh Muslim University Online MBA Details.xlsx
├── Amity University Online MBA Course Details.xlsx
├── Andhra University Online Course.xlsx
```

---

## 📦 Requirements

- Python 3.9+
- python-docx
- openpyxl

---

## 📄 requirements.txt

```
python-docx
openpyxl
```

---

## ⚙️ How It Works

1. Scans the `project/` directory.
2. Opens each `.docx` file.
3. Extracts:
   - Paragraphs
   - Tables
4. Creates a corresponding `.xlsx` file.
5. Saves the converted file into the `output/` directory.

---

## 💡 Future Improvements

- Preserve text formatting.
- Extract images.
- Merge multiple tables into separate worksheets.
- Command-line arguments for custom input/output folders.
- Logging and progress bar.
- Batch conversion with multiprocessing.
- GUI version using Tkinter or PyQt.

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository.
2. Create a new feature branch.

```bash
git checkout -b feature-name
```

3. Commit your changes.

```bash
git commit -m "Add new feature"
```

4. Push to your branch.

```bash
git push origin feature-name
```

5. Open a Pull Request.

---

## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.
