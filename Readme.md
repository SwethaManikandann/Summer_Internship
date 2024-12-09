# 🌾 **FNN Crop production rate prediction for farmers using Knowledge Graph**

# 📜 **Project Overview**
This project implements a deep learning-based approach to classify crop production levels (low, medium, high) and visualize insights using a knowledge graph. A user-friendly Flask web interface is designed for user interaction, allowing real-time visualization of crop-specific knowledge graphs based on the input crop name.

# Features
Multi-class classification of crop production using a feed-forward neural network.
Knowledge graph visualization for relationships between crops, seasons, and states.
Flask-based user interface for seamless interaction.
Insights on top-performing states and seasons for a given crop.
Scalable design to incorporate additional data and real-time predictions.

# 📊 **Dataset**
Source: Indian Agriculture Crop Production database.
Key Features:
`Crop Type`, `Season`, `State`, `District`, `Area`, `Crop Year`, `Production Rate`.
Target Variable: Production Class (`Low, Medium, High`).

# ⚙️**System Workflow**
1) Data Preprocessing:
        Handle missing values and normalize categorical data using label encoding.
        Define production classes using quantiles for multi-class classification.
        Scale feature data and one-hot encode the target variable.
        ![Crop production Dataset](dataset.JPG)
2) Model Development:
        Train a deep learning model using TensorFlow/Keras with multiple hidden layers and ReLU activation.
        Use early stopping to optimize training and prevent overfitting.
        ![Model Training & Evaluation](ar3.PNG)
        ![Classification Metrics for each class](classi.JPG)
        ![Comparison of Predicted and Actual classes](comp.JPG)
        ![Training and Validation Accuracy over epochs](acc.JPG)
        ![Training and Validation loss over epochs](loss.JPG)
3) Knowledge Base Construction:
        A KB for predicting crop production rates and prices can consist of the following components:

        Entities: Key objects such as crops, years, regions, production rates, and prices.

        Attributes: Characteristics of each entity (e.g., production rate, price, soil type).

        Relationships: Links between entities (e.g., "Region X affects Crop Y's production").

        Rules: Logical inferences or trends derived from historical data and predictive models.
        ![Knowledge Base in Tabular Form](<kb.JPG>)
        
4) Knowledge Graph Generation:
        Use NetworkX to create graphs visualizing crop relationships with states and seasons.
        Highlight the state and season with the highest production for the given crop.
        ![Knowledge Graph generation](<result image.JPG>)
5) User Interaction:
        Develop a Flask-based web application for user input and graph visualization.
        ![User Interface](5.png)


# 📚 **Libraries Used**

- **Deep Learning**: TensorFlow, Keras

- **Data Processing**: Pandas, NumPy, Scikit-learn

- **Graph Visualization**: NetworkX, Matplotlib

- **Web Development**: Flask

# 🖥️**System Requirements**
# Hardware:
- **Processor**: Intel Core i5 or higher.
- **RAM**: Minimum 8GB.
- **Storage**: 256GB SSD (minimum).

# Software:
Python 3.x
Libraries: TensorFlow, Pandas, NetworkX, Flask, Matplotlib
Usage Instructions

# Setup:

Clone the project repository.
Install dependencies using pip install -r requirements.txt.
Run the Application:

Start the Flask server with python app.py.
Open the web interface at http://127.0.0.1:5000 or http://192.168.1.120:5000

# Input:
Enter the name of the crop (e.g., "Rice").
!(4.png)

# Output:
View the knowledge graph and insights for the entered crop.
!(5-1.png)

# 🔮 **Future Enhancements**
- **Real-Time Data Integration**: Incorporate real-time weather and market data for dynamic predictions.

- **Mobile-Friendly Interface**: Adapt the Flask app for mobile devices to improve accessibility.

- **Expanded Dataset**: Integrate additional crops, soil data, and economic parameters for broader applicability.
