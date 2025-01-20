# Medical Data Extraction System  

This repository contains a project that automates the extraction of key information from medical documents like prescriptions. The system utilizes PDF-to-image conversion, image processing, Optical Character Recognition (OCR), and text structuring to deliver structured data outputs.  

---

## **Features**  
- Converts PDFs to images for text extraction.  
- Enhances image quality using OpenCV for better OCR accuracy.  
- Extracts text from images using Tesseract OCR.  
- Uses regular expressions to structure extracted data into a JSON format.  

---

## **Tech Stack**  
- **Python**: Core programming language for the project.  
- **pdf2image**: Converts PDF documents to images.  
- **OpenCV**: Processes and enhances images.  
- **pytesseract**: Extracts text from images using OCR.  
- **Regex**: Structures unstructured text into key fields.  

---

## **How It Works**  

1. **PDF to Image Conversion**:  
   Converts PDF files to images using `pdf2image`.  

2. **Image Processing**:  
   Enhances images with OpenCV to improve text clarity for OCR.  

3. **Text Extraction**:  
   Extracts text from the processed images using `pytesseract`.  

4. **Data Structuring**:  
   Uses regular expressions to identify and extract specific fields like patient name, address, prescriptions, directions, and refills.  

---

## **Example Output**  

**Input**: A scanned prescription document.  
**Output**:  

```json
{
  "patient_name": "Maria Sharapova",
  "patient_address": "9 tennis court, new Russia, DC",
  "medicines": "Prednisone 20 mg, Lialda 2.4 gram",
  "directions": "Prednisone, Taper 5 mg every 3 days, finish in 2.5 weeks",
  "refills": "2"
}
```  

---

## **Setup and Usage**  

### **Prerequisites**  
- Python 3.x  
- Libraries: `pdf2image`, `opencv-python`, `pytesseract`, `poppler-utils`  

### **Steps**  

1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/medical-data-extraction
   cd medical-data-extraction
   ```  

2. Install the required dependencies:  
   ```bash
   pip install -r requirements.txt
   ```  

3. Run the script with a sample PDF:  
   ```bash
   python main.py --file sample_prescription.pdf
   ```  

---

## **Project Workflow**  

1. **Input**: PDF medical document.  
2. **Processing**:  
   - Convert PDF to image.  
   - Enhance image quality.  
   - Extract text using OCR.  
3. **Output**: Structured JSON data.  

---

## **Future Enhancements**  
- Support for multi-page PDF documents.  
- Integration with cloud OCR APIs for enhanced accuracy.  
- A web-based interface for real-time document processing.  

---

## **Contributions**  
Contributions, issues, and feature requests are welcome! Feel free to open a pull request or issue in this repository.  

---

## **License**  
This project is licensed under the MIT License.  

---

Feel free to explore and use this project! 😊  
