# Handwritten Digit Recognition

A small deep-learning web application that accepts a user-drawn digit and returns a CNN prediction for one of the classes 0–9.

## How it works

1. The user draws a digit in the browser.
2. The frontend sends the drawing image to a Flask endpoint.
3. The application decodes the image, converts it to grayscale, and resizes it to 28 × 28 pixels.
4. The saved Keras CNN model predicts the digit.
5. The application returns the predicted class to the frontend.

## Tech stack

- Python
- Flask
- Keras
- NumPy
- Pillow
- HTML, CSS, and JavaScript

## Run locally

1. Clone the repository:

   ```bash
   git clone https://github.com/SandhyaRani1518/DL-projects.git
   cd DL-projects
   ```

2. Create and activate a virtual environment.

3. Install dependencies:

   ```bash
   python -m pip install --upgrade pip
   pip install -r requirements.txt
   ```

4. Ensure `model_cnn.h5` is in the project root.

5. Start the Flask application:

   ```bash
   python app.py
   ```

6. Open the local address printed by Flask in your browser.

## Repository contents

- `app.py` — Flask application and prediction endpoint.
- `model_cnn.h5` — saved CNN model.
- `HANDWRITTEN RECG.ipynb` — handwritten-digit recognition notebook.
- `templates/` and `static/` — web interface files.
- `NumPy_Full_Course.ipynb` — NumPy learning notebook.
- `requirements.txt` — Python package dependencies.

## Notes

This is an educational demonstration, not a production inference service. The Flask application currently runs with debug mode enabled in the source; keep it restricted to local development and do not deploy it with debug mode enabled. Model compatibility may depend on the installed Keras / TensorFlow versions.

Predictions from this project are model outputs for handwritten digit images; they are not claims of a measured accuracy unless supported by a separate evaluation.