
# Color Vision Classifier and Simulator

This project provides a tool to classify the type of color blindness a user has and simulate how images appear to them based on their condition. It aims to raise awareness and help colorblind individuals better understand their vision.

## Features
- **Classification**: Identify the type of color blindness using an AI-based classifier.
- **Simulation**: Upload images and see how they appear with your type of color blindness.
- **Interactive Interface**: User-friendly interface for testing and image simulation.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Setsofia-lab/CNN_ColourBlindPerception.git
   cd color-vision-simulator

Install dependencies:
 pip install -r requirements.txt


Run the app locally:
 python app.py


Usage
Access the interface at http://localhost:5000.
Take the test to classify your type of color blindness.
Upload an image to see its simulation based on the results.
Data Sources
The classification model is trained on synthetic Ishihara test data and other color blindness datasets. For more details, refer to the Data section.
Future Work
Improve classification model with more real-world data.
Integrate support for live video simulation.
License
MIT License

---

### **5. Data Sources and Preprocessing**
#### **Data Sources**:
- **Ishihara Test Dataset**: Generate synthetic test images using OpenCV or download existing datasets.
- **Color Blindness Simulation Standards**:
  - [Coblis](https://www.color-blindness.com/coblis-color-blindness-simulator/): Learn about color transformation standards.
  - Public datasets like Kaggle’s color blindness datasets.

#### **How to Work with Image Data**:
1. **Image Collection**:
   - Gather diverse datasets with known ground truth for color blindness types.
   - Include RGB images for simulation.

2. **Preprocessing**:
   - Resize images to a consistent shape (e.g., 224x224 for CNNs).
   - Normalize pixel values to [0, 1] for neural network input.
   - Augment data with brightness/contrast variations for robustness.

3. **Color Blind Simulation Pipeline**:
   - Adjust RGB channels to simulate Protanopia, Deuteranopia, and Tritanopia.
   - Validate with tools like Coblis for accuracy.

