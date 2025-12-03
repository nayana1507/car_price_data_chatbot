# Car Price Data ChatBot 🚗💬

This project features a rule-based chatbot that provides interactive querying of a used car dataset. It allows users to ask natural language questions about car models, prices, mileage, and specifications.

## 📖 Overview

The core of this project is the `chatbot_carprice.ipynb` Jupyter Notebook, which performs data cleaning and manipulation using **Pandas** and exposes the data through a user-friendly conversational interface built with **Gradio**.

### Key Features
* **Data Querying:** Answer questions about specific car models (e.g., "selling price of swift").
* **Comparative Analysis:** Find the highest/lowest selling price or most/least driven cars.
* **Filtering:** List cars by **Fuel Type** (Petrol/Diesel), **Transmission** (Manual/Automatic), **Manufacturing Year**, and **Owner** category (First-hand, Second-hand, etc.).
* **Interactive Interface:** The bot is launched locally using Gradio's chat interface.

## 🛠️ Setup and Requirements

### Dependencies

This project requires Python 3.x and the following libraries:

| Library | Purpose |
| :--- | :--- |
| **pandas** | Data loading, cleaning, and filtering. |
| **gradio** | Creating the web-based chatbot interface. |

### Data Source

The notebook requires a file named `cardata.csv`. The notebook loads this file, performs a cleaning step (dropping index 100 to 200), and saves a modified version as `cleaned_car_data.csv`.

## ▶️ How to Run

1.  **Clone the repository** (or ensure you have the files, including `cardata.csv` and `chatbot_carprice.ipynb`).
2.  **Install dependencies** using the provided `requirements.txt`:

    ```bash
    pip install -r requirements.txt
    ```

3.  **Launch the Jupyter Notebook** and run all cells sequentially:

    ```bash
    jupyter notebook chatbot_carprice.ipynb
    ```

4.  The final cell will launch the Gradio ChatBot interface in your browser (usually at a local URL like `http://127.0.0.1:7861/`).

## ❓ Example Queries

You can ask the chatbot questions such as:

* "highest selling price"
* "selling price of ciaz"
* "most driven diesel car"
* "cars after 2016"
* "fuel type of swift"
