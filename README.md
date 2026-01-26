# Machine Learning Internship Tasks

## 📋 Overview
This repository contains two complete machine learning projects developed for an internship:
1. **Email Spam Classification System** - Interactive dashboard for spam detection
2. **MNIST Digit Recognition System** - Image-based digit classification with web interface

Both projects feature complete machine learning pipelines, interactive web interfaces, and comprehensive evaluation metrics.

---

## 🚀 Quick Start

### Prerequisites
```bash
pip install pandas numpy scikit-learn tensorflow keras matplotlib seaborn
pip install gradio pillow ipywidgets
```

### Running the Projects

#### Option 1: Run in Google Colab
Simply upload the notebook to Google Colab and run all cells.

#### Option 2: Run Locally
```bash
# For Spam Classification
python -m notebook # Open and run spam classification cells

# For Digit Recognition
python -m notebook # Open and run MNIST classification cells
```

---

## 📧 Project 1: Email Spam Classification System

### 🎯 Objective
Build an interactive system to classify emails as spam or not spam using machine learning with real-time predictions.

### 📊 Dataset
- **File**: `emails.csv`
- **Samples**: 5,172 emails
- **Features**: 3,000 word count features
- **Labels**: Binary (0 = Not Spam, 1 = Spam)

### 🔧 Technical Implementation

#### Data Processing
- Automatic feature extraction from word counts
- Binary label conversion (0/1)
- Stratified train-test split (80/20)
- CountVectorizer for text feature extraction

#### Model Architecture
- **Algorithm**: Logistic Regression
- **Optimization**: L2 regularization
- **Max Iterations**: 1000 for convergence
- **Random State**: 42 for reproducibility

#### Interactive Features
1. **Text Input**: Direct email text input
2. **File Upload**: Support for .txt and .eml files
3. **Real-time Prediction**: Instant spam/not spam classification
4. **Confidence Scores**: Probability of spam prediction
5. **Word Analysis**: Highlight influential words in decision

### 📈 Performance Metrics
| Metric | Value |
|--------|-------|
| Accuracy | 98.26% |
| Precision | 95.78% |
| Recall | 98.33% |
| F1-Score | 97.04% |

### 🎮 User Interface Components
- **TextArea**: For manual email input
- **FileUpload**: For .txt/.eml file uploads
- **Predict Button**: Triggers classification
- **Output Display**: Shows results with confidence
- **Word Highlighting**: Displays influential words

### 🔍 Key Features
- Real-time spam detection
- File upload support (.txt, .eml)
- Detailed classification explanation
- Error handling for invalid inputs
- Visual feedback during processing

---

## 🔢 Project 2: MNIST Digit Recognition System

### 🎯 Objective
Create a machine learning system to recognize handwritten digits (0-9) from images with a user-friendly interface.

### 📊 Dataset
- **Source**: Keras MNIST dataset
- **Training Samples**: 60,000 images
- **Testing Samples**: 10,000 images
- **Image Size**: 28×28 pixels (grayscale)

### 🔧 Technical Implementation

#### Image Preprocessing
- Pixel normalization (0-255 → 0-1)
- Image flattening (28×28 → 784 features)
- Grayscale conversion
- Automatic resizing to 28×28

#### Model Architecture
- **Algorithm**: Logistic Regression
- **Input Shape**: 784 features (flattened images)
- **Classes**: 10 (digits 0-9)
- **Training**: 1000 iterations for convergence

#### Interactive Features
1. **Image Upload**: PNG/JPG file upload
2. **Real-time Prediction**: Instant digit classification
3. **Visual Display**: Shows uploaded image
4. **Error Handling**: Invalid image feedback

### 📈 Performance Metrics
| Metric | Value |
|--------|-------|
| Overall Accuracy | 92.64% |
| Best Class (Digit 1) | 97% F1-score |
| Worst Class (Digit 5/8) | 88% F1-score |
| Macro Average | 92.6% |

### 🎮 User Interface Components
- **FileUpload**: For image uploads (PNG/JPG)
- **Predict Button**: Triggers digit recognition
- **Image Display**: Shows uploaded digit
- **Result Display**: Shows predicted digit

### 🔍 Key Features
- Handwritten digit recognition
- Image upload interface
- Real-time predictions
- Support for various image formats
- Robust error handling

---

## 🏗️ Project Structure

```
ARCH_ML_Internship_Tasks.ipynb
│
├── Spam Classification Section
│   ├── Data Loading & Preprocessing
│   ├── Model Training (Logistic Regression)
│   ├── Performance Evaluation
│   ├── Interactive Dashboard
│   └── File Upload System
│
├── Digit Recognition Section
│   ├── MNIST Data Loading
│   ├── Image Preprocessing
│   ├── Model Training
│   ├── Model Evaluation
│   └── Image Prediction Interface
│
└── Utility Functions
    ├── Email preprocessing
    ├── Image preprocessing
    ├── Prediction functions
    └── Visualization helpers
```

---

## 🛠️ Technologies Used

### Core Libraries
- **Pandas & NumPy**: Data manipulation
- **Scikit-learn**: Machine learning algorithms
- **TensorFlow/Keras**: Deep learning framework
- **Matplotlib & Seaborn**: Data visualization

### Interface & Utilities
- **IPyWidgets**: Interactive widgets
- **PIL/Pillow**: Image processing
- **Gradio**: Web interface (alternative)
- **Email Parser**: .eml file processing

### Development Environment
- **Google Colab**: Cloud-based execution
- **Jupyter Notebook**: Interactive development
- **Python 3.8+**: Programming language

---

## 📋 Installation Requirements

### For Spam Classification
```python
pip install pandas scikit-learn matplotlib seaborn
pip install ipywidgets pillow email
```

### For Digit Recognition
```python
pip install tensorflow keras scikit-learn
pip install pillow ipywidgets matplotlib
```

### Complete Requirements
```txt
pandas==1.5.0
numpy==1.24.0
scikit-learn==1.3.0
tensorflow==2.13.0
keras==2.13.0
matplotlib==3.7.0
seaborn==0.12.0
ipywidgets==8.0.0
pillow==10.0.0
```

---

## 🚀 How to Use

### For Spam Classification
1. Run all cells in the notebook
2. Scroll to the interactive interface
3. Enter email text or upload a file
4. Click "Predict Spam" for results

### For Digit Recognition
1. Run all cells in the notebook
2. Scroll to the image interface
3. Upload a handwritten digit image
4. Click "Predict Digit" for results

---

## 📊 Model Performance Summary

### Spam Classification
- **High Accuracy**: 98.26% on test set
- **Low False Positives**: 95.78% precision
- **High Recall**: 98.33% spam detection
- **Balanced Performance**: 97.04% F1-score

### Digit Recognition
- **Good Accuracy**: 92.64% on MNIST test
- **Consistent Performance**: Similar across digits
- **Fast Inference**: Real-time predictions
- **Robust**: Handles various image qualities

---

## 🎯 Key Features & Innovations

### Spam Classifier
✅ **Interactive Dashboard**: User-friendly interface  
✅ **Multiple Input Methods**: Text & file upload  
✅ **Explainable AI**: Shows influential words  
✅ **File Support**: .txt and .eml formats  
✅ **Real-time Feedback**: Instant predictions  

### Digit Recognizer
✅ **Image Processing**: Automatic preprocessing  
✅ **User Interface**: Simple image upload  
✅ **High Accuracy**: 92.64% on MNIST  
✅ **Error Handling**: Invalid image feedback  
✅ **Visual Results**: Shows image with prediction  

---

## 🔮 Future Enhancements

### Spam Classification
- Add neural network models for better performance
- Implement real-time email scanning
- Add multilingual support
- Create Chrome extension for Gmail

### Digit Recognition
- Implement CNN for improved accuracy
- Add drawing canvas for direct input
- Support for multi-digit images
- Deploy as web application

---

## 📝 Notes

1. **Dataset**: Both projects use standard datasets (emails.csv and MNIST)
2. **Performance**: Models show production-ready performance
3. **Scalability**: Code is modular and easily extendable
4. **Documentation**: Comprehensive comments and explanations

---

## 📞 Contact & Support

For questions or issues:
- Check the notebook comments for implementation details
- Review the model evaluation sections for performance metrics
- Test with provided sample inputs for verification

---

## 📄 License

This project is for educational purposes as part of a machine learning internship. All code is provided as-is for learning and demonstration.

---

## ⭐ Acknowledgments

- Kaggle for the spam dataset
- TensorFlow/Keras for MNIST dataset
- Scikit-learn for machine learning algorithms
- Google Colab for cloud computing resources

---

**Last Updated**: January 2024  
**Status**: Complete & Production-Ready
