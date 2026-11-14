# Deep Learning Projects

A collection of deep-learning practice work, including a handwritten-digit recognition application.

## Featured: Handwritten Digit Recognition

This project uses a convolutional neural network (CNN) to classify a handwritten digit from an image. A Flask application serves the interface and prediction endpoint.

### How it works

1. The user submits a drawing as an image.
2. The application decodes the image and converts it to grayscale.
3. The image is resized to 28 × 28 pixels and preprocessed.
4. The trained CNN predicts one of the digits from 0 to 9.
5. The application returns the predicted digit.

## Tech stack

- Python
- Keras
- NumPy
- Pillow
- Flask
- Jupyter Notebook

## Run locally

1. Clone the repository:
   ```bash
   git clone https://github.com/SandhyaRani1518/DL-projects.git
   cd DL-projects
   ```
2. Create and activate a virtual environment.
3. Install the dependencies used by the application:
   ```bash
   pip install flask keras numpy pillow
   ```
4. Make sure `model_cnn.h5` is in the project root.
5. Start the app:
   ```bash
   python app.py
   ```

Open the local address printed by Flask in your browser.

## Repository contents

- `HANDWRITTEN RECG.ipynb` — handwritten-digit recognition notebook.
- `app.py` — Flask application and prediction endpoint.
- `model_cnn.h5` — saved CNN model.
- `templates/` and `static/` — web interface assets.
- `NumPy_Full_Course.ipynb` — NumPy learning notebook.

This is an educational project, not a production-ready inference service. Review and update dependencies for your local Python and Keras versions if needed.
