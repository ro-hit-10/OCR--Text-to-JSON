# Invoice Digitization and Document Processing Pipeline

## 📌 Overview
This project, developed during my internship at **Data North Technologies (Jun 2024 – Present)**, focuses on automating the digitization of invoices.  
The pipeline converts scanned and digital invoice documents into **searchable PDFs** and **structured CSV/JSON outputs** using **PaddleOCR**.  

By leveraging **PP-OCRv5** and **PP-StructureV3**, the system extracts text, tables, and layouts with high accuracy, reducing manual data entry and enabling downstream analytics.

---

## 🚀 Key Features
- 📄 **Invoice Digitization**: Converts scanned/digital invoices into machine-readable formats.  
- 🔍 **Text & Layout Extraction**: High-accuracy OCR (91.7% precision) using PP-OCRv5.  
- 📊 **Table Recognition**: Structural parsing with PP-StructureV3 for tabular data recovery.  
- 🗂️ **Multi-format Output**:
  - Searchable PDFs (layout preserved)  
  - Structured CSV files (for analytics/reconciliation)  
  - JSON files with text + positional metadata  
- ⚡ **Automation**: End-to-end invoice processing pipeline with pre/post-processing for quality improvement.  

---

## 📂 Repository Structure
- `notebook.ipynb` → Main implementation of the document processing pipeline  
- `README.md` → Project documentation and usage guide  

---

## 🛠️ Technologies Used
- **Python 3.x**
- **PaddleOCR (PP-OCRv5, PP-StructureV3)**
- **OpenCV** – preprocessing scanned invoices  
- **Matplotlib / Seaborn** – visualization  
- **Pandas, NumPy** – structured data handling  
- **Google Colab** – development environment  

---

## 📊 Project Workflow
1. **Setup & Imports**  
   Install PaddleOCR and required libraries.  

2. **Data Loading**  
   Load scanned or digital invoice images.  

3. **Preprocessing**  
   Apply image cleaning, resizing, and thresholding for OCR readiness.  

4. **OCR & Layout Detection**  
   - Text extraction with PP-OCRv5  
   - Layout & table recognition with PP-StructureV3  

5. **Output Generation**  
   - Export structured CSVs  
   - Generate searchable PDFs with overlaid text  
   - Store full JSON metadata (text + bounding boxes)  

6. **Results & Evaluation**  
   - Achieved **91.7% OCR precision** across diverse invoice formats  
   - Reduced manual data entry & improved data consistency  

---

## ▶️ How to Run
### Option 1: Run on Google Colab
Click below to open and run the notebook in Google Colab:

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ro-hit-10/OCR--Text-to-JSON/blob/main/notebook.ipynb)

