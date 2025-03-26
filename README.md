

## DeepAgri - Crop Disease Detection using AI

A Flask-based web application that detects plant diseases (Tomato, Potato, Corn) from uploaded images using CNN models, provides dictionary-based organic tips, with Text-to-Speech (TTS) for user convenience.  


 ## Table of Contents

1. Features
2. Tech Stack  
3. Installation  
4. Usage
5. Project Structure


 ## Features

1. CNN Disease Detection
   - Models for Tomato, Potato, and Corn disease classification.  
   - Upload leaf images, get predicted disease with confidence.

2. Dictionary-Based Organic Tips
   - Hard-coded dictionary for Organic Treatment, Prevention, and Crop Rotation recommendations.  
   - If disease is found, relevant tips are displayed (and translated if needed).

3. Multi-Language Translation  
   - Uses googletrans (https://py-googletrans.readthedocs.io/en/latest/) to translate tips into Hindi, Marathi, Gujarati, or other languages selected by the user.

4. Text-to-Speech  
   - Integrated with ResponsiveVoice (https://responsivevoice.org/) for “Listen” buttons.  
   - Each tip can be spoken aloud, improving accessibility for farmers.


## Tech Stack

- Backend: Python 3, Flask, TensorFlow/Keras for CNN models  
- Frontend: HTML, CSS (Bootstrap), JavaScript  
- TTS: ResponsiveVoice.js (https://responsivevoice.org/) (free/demo version or key)  
- Translation: googletrans (https://py-googletrans.readthedocs.io/en/latest/)  


## Installation

2. Create a virtual environment (recommended):
  
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate


3. Install dependencies:
  
   pip install -r requirements.txt


4. Models:
   - Place your trained CNN models (`tomato_disease_detection.h5`, etc.) in a `models/` folder.
   - Ensure you also have label files (`tomato_disease_labels.txt`, etc.).


 ## Usage

1. Run the Flask app :
 
   python app.py

2. Open your browser at `http://127.0.0.1:5000`.  
3. Upload an image of a leaf (Tomato, Potato, or Corn).  
4. View the predicted disease, confidence score, and dictionary-based tips.  
5. Listen to tips by clicking the “Listen” button (uses ResponsiveVoice).  

---



