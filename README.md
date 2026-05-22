# PlantGuard

PlantGuard is a web-based application designed for the accurate detection and classification of plant diseases. Powered by a deep Convolutional Neural Network (CNN) built with PyTorch, it analyzes leaf imagery to identify up to 39 distinct plant disease classes. 

The system leverages a Flask backend for high-performance inference and provides a streamlined interface for real-time disease identification.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)

## Key Features

- **High-Accuracy Classification**: Utilizes a custom PyTorch CNN architecture optimized for agricultural image classification.
- **Extensive Database**: Trained to detect and classify 39 different plant diseases and healthy crop states.
- **Local Inference**: All image processing and model inference are handled locally to ensure data privacy and minimal latency.
- **Responsive Interface**: A clean, intuitive web UI designed for straightforward image uploads and instantaneous result delivery.

## Architecture

The system operates via a standard client-server architecture:

1. **Client**: A browser-based frontend where users can upload or capture plant imagery.
2. **Backend**: A Flask API that handles image preprocessing (resizing, normalization).
3. **Inference Engine**: The PyTorch model receives the processed tensor, performs inference, and returns the predicted class along with a confidence score.

## Getting Started

### Prerequisites

Ensure the following dependencies are installed on your system:
- Python 3.8 or higher
- Git

### Installation

1. Clone the repository:
```bash
git clone https://github.com/mayankdl03/PlantGuard.git
cd PlantGuard
```

2. Create and activate a virtual environment (recommended):
```bash
python -m venv venv

# On Windows:
venv\Scripts\activate

# On macOS and Linux:
source venv/bin/activate
```

3. Install the required Python packages:
```bash
pip install -r requirements.txt
```

### Usage

1. Start the Flask development server:
```bash
python app.py
```

2. Open your web browser and navigate to:
```
http://localhost:5000
```

3. Upload an image of a plant leaf through the web interface to receive an instant disease prediction and confidence metric.

## Screenshots

<details>
<summary>Click to view system interface</summary>

**Homepage**  
<img src="https://github.com/user-attachments/assets/851873b4-a1cc-493f-af14-32e545263df8" alt="Homepage" width="800"/>

**Analysis Interface**  
<img src="https://github.com/user-attachments/assets/f7a585a4-dc94-484f-ac14-fec4809a0f16" alt="Analysis Interface" width="800"/>

</details>

## Contributing

Contributions are welcome. Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature-name`).
3. Commit your changes (`git commit -m 'Add your feature'`).
4. Push to the branch (`git push origin feature/your-feature-name`).
5. Open a Pull Request for review.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
