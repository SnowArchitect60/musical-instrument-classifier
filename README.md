# Musical Instrument Classifier (MIC)
This is a computer vision + machine learning project trained using the FastAI `resnet18` CNN model to classify 47 musical instruments based on images.

### 📌 Project Summary
This project demonstrates the use of deep learning to classify musical instruments from images. Despite class imbalance and visual similarity between instruments, the model achieved strong accuracy with minimal confusion.

### ✅ Features
- Recognizes 47 musical instruments across 6 categories:
      -🎻 Stringed instruments: e.g., acoustic guitar, violin, cello, harp
      -🎹 Keyboard instruments: e.g., piano, organ, synthesizer
      -🎺 Brass instruments: e.g., trumpet, tuba, french horn
      -🎷 Woodwind instruments: e.g., flute, clarinet, saxophone
      -🥁 Percussion instruments: e.g., drum set, cymbals, marimba
      -🎛️ Miscellaneous: microphone, theremin, DJ controller, etc.
- Trained with ResNet18 and fine-tuned over 10 epochs
- Interactive prediction interface via image upload in Colab
- Includes top-3 prediction chart and natural language output
- Data collected using DuckDuckGo Search API

### 📊 Model Performance
------------------------------
| Metric          | Value    |
| --------------- | -------- |
| Training Loss   | ≈ 0.0448 |
| Validation Loss | ≈ 0.5377 |
| Error Rate      | ≈ 12.62% |
| Accuracy        | ≈ 87.38% |
| Classes (total) |    47    |
------------------------------

### 📁 Files
- `musical_instrument_classifier.ipynb` – Google Colab notebook
- `musical_instrument_classifier_resnet18.pkl` – Trained model
- `confusion_matrix.png` – Visualization of class performance

### 🔧 Tools
- Python
- fastai / PyTorch
- resnet18
- DuckDuckGo API (for image scraping)
- Matplotlib / ipywidgets
- Google Colab

### ⚠️ Limitations
- Unconventional or niche instruments may produce inaccurate predictions.
- Visually complex instruments (e.g., flamed-top guitars) may confuse the model.
- The model is based on resNet18; performance can improve using resnet34 or resnet50.
- No data cleaning performed.

### 📌 Future Improvements
- Retrain with deeper CNNs (resnet34 or resnet50)
- Clean and balance the dataset more evenly
- Add more instrument types and non-standard angles/backgrounds

### 📄 License
This project is licensed under the MIT License.
