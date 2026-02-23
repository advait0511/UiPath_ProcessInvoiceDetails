# Invoice Extraction Automation (UiPath + GenAI)

This project automates the extraction of invoice details from PDF files using UiPath and GenAI (gpt 5.2).  
It processes multiple invoices, extracts structured fields, and writes the results into Excel.

---

## 🚀 Features
- Reads all PDF invoices from `/Data/Input`
- Uses GenAI to extract:
  - Invoice Number
  - Date (DD/MM/YYYY)
  - Amount (with currency)
- Parses extracted text using Regex
- Adds each invoice as a row in a DataTable
- Email invoice details
- Writes final output to Excel
- Includes Try/Catch for robust error handling
- Logs failures and continues processing

---

## 🧠 Workflow Steps
1. Build DataTable
2. Loop through all PDFs
3. Read PDF text
4. AI extraction (Claude Haiku)
5. Regex parsing
6. Add Data Row
7. Write to Excel

---

## 📂 Project Structure

