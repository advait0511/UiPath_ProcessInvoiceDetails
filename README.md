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
4. AI extraction (gpt 5.2)
5. Regex parsing
6. Send SMTP Email
7. Add Data Row
8. Write to Excel

---

## 📂 Project Structure

Invoice_Document_Understanding_Advait/
│
├── Workflows
│   ├── Main.xaml
│
├── Data/
│   ├── Input/
│   │   ├── (Invoices PDF to be stored here)
│   └── Output/
│       └── (Excel file generated here)
│
├── Screenshots/
│
└── README.md

---

## 📝 How to Run
1. Place PDFs in `Data/Input`
2. Open the project in UiPath Studio
3. Run `Main.xaml`
4. Output Excel appears in `Data/Output/InvoiceDetail.xlsx`

---

## 🛠 Technologies Used
- UiPath Studio
- UiPath.Excel.Activities
- UiPath.PDF.Activities
- UiPath GenAI Activities (gpt 5.2)


