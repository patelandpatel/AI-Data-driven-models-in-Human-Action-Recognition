# AI Data-Driven Models in Human Action Recognition

This repository implements a **Human Action Recognition System** by leveraging deep learning techniques for video classification. The system identifies human actions in videos by combining **Convolutional Neural Networks (CNNs)** for extracting spatial features and **Long Short-Term Memory (LSTM)** networks for analyzing temporal relationships between frames.

The project achieves an **84% accuracy** in detecting specific actions, such as "hitting children themselves", "hitting children other", "They are just playing not hiting".
---
## Project Overview   

Human Action Recognition is a critical task in computer vision with applications in surveillance, video analysis, and human-computer interaction. This project integrates CNN and LSTM to classify human actions effectively:
- **CNNs** process each video frame to extract spatial features.
- **LSTMs** capture temporal relationships between frames, enabling action classification.

### Key Features
- **Video Classification:** Classifies human actions based on spatial and temporal data.
- **Action Detection:** Specifically tuned for detecting harmful actions like "hitting children themselves."
- **Deep Learning Models:** Combines CNNs for spatial feature extraction and LSTMs for temporal feature analysis.

---

## Getting Started

### Prerequisites

Ensure you have the following installed:
- Python 3.8+
- TensorFlow/Keras
- NumPy
- OpenCV
- Matplotlib
- Pandas

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/AI-Data-driven-models-in-Human-Action-Recognition.git
   cd AI-Data-driven-models-in-Human-Action-Recognition
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Prepare your dataset:
   - Place video files in the `data/` folder.
   - Use the provided preprocessing script to prepare the data:
     ```bash
     python preprocess_data.py
     ```

---

## Usage

### Training the Model

1. Train the CNN model for spatial feature extraction:
   ```bash
   python train_cnn.py
   ```

2. Train the LSTM model for temporal analysis:
   ```bash
   python train_lstm.py
   ```

3. Combine both models for end-to-end training:
   ```bash
   python train_har_system.py
   ```

### Testing the Model

Test the trained model on a video:
```bash
python test_model.py --video_path path_to_video
```

---

## Project Structure

```
AI-Data-driven-models-in-Human-Action-Recognition/
├── data/                  # Dataset and related files
├── models/                # Pre-trained models and checkpoints
├── src/                   # Source code for training, testing, and preprocessing
├── results/               # Results such as performance metrics and logs
├── requirements.txt       # Required Python libraries
└── README.md              # Project overview
```

---

## Results

- **Accuracy:** 84% in detecting specific actions like "hitting children themselves."
- **Performance Metrics:** Loss and accuracy graphs are generated during training.

---

## Future Work

- Improve model accuracy for detecting more complex actions.
- Expand the dataset to include diverse actions.
- Optimize the model for real-time video analysis.

---

## Contributing

Contributions are welcome! Follow these steps:
1. Fork this repository.
2. Create a new branch for your feature:
   ```bash
   git checkout -b feature-branch-name
   ```
3. Commit and push your changes:
   ```bash
   git commit -m "Description of changes"
   git push origin feature-branch-name
   ```
4. Submit a pull request.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Contact

For more information, feel free to reach out via email at [your_email@example.com] or visit the [project page](https://github.com/yourusername/AI-Data-driven-models-in-Human-Action-Recognition).
