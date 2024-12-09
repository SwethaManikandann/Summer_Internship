# Summer_Internship
# **FNN Crop Production Rate Prediction for farmers using Knowledge Graph**

# Project Overview
This project implements a deep learning-based approach to classify crop production levels (low, medium, high) and visualize insights using a knowledge graph. A user-friendly Flask web interface is designed for user interaction, allowing real-time visualization of crop-specific knowledge graphs based on the input crop name.

# Features
Multi-class classification of crop production using a feed-forward neural network.
Knowledge graph visualization for relationships between crops, seasons, and states.
Flask-based user interface for seamless interaction.
Insights on top-performing states and seasons for a given crop.
Scalable design to incorporate additional data and real-time predictions.

# Dataset
Source: Indian Agriculture Crop Production database.
Key Features:
Crop Type, Season, State, District, Area, Crop Year, Production Rate.
Target Variable: Production Class (Low, Medium, High).

# System Workflow
1) Data Preprocessing:
        Handle missing values and normalize categorical data using label encoding.
        Define production classes using quantiles for multi-class classification.
        Scale feature data and one-hot encode the target variable.
2) Model Development:
        Train a deep learning model using TensorFlow/Keras with multiple hidden layers and ReLU activation.
        Use early stopping to optimize training and prevent overfitting.

   ![image](https://github.com/user-attachments/assets/402a25b7-5ada-4162-86e2-b4537951035d)

   ![image](https://github.com/user-attachments/assets/759b9367-5e4a-4322-9347-654f90683d1b)


![image](https://github.com/user-attachments/assets/2205bef6-4ffd-42c8-b090-767c9a2f88ad)

   
![image](https://github.com/user-attachments/assets/699c4756-7c15-4857-a26b-46cc4d2ee3ec)

   
4) Knowledge Graph Generation:
        Use NetworkX to create graphs visualizing crop relationships with states and seasons.
        Highlight the state and season with the highest production for the given crop.
        User Interaction:

# Develop a Flask-based web application for user input and graph visualization.
# Libraries Used

Deep Learning: TensorFlow, Keras

Data Processing: Pandas, NumPy, Scikit-learn

Graph Visualization: NetworkX, Matplotlib

Web Development: Flask

# System Requirements
# Hardware:
Processor: Intel Core i5 or higher.
RAM: Minimum 8GB.
Storage: 256GB SSD (minimum).

# Software:
Python 3.x
Libraries: TensorFlow, Pandas, NetworkX, Flask, Matplotlib
Usage Instructions

# Setup:

Clone the project repository.
Install dependencies using pip install -r requirements.txt.
Run the Application:

Start the Flask server with python app.py.
Open the web interface at http://localhost:5000.

# Input:
Enter the name of the crop (e.g., "Rice").

# Output:
View the knowledge graph and insights for the entered crop.


# Future Enhancements
Real-Time Data Integration: Incorporate real-time weather and market data for dynamic predictions.

Enhanced Visualizations: Add interactive graphs using tools like Plotly or D3.js.

Mobile-Friendly Interface: Adapt the Flask app for mobile devices to improve accessibility.

Expanded Dataset: Integrate additional crops, soil data, and economic parameters for broader applicability.

