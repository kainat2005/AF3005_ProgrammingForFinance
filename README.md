# Smart Financial Management System

## 📌 Overview
This project is a **Smart Financial Management System** developed as part of the AF3005 - Programming for Finance course assignment. The system utilizes `ipywidgets` to create an interactive stock price tracker that processes stock prices, skips missing data, and stops tracking when a target price is reached (PKR 200).

## 🛠 Features
- **Interactive input using `ipywidgets`** for real-time stock price tracking.
- **Handles missing stock data** by skipping `None` values.
- **Stops tracking** once the stock price reaches PKR 200.
- **User-friendly interface** for seamless interaction.
- **Real-time alerts** when conditions are met.

## 🚀 How to Run
1. **Clone this repository**:
   ```bash
   git clone https://github.com/yourusername/AF3005_ProgrammingForFinance.git
   ```
2. **Install dependencies** (if not already installed):
   ```bash
   pip install ipywidgets
   ```
3. **Open Jupyter Notebook** and navigate to the `.ipynb` file.
4. **Run the notebook** and use the interactive widgets to enter stock prices.
5. The system will process the prices and provide alerts when the target price is met.

## 📂 Repository Structure
```
AF3005_ProgrammingForFinance/
│── i222290_Kainat_Irfan_AF3005–Assignment_1_Smart_Financial_Management_System.ipynb
│── README.md
```

## 🏗 Understanding `ipywidgets`
This project utilizes `ipywidgets` to create an interactive stock tracking system. Below are the widgets used:

### 🔹 **1. IntSlider**
Used to input stock prices interactively.
```python
import ipywidgets as widgets
price_slider = widgets.IntSlider(min=0, max=500, step=1, description='Stock Price:')
display(price_slider)
```
**Usage:** Users can slide to select a stock price.

### 🔹 **2. Button**
Used to trigger the tracking system.
```python
track_button = widgets.Button(description='Track Stock')
display(track_button)
```
**Usage:** Clicking this button starts the stock price evaluation.

### 🔹 **3. Output**
Displays alerts when conditions are met.
```python
output = widgets.Output()
with output:
    print("Tracking started...")
display(output)
```
**Usage:** Displays messages like "Stock reached PKR 200!"

### 🔹 **4. VBox & HBox**
Used to arrange widgets in a structured layout.
```python
ui = widgets.VBox([price_slider, track_button, output])
display(ui)
```
**Usage:** Groups multiple widgets together for better presentation.


### 🔗 Author
Kainat Irfan (i222290)

