# Document Analyzer with Summarization & Question Generation

This project provides a multi-functional document analyzer that supports text extraction, summarization, and question generation. The tool supports various input formats like PDFs, images, audio, Excel, Word, and PowerPoint files. Leveraging `transformers`, `OCR (Tesseract)`, `PyMuPDF`, and other machine learning libraries, it can handle multilingual content (especially Arabic and English) for both summarization and question generation tasks.

## Features
- **Text Extraction**: Extract text from documents including PDFs, images, audio files, Excel, Word, and PowerPoint.
- **Summarization**: Summarize extracted text in either Arabic or English.
- **Question Generation**: Generate comprehension questions based on the extracted text.

## Supported File Formats
- **Documents**: PDF, DOCX, XLSX, PPTX
- **Images**: PNG, JPG, JPEG
- **Audio**: MP3, WAV
- **Text**: Plain text

## Technologies Used
- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) for optical character recognition (text extraction from images)
- [PyMuPDF](https://github.com/pymupdf/PyMuPDF) for PDF processing
- [Transformers](https://github.com/huggingface/transformers) for summarization and question generation using Meta's Llama models
- [Gradio](https://github.com/gradio-app/gradio) for creating the user interface
- [SpeechRecognition](https://github.com/Uberi/speech_recognition) for converting audio files to text
- [OpenCV](https://github.com/opencv/opencv) for image processing
- [PyMuPDF](https://github.com/pymupdf/PyMuPDF) for working with PDF files
- [python-docx](https://github.com/python-openxml/python-docx) for working with Word documents
- [openpyxl](https://github.com/jmcnamara/openpyxl) for working with Excel files
- [python-pptx](https://github.com/scanny/python-pptx) for working with PowerPoint files

## Installation
### Prerequisites
- Python 3.8+
- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) installed on your system.
  
You can install Tesseract with:
  sudo apt-get install tesseract-ocr -y
  sudo apt-get install tesseract-ocr-ara -y  # For Arabic support

##Clone the Repository
git clone https://github.com/your-username/document-analyzer.git
cd document-analyzer

## Install Dependencies
Install the required Python libraries:
pip install -r requirements.txt

## Download Trained Data for OCR (Arabic Support)
wget https://github.com/tesseract-ocr/tessdata/raw/master/ara.traineddata -P /usr/share/tesseract-ocr/4.00/tessdata/

## Usage
  1-Text Input: Enter text manually or upload a file for analysis.
  2-Select OCR Language: Choose between eng for English and ara for Arabic for text extraction from images.
  3-Choose Task: You can choose to perform text extraction, summarization, and/or question generation.
  4-Set Parameters: Specify the length of the summary or the number of questions you want generated.
  5-Process: Click "Submit" to process the input and retrieve results.

##Select Task:
  OCR Language: Choose the language for OCR (Arabic or English).
  Task Selection: Choose whether you want to perform Summarization or Question Generation (or both).
  Summarization Language: Select the language for the summary (Arabic or English).
  Summary Length: Set the maximum number of words for the summary.
  Number of Questions: Specify how many questions you want to generate.

## Sample Input and Output
  # Input
  Upload a PDF, DOCX, or an image with text, and select Summarization.
  Choose English or Arabic summarization and specify the word count.
  # Output
  Extracted Text: Full text from the document.
  Summary: A concise summary of the text.
  Generated Questions: A list of comprehension questions based on the document's content.

## Example
Upload a PDF, image, or audio file, select the OCR language, and specify if you want a summarization or question generation. The extracted text will be processed, and the results will be displayed.

## Contributing
We welcome contributions to improve this project! If you would like to contribute, please fork the repository, create a new branch, and submit a pull request.

## Acknowledgements
This project uses the following libraries and models:

  Gradio: For building the user interface.
  Tesseract: For OCR processing.
  Hugging Face Transformers: For text generation, summarization, and question generation.
  LLAMA Models: For advanced text generation tasks.
  OpenCV: For image processing.
  SpeechRecognition: For audio transcription.
  Pytesseract: For integrating Tesseract with Python.

