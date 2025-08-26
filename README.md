🚗 Vehicle Damage Detection

A deep learning project that detects and classifies vehicle damage using Transfer Learning with ResNet. The model achieves ~80% accuracy in predicting six different damage categories.

📊 Project Overview

This project uses ResNet (transfer learning) to classify vehicle images into six categories of damage:

class_names = [
    'Front Breakage',
    'Front Crushed',
    'Front Normal',
    'Rear Breakage',
    'Rear Crushed',
    'Rear Normal'
]



The goal is to provide an AI-powered system that can assist insurance companies, workshops, and customers in quickly assessing the type and extent of vehicle damage from images.

✅ Features

🧠 Transfer Learning with ResNet architecture

🔎 Detects front and rear damage conditions

📈 Achieved 80% accuracy on test data

🖥️ Includes a Streamlit app for easy image upload and prediction

📒 Jupyter notebook for training, evaluation, and experimentation

🖼 Example Prediction

Below is a screenshot of the Streamlit app classifying a vehicle image as Rear Crushed:


⚙️ Installation
# Clone the repository
git clone https://github.com/Mohamed-Elguindy/Vehicle-Damage-Detection.git
cd Vehicle-Damage-Detection

# (Optional) create virtual environment
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt


🚀 Usage
🔹 1. Jupyter Notebook

Run the notebook for training and evaluation:

jupyter notebook damage_predication.ipynb

🔹 2. Streamlit App

Launch the web app for interactive predictions:

cd streamlit-app
streamlit run app.py


Upload a car image, and the model will predict the damage type.

📂 Folder Structure
Vehicle-Damage-Detection/
├── damage_predication.ipynb     # Training & evaluation notebook
├── saved_model.pth              # Pre-trained ResNet model
├── streamlit-app/               # Streamlit web app
│   └── app.py
├── images/                      # Demo photos 
│   └── demo.png
└── requirements.txt             # Dependencies


📊 Results

Model: ResNet (Transfer Learning)

Accuracy: ~80%

Classes: 6 damage categories

Frameworks: PyTorch, TorchVision, Streamlit

🔮 Future Work

Improve dataset size & diversity for better generalization

Add bounding box localization for precise damage area detection

Deploy Streamlit app with Docker or Hugging Face Spaces

Integrate with insurance claim systems

📜 License

This project is licensed under the MIT License – feel free to use and modify.
