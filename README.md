# Invoice Processing Bot with Smart Validation & Approval Workflow

##  Overview
Automated invoice processing system built with UiPath that reads PDF invoices, validates vendor information against master data, and manages approval workflows based on spending limits.

## Features
- **OCR PDF Processing**: Extracts invoice data from PDF documents
- **Vendor Validation**: Checks vendor against master database
- **Smart Approval Logic**: Routes high-value invoices for approval
- **Comprehensive Logging**: Creates detailed audit trail in CSV format
- **Error Handling**: Robust error management with Try-Catch blocks
- **Professional Architecture**: Clean, maintainable code structure

## Project Structure
InvoiceProcessingBot/
├── Main_InvoiceProcessor.xaml    # Main workflow
├── Data/
│   └── VendorMasterData.xlsx     # Vendor master database
├── Input/
│   └── *.pdf                     # Invoice PDFs to process
├── Output/
│   └── ApprovalLog.csv          # Processing results log
└── Config/
└── (Configuration files)

## Setup Instructions
1. Clone this repository
2. Open `Main_InvoiceProcessor.xaml` in UiPath Studio
3. Place your vendor data in `Data/VendorMasterData.xlsx`
4. Add invoice PDFs to the `Input/` folder
5. Run the workflow

## Sample Output
The bot processes invoices and creates detailed logs:
- Auto-approved invoices (within vendor limits)
- Approval-required invoices (exceeding limits)  
- Invalid vendor alerts (unknown vendors)

## Technologies Used
- UiPath Studio
- Document Understanding (OCR)
- Excel/Workbook Activities
- Regular Expressions for data parsing
- CSV logging system

## Business Value
- Reduces manual invoice processing time by 80%
- Ensures compliance with vendor approval limits
- Creates comprehensive audit trail
- Eliminates human errors in data entry
- Scalable for high-volume processing

## Author
Roya Valiyeva
