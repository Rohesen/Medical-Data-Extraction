# 🚀 Medical Data Extraction 🏥  

This repository showcases an automated system for extracting critical information from medical documents like prescriptions. It converts PDFs to images, processes them for better clarity, extracts text using OCR, and structures the data into a readable format.  

---

## 🌟 **Features**  
✅ Converts PDFs into images for efficient text extraction.  
✅ Enhances image quality using OpenCV for better OCR accuracy.  
✅ Extracts text from images using Tesseract OCR.  
✅ Structures unstructured text into a well-defined JSON format.  



![Medical Data Extraction Workflow](https://github.com/Rohesen/Medical-Data-Extraction/blob/main/medical%20data%20extraction%205.png)




---

## 🛠️ **Tech Stack**  
🔹 **Python**: The core programming language of the project.  
🔹 **pdf2image**: For converting PDF documents into images.  
🔹 **OpenCV**: For image preprocessing and enhancement.  
🔹 **pytesseract**: For text extraction using OCR technology.  
🔹 **Regex**: To structure the extracted text into key-value pairs.  

---

## 🔍 **How It Works**  

1️⃣ **PDF to Image Conversion**  
   - Converts PDF files to high-quality images using `pdf2image`.

![Medical Data Extraction Workflow](https://github.com/Rohesen/Medical-Data-Extraction/blob/main/medical%20data%20extraction%201.png)


2️⃣ **Image Processing**  
   - Enhances image clarity using OpenCV for improved OCR results.

     

![Simple Thresholding](https://github.com/Rohesen/Medical-Data-Extraction/blob/main/medical%20data%20extraction%203.png)





![Adaptive Thresholding](https://github.com/Rohesen/Medical-Data-Extraction/blob/main/medical%20data%20extraction%202.png)


 

3️⃣ **Text Extraction**  
   - Extracts meaningful text from images using `pytesseract`.



![Text Extraction](https://github.com/Rohesen/Medical-Data-Extraction/blob/main/medical%20data%20extraction%204.png)




4️⃣ **Data Structuring**  
   - Uses regular expressions to identify and organize fields like patient name, address, medications, and more.



---

## 🧾 **Example Output**  

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

## 📦 **Setup and Usage**  

### 📋 **Prerequisites**  
🔹 Python 3.x installed.  
🔹 Libraries: `pdf2image`, `opencv-python`, `pytesseract`, `poppler-utils`.  

### ⚙️ **Steps**  

1️⃣ Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/medical-data-extraction
   cd medical-data-extraction
   ```  

2️⃣ Install the required dependencies:  
   ```bash
   pip install -r requirements.txt
   ```  

3️⃣ Run the script with a sample PDF:  
   ```bash
   python main.py --file sample_prescription.pdf
   ```  

---

## 📂 **Project Workflow**  

1️⃣ **Input**: A PDF medical document.

2️⃣ **Processing**:  
   - Convert PDF to image.  
   - Enhance image quality.  
   - Extract text using OCR. 

3️⃣ **Output**: A structured JSON file with extracted data.  


---

![Review Video](https://github.com/Rohesen/Medical-Data-Extraction/blob/main/project_review_video.gif)


---

## 🚀 **Future Enhancements**  
✨ Add support for multi-page PDFs.  
✨ Integrate cloud OCR APIs for enhanced accuracy.  
✨ Build a web-based interface for real-time document uploads and processing.  

---

## 🤝 **Contributions**  
Contributions, issues, and feature requests are welcome! Feel free to open a pull request or issue in this repository.  

---

## 📜 **License**  
This project is licensed under the **MIT License**.  

---

🎉 Feel free to explore the project, use it, or contribute to make it even better! Let's connect if you'd like to collaborate. 😊  
