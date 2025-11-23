# Aerial-Object-Classification-Detection
Aerial image classifier (Bird vs Drone) using CNN and Transfer Learning. MobileNet achieved 99.07% accuracy. Deployed with Streamlit

📌 Project Overview

This project develops an AI system for aerial surveillance to distinguish between birds and drones, useful for:
- Wildlife Protection
- Security & Defense Surveillance
- Airport Bird-Strike Prevention
- Environmental Research

 📊 Dataset

-Training: 2,662 images (Bird: 1,414 | Drone: 1,248)
- Validation: 442 images (Bird: 217 | Drone: 225)
- Test: 215 images (Bird: 121 | Drone: 94)
- Image Size: 224×224 pixels
  
 🛠️ Technologies

- Python 3.x
- TensorFlow/Keras
- Transfer Learning (ResNet50, MobileNet, EfficientNetB0)
- Streamlit for deployment

🚀 Workflow

1. Understand Dataset - Explored and visualized data
2. Data Preprocessing - Normalized and resized images
3. Data Augmentation - Rotation, flipping, zoom, brightness, cropping
4. Model Building - Custom CNN + 3 Transfer Learning models
5. Model Training - Trained with EarlyStopping & ModelCheckpoint
6. Model Evaluation - Confusion matrix, classification report
7. Model Comparison - Compared accuracy and training time
8. Streamlit Deployment - Interactive web app


 📈 Results

| Model | Accuracy | Precision | Recall | F1-Score | Time |
|-------|----------|-----------|--------|----------|------|
| Custom CNN | 90.70% | 90.22% | 88.30% | 89.25% | 12.96 min |
| ResNet50 | 78.14% | 86.15% | 59.57% | 70.44% | 13.30 min |
| **MobileNet** | **99.07%** | **100.00%** | **97.87%** | **98.92%** | **7.05 min** |
| EfficientNetB0 | 56.28% | 0.00% | 0.00% | 0.00% | 5.16 min |

 🏆 Best Model: MobileNet (99.07% accuracy)

📁 Project Structure

├── README.md                    # Documentation
├── requirements.txt             # Dependencies
├── AERIAL_OBJECT.ipynb          # Training notebook
├── app.py                      # Streamlit app
└── best_model.keras            # Trained model


🎯 Usage

1. Run Streamlit app: `streamlit run app.py`
2. Upload bird or drone image
3. Click "Classify Image"
4. View prediction and confidence

📝 Deliverables

✅ Trained models (Custom CNN, Transfer Learning)  
✅ Streamlit app for classification  
✅ Scripts & notebooks for preprocessing, training, evaluation  
✅ Model comparison report  
✅ GitHub repository with documentation  
✅ Well-structured, commented code

