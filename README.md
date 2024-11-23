# OCR-Based Text Detection on Medicine Photos

This project demonstrates a text detection and recognition system using EasyOCR and OpenCV to extract and highlight text from medicine images. The detected text is displayed with bounding boxes for easy visualization, making it useful for applications such as automating text extraction for medical records or packaging analysis.

## Features
- **Text Detection and Recognition**: Uses EasyOCR to read text from images, supporting multi-line and multi-language (extendable) detection.
- **Bounding Box Visualization**: Draws bounding boxes around detected text for visual confirmation.
- **Detected Text Export**: Displays and stores extracted text for further analysis.
- **Image Annotation**: Annotates the image with recognized text, aiding in visual understanding.

---

## How It Works
1. **Input**: An image containing medicine packaging (e.g., a photo of a medicine strip or box).
2. **Processing**:
   - EasyOCR detects and reads text from the image.
   - Bounding boxes are created for each detected text region.
   - Recognized text is displayed and saved.
3. **Output**:
   - An annotated image with bounding boxes and text displayed.
   - A list of all detected text in the console for further use.

---

## Setup and Dependencies

### Prerequisites
- Python 3.x
- Required libraries:
  ```bash
  pip install easyocr opencv-python-headless matplotlib numpy
  ```
### Files
- `main.py`: Script for OCR text detection and visualization.
- `2.jpg`: Sample input image (medicine photo).

---

## Usage

### Step 1: Clone the Repository
```bash
  git clone https://github.com/YourUsername/MedicineOCR.git  
  cd MedicineOCR  
  ```
### Step 2: Run the Script
```bash
python main.py 
``` 
### Step 3: View Output
- The annotated image with detected text is displayed.
- Extracted text appears in the console for further processing.

---

## Sample Output
### Detected Text (Example)
```bash
Detected Text:  
1. NFwL  
2. Rac  
3. Acets 400 mg  
4. Manufactured by Alembic Pharmaceuticals Ltd  
5. Store protected from moisture at a temperature not exceeding 25°C.  
```

### Annotated Image
The output displays bounding boxes and text overlaid on the input image.

---

## Applications
- Medical Record Digitization: Automate the process of extracting text from prescriptions and packaging.
- Inventory Management: Quickly digitize data from medicine labels.
- Accessibility: Assist visually impaired users by reading text from medicine packages.

---

### Future Enhancements
- Language Support: Extend the OCR to support multiple languages.
- GUI Application: Build a user-friendly interface for non-technical users.
- GPU Acceleration: Enable GPU support for faster processing.
