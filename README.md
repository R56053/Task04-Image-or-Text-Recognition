# Image-or-Text-Recognition
AI PROJECT 4
IMAGE ANALYSIS SYSTEM
README Documentation
1. Project Overview
AI Project 4 is an Artificial Intelligence-based Image Analysis System. The system analyzes images using Optical Character Recognition (OCR) and Object Detection. A graphical user interface (GUI) allows the user to select an image and analyze it.
The system can:
•	Read text from images.
•	Detect objects inside images.
•	Display detected text and objects.
•	Save OCR results.
•	Save processed object detection images.

2. Features

2.1 Image Selection
The user can select an image from the computer.
Supported image formats:
•	JPG
•	JPEG
•	PNG
•	BMP

2.2 OCR Text Recognition
The system uses Tesseract OCR to extract text from images.
The extracted text is saved inside:
output/ocr_results/result.txt

2.3 Object Detection
The system uses the MobileNet-SSD deep learning model to detect objects.
Examples include:
•	Person
•	Bird
•	Car
•	Dog
•	Cat
•	Chair
•	Bottle
•	Bicycle
•	Bus
•	Motorcycle
The processed image is saved inside:
output/detected_objects/detected_image.jpg

2.4 Graphical User Interface
The project contains a GUI created using Tkinter.
•	Select Image button
•	Analyze Image button
•	Image preview
•	OCR results
•	Object detection results

3. Technologies Used
•	Python
•	OpenCV
•	Tesseract OCR
•	Pytesseract
•	Pillow
•	Tkinter
•	MobileNet-SSD
•	Caffe Deep Learning Model

4. Project Structure
AI-Project4/
│
├── images/
│   └── text_image.jpg
│
├── models/
│   ├── MobileNetSSD_deploy.caffemodel
│   └── MobileNetSSD_deploy.prototxt
│
├── modules/
│   ├── ocr.py
│   ├── object_detection.py
│   └── image_analysis.py
│
├── output/
│   ├── ocr_results/
│   │   └── result.txt
│   │
│   └── detected_objects/
│       └── detected_image.jpg
│
├── gui.py
├── main.py
├── requirements.txt
└── README.md

5. Installation
Step 1: Check Python
python --version

Step 2: Create a Virtual Environment
python -m venv venv

Step 3: Activate the Virtual Environment
venv\Scripts\Activate.ps1

Step 4: Upgrade pip
python -m pip install --upgrade pip

Step 5: Install Required Libraries
pip install -r requirements.txt

6. Tesseract OCR Installation
Tesseract OCR must be installed separately on Windows. The Tesseract executable path can be configured in the OCR module if required.
pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files\Tesseract-OCR\tesseract.exe"

7. Object Detection Model
The project uses the MobileNet-SSD model. The following files are required:
•	MobileNetSSD_deploy.prototxt
•	MobileNetSSD_deploy.caffemodel
These files must be placed inside:

models/
The model is loaded using OpenCV:
cv2.dnn.readNetFromCaffe()

8. Running the Project
Activate the virtual environment:
venv\Scripts\Activate.ps1
Run the GUI application:
python gui.py

9. Using the Application
1. Click Select Image.
2. Choose an image from your computer.
3. Click Analyze Image.
4. The system performs OCR and object detection.
5. The results are displayed in the GUI.
10. System Workflow

User
 │
 ▼
Select Image
 │
 ▼
Load Image
 │
 ├───────────────┐
 │               │
 ▼               ▼
OCR          Object Detection
 │               │
 ▼               ▼
Extract Text   Detect Objects
 │               │
 └───────┬───────┘
         │
         ▼
   Display Results
         │
         ▼
    Save Results
11. Example Output
============================================================
             AI ANALYSIS RESULT
============================================================

DETECTED TEXT
------------------------------------------------------------

No text detected.

DETECTED OBJECTS
------------------------------------------------------------

- bird

Analysis completed successfully!

12. Project Objectives
•	Understand Artificial Intelligence concepts.
•	Implement OCR technology.
•	Implement object detection.
•	Use deep learning models.
•	Process real-world images.
•	Create a graphical user interface.
•	Combine multiple AI technologies in one application.

13. Future Improvements
•	Voice output
•	Real-time camera detection
•	Video object detection
•	More advanced AI models
•	Face detection
•	Automatic image classification
•	Web-based interface
•	Mobile application
•	Database storage
•	Multi-language OCR support

14. Conclusion
AI Project 4 successfully combines OCR and Object Detection into one complete Image Analysis System. The system can analyze images, extract text, detect objects, and display the results through a graphical user interface. This project demonstrates the practical use of Artificial Intelligence, Computer Vision, Deep Learning, and Python programming.

15. Complete Commands - Step by Step
The following commands explain the complete process for a new user to download, set up, and run the project.

Step 1: Clone the GitHub Repository
git clone YOUR_GITHUB_REPOSITORY_LINK
cd AI-Project4
Replace YOUR_GITHUB_REPOSITORY_LINK with the actual GitHub repository URL.

Step 2: Check Python Installation
python --version

Step 3: Create a Virtual Environment
python -m venv venv

Step 4: Activate the Virtual Environment
Windows PowerShell:
venv\Scripts\Activate.ps1
Windows Command Prompt:
venv\Scripts\activate
macOS / Linux:
source venv/bin/activate

Step 5: Upgrade pip
python -m pip install --upgrade pip

Step 6: Install Project Dependencies
pip install -r requirements.txt

Step 7: Check the Project Structure
Make sure the model files are inside the models folder:
models/
├── MobileNetSSD_deploy.prototxt
└── MobileNetSSD_deploy.caffemodel

Step 8: Configure Tesseract OCR
Make sure the Tesseract OCR executable path is correct in the OCR code:
pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files\Tesseract-OCR\tesseract.exe"

Step 9: Run the Main Image Analysis Program
python main.py

Step 10: Run the GUI Application
python gui.py

Step 11: Use the Application
1. Click Select Image.
2. Choose a JPG, JPEG, PNG, or BMP image.
3. Click Analyze Image.
4. Wait for OCR and Object Detection to finish.
5. View the detected text and objects in the results window.

Step 12: Check Saved Results
OCR results:
output/ocr_results/result.txt
Detected image:
output/detected_objects/detected_image.jpg

Step 13: Deactivate the Virtual Environment
deactivate
Complete Windows Command Sequence
git clone YOUR_GITHUB_REPOSITORY_LINK
cd AI-Project4
python --version
python -m venv venv
venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
python gui.py
Important Notes
•	Do not upload the venv folder to GitHub.
•	Do not upload __pycache__ folders or .pyc files.
•	The MobileNet-SSD model files must be available in the models folder.
•	Tesseract OCR must be installed separately on Windows.
•	If the Tesseract installation path is different, update the path in the OCR module.

![image]()
•	The project requires Python and the required packages listed in requirements.txt.

