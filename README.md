# Laptop Price Predictor App

This project is a Streamlit-based web application that predicts laptop prices using a machine learning model trained on a dataset of approximately 1200 laptops. The application allows users to input various laptop specifications and receive an estimated price based on the trained model.

## Features

* Predicts laptop prices based on multiple hardware specifications.
* Interactive Streamlit interface with dropdowns, sliders, and pill selectors.
* Utilizes a pre-trained machine learning pipeline stored with Joblib.
* Calculates additional features such as pixels per inch (PPI) for more accurate predictions.

## Technologies Used

* Python
* Streamlit
* Scikit-learn
* Joblib
* Pandas
* NumPy

## Project Structure

```
.
├── laptop_app.py         # Main Streamlit application
├── pipe_compressed       # Trained ML model pipeline (Joblib)
├── df                    # Dataset used for dropdown selections
└── README.md
```

## Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the application

```bash
streamlit run laptop_app.py
```

## How the App Works

1. Users select laptop specifications such as company, processor, RAM, GPU, display resolution, storage type, and more.
2. The app converts screen resolution into PPI (Pixels Per Inch), a key feature for price estimation.
3. Specifications are passed into the machine learning pipeline.
4. The model returns an estimated laptop price, rounded to the nearest hundred for clarity.

## Model Information

* The model was trained on real-world laptop data.
* The pipeline includes preprocessing, feature engineering, and regression modeling.
* Important features include CPU type, GPU brand, storage configuration, weight, and PPI.

## Contributing

Contributions are welcome. If you encounter issues or have suggestions, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License.

