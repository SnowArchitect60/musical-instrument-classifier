# Musical Instrument Classifier (MIC)
This is a computer vision + machine learning project trained using the FastAI `resnet152` CNN model to classify 54 musical instruments based on images.

### 📌 Project Summary
This project demonstrates the use of deep learning to classify musical instruments from images. Despite class imbalance and visual similarity between instruments, the model achieved strong accuracy with minimal confusion.

### ✅ Features
- Recognizes 54 musical instruments across 6 categories (stringed, keyboard, brass, woodwind, percussion, and miscellaneous instruments).
- Data collected (~1000 images per instrument) using DuckDuckGo Search API.
- Trained with `resnet152` and fine-tuned over 10 epochs of augmented data.
- Interactive prediction interface via image upload in Colab.
- Includes top-3 prediction chart and natural language output.

### 📊 Current Model Performance (v1.0.a)
------------------------------
| Metric          | Value    |
| --------------- | -------- |
| Training Loss   | ≈ 0.4146 |
| Validation Loss | ≈ 1.4144 |
| Error Rate      | ≈ 31.56% |
| Accuracy        | ≈ 68.44% |
| Classes (total) |    54    |
------------------------------

### 📁 Files
- `musical_instrument_classifier.ipynb` – Google Colab notebook.
- `musical_instrument_classifier_resnet18.pkl` – Trained model (v0.5.a).
- `musical_instrument_classifier_resnet152.pkl` – Trained model (v1.0.a).
- `confusion_matrix_resnet18.png` – Class performance visualization of the model pre-trained with resnet18.
- `confusion_matrix_resnet152_v1.png` – Class performance visualization of the model pre-trained with resnet152.
- `top_losses_resnet152.png` – Top losses list of the model pre-trained with resnet152.

### 🔧 Tools
- Python
- fastai / PyTorch
- resnet152
- DuckDuckGo API (for image scraping)
- Hashlib (for duplicate scraped images)
- Pathlib and PIL (for corrupt/unsupported image file handling)
- Matplotlib / ipywidgets
- Google Colab

### ⚠️ Limitations
- Unconventional or niche instruments may produce inaccurate predictions.
- Visually complex instruments may confuse the model or provide accurate but relatively unconfident results.
- The accuracy and generalization performance of the model suffer due to the intrinsic disadvantage of having a general dataset.

### 📌 Future Improvements
- Expand the training dataset strategically by providing special queries highlighting the qualities specific to each instrument. (v0.5.b)
- Add more instrument types, non-standard angles, and backgrounds. (v1.0.b)
- Include Gradio or HuggingFace for the model's UI application. (v1.0)

### 📈 Update Log
- MIC model trained using `resnet152` (v1.0.a). Data cleaning and augmentation performed.
- MIC model trained using `resnet18` (v0.5.a). No data cleaning and augmentation.

### 📄 License
- This project is licensed under the MIT License.
