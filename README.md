# Electoral_Roll_Preproceessing
Electoral Data present on https://ceodelhi.gov.in/ to an easy to recognise and analyse CSV file.

## Steps Involved :
1. Download PDF using Selenium (haven't implemented it here, but you can contact with me on nameer3865@gmail.com for help.
2. Convert those pdf to cropped pdf
3. Convert cropped pdf to images
4. Get text from images using pytesseract OCR
5. Save text in Temp.csv
6. Preprocess temp.csv and save information to Final.csv

## Important Pre-Requisites
1. Install tesseract using windows installer available at: https://github.com/UB-Mannheim/tesseract/wiki

2. Note the tesseract path from the installation. Default installation path at the time of this edit was: C:\Program Files\Tesseract-OCR. It may change so please check the installation path.

3. pip install pytesseract

4. Set the tesseract path in the script before calling image_to_string:

pytesseract.pytesseract.tesseract_cmd = r'C:\Program Files\Tesseract-OCR\tesseract.exe'OR you can also set the path in enviroment variables. Do whatever you prefer
