# Decision Support System for Precision Crop Recommendation

[![Python](https://img.shields.io/badge/Python-3.7%2B-blue.svg)](https://www.python.org/)
[![Framework](https://img.shields.io/badge/Framework-Flask-brightgreen.svg)](https://flask.palletsprojects.com/)
[![ML](https://img.shields.io/badge/ML%20Library-Scikit--learn-orange.svg)](https://scikit-learn.org/)

A Machine Learning-Based Decision Support System for Precision Crop Recommendation in Smart City Urban Agriculture. This project provides a web-based application to help users find the most suitable crop to grow based on environmental factors.

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Key Features](#-key-features)
- [Project Structure](#-project-structure)
- [Dataset](#-dataset)
- [Machine Learning Model](#-machine-learning-model)
- [Technologies Used](#-technologies-used)
- [Setup and Installation](#-setup-and-installation)
- [How to Run](#-how-to-run)
- [Showcase & Documentation](#-showcase--documentation)
- [Academic Context](#-academic-context)
- [Contributing](#-contributing)
- [License](#-license)

---

## Overview

This project is a **Decision Support System** designed to tackle challenges in urban agriculture within smart cities. By leveraging machine learning, it analyzes various environmental parameters to provide precise crop recommendations. This helps in optimizing resource usage, increasing yield, and promoting sustainable farming practices.

The core of the project is a machine learning model trained on a comprehensive dataset of soil and climate data. This model is deployed as a user-friendly web application using the **Flask** framework.

---

## 🚀 Key Features

-   **Intelligent Crop Recommendation:** Utilizes a trained machine learning model to predict the most suitable crop.
-   **Web-Based Interface:** An easy-to-use web application (built with Flask and HTML) for users to input their environmental data.
-   **Data-Driven Insights:** The model is trained on key agricultural parameters for accurate predictions.
-   **Scalable Preprocessing:** Includes saved data scalers (`standscaler.pkl`, `minmaxscaler.pkl`) for consistent preprocessing of new user inputs.

---

## 📂 Project Structure

Here is an overview of the key files and directories in this repository:

```
├── static/                   # CSS, JS, and image files for the web app
├── templates/                # HTML files for the Flask web application
│   └── index.html            # Main page for user input
├── app.py                    # The Flask application backend
├── Crop Recommendation Using Machine Learning.ipynb  # Jupyter Notebook with data analysis, preprocessing, and model training
├── Crop_recommendation.csv   # The dataset used for training
├── model.pkl                 # The saved, pre-trained machine learning model
├── minmaxscaler.pkl          # Saved MinMax scaler object
├── standscaler.pkl           # Saved StandardScaler object
├── Project_Report.pdf        # (Placeholder for your report)
├── Video_Demo.mp4            # (Placeholder for your video)
├── Presentation.ppt          # (Placeholder for your presentation)
├── *.pdf                     # Research papers and project documentation
└── README.md                 # This file
```

---

## 📊 Dataset

The model is trained on the `Crop_recommendation.csv` dataset. This dataset contains 2200 instances and 8 features (columns) that are crucial for determining an optimal crop.

The features included are:
-   **N:** Ratio of Nitrogen content in soil
-   **P:** Ratio of Phosphorous content in soil
-   **K:** Ratio of Potassium content in soil
-   **temperature:** Temperature in degrees Celsius
-   **humidity:** Relative humidity in %
-   **ph:** pH value of the soil
-   **rainfall:** Rainfall in mm
-   **label:** The target variable, representing the crop (e.g., 'rice', 'maize', 'coffee', etc.)

---

## 🤖 Machine Learning Model

The complete workflow for data analysis, exploratory data analysis (EDA), feature engineering, and model training is detailed in the `Crop Recommendation Using Machine Learning.ipynb` Jupyter Notebook.

Several classification algorithms were likely evaluated, and the best-performing model was saved as `model.pkl` for deployment in the Flask app.

**(Note to owner: You should specify which model was selected, e.g., "The final model selected was a Random Forest Classifier, which achieved an accuracy of XX%.")**

---

## 💻 Technologies Used

-   **Backend:** Python, Flask
-   **Data Science & ML:** Scikit-learn, Pandas, NumPy
-   **Frontend:** HTML (served via Flask templates)
-   **Environment:** Jupyter Notebook

---

## ⚙️ Setup and Installation

To run this project locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/harshita0212/Decision-Support-System-for-Precision-Crop-Recommendation-in-Smart-City-.git](https://github.com/harshita0212/Decision-Support-System-for-Precision-Crop-Recommendation-in-Smart-City-.git)
    cd Decision-Support-System-for-Precision-Crop-Recommendation-in-Smart-City-
    ```

2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the required libraries:**
    *This project does not include a `requirements.txt` file. Based on the files, you will need the following libraries. You can create a `requirements.txt` file and add them.*
    ```bash
    pip install Flask pandas numpy scikit-learn
    ```

---

## ▶️ How to Run

There are two main components to run: the Jupyter Notebook and the Flask web app.

### 1. Run the Jupyter Notebook

If you want to explore the data analysis and model training process:
```bash
jupyter notebook "Crop Recommendation Using Machine Learning.ipynb"
```

### 2. Run the Flask Web Application

To start the decision support system:
```bash
python app.py
```
This will start a local server. Open your web browser and navigate to:
[http://127.0.0.1:5000/](http://127.0.0.1:5000/)

You will see the web interface where you can input the environmental parameters to get a crop recommendation.

---

## 💡 Showcase & Documentation

This repository also contains the complete documentation and demonstration of the project:

-   **📄 Project Report:** (e.g., `Project_Report.pdf`) - A detailed report outlining the project's objectives, methodology, results, and conclusions.
-   **📽️ Video Demonstration:** (e.g., `Video_Demo.mp4`) - A video walkthrough of the web application, showing how to use it and its key features.
-   **Presentation:** (e.g., `Presentation.ppt`) - A slide deck summarizing the project, suitable for presentations.

*(Note: Please update the file paths and names in this section and in the "Project Structure" section once you add the files.)*

---

## 📜 Academic Context

The findings and methodology of this project were part of a research paper submitted to an IEEE International Conference. The relevant documentation and submission files (e.g., `SmartCities_Paper_Submitted_IEEE...pdf`) are included in this repository.

---

## 🤝 Contributing

Contributions are welcome! If you have suggestions for improvements, please feel free to fork the repository and submit a pull request.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

---

## 📄 License

This project is open-source. Please add a license file to define how others can use your work.
**(Note to owner: You should add a `LICENSE` file. The [MIT License](https://choosealicense.com/licenses/mit/) is a popular and permissive choice.)**

```
