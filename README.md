Fake Review Detector App
Project Overview
This project is a web application designed to detect fake reviews. The application uses machine learning to classify reviews as either "authentic" or "deceptive" (fake). It provides a user-friendly interface where users can input a review and receive an instant prediction.

Features
Review Prediction: The core functionality of the app is to analyze and predict the authenticity of a given review.

Sentiment Analysis: The app also performs sentiment analysis on the reviews, classifying them as "positive," "negative," or "neutral."

Interactive UI: A simple and clean user interface for easy interaction.

Technologies Used
Python: The backend logic for the machine learning model.

Flask: A micro-framework for building the web application.

HTML/CSS/JavaScript: Frontend for the user interface.

Machine Learning: Utilizes a pre-trained model for classification.

Execution Steps
Follow these steps to set up and run the application on your local machine.

Step 1: Clone the Repository
First, you need to download the project files to your computer. Open your terminal or command prompt and run the following command:

git clone [https://github.com/unrealayush/Fake-Review-Detector-App.git](https://github.com/unrealayush/Fake-Review-Detector-App.git)

Step 2: Navigate to the Project Directory
Change your current directory to the cloned project folder:

cd Fake-Review-Detector-App

Step 3: Set Up the Virtual Environment (Recommended)
It's a best practice to use a virtual environment to manage dependencies. This ensures that the project's libraries do not conflict with other Python projects on your computer.

python -m venv venv

Activate the virtual environment:

On Windows:

venv\Scripts\activate

On macOS/Linux:

source venv/bin/activate

Step 4: Install Dependencies
With the virtual environment active, install all the required Python libraries using the requirements.txt file.

pip install -r requirements.txt

Step 5: Run the Flask Application
Finally, start the Flask web server. This will make the application accessible in your web browser.

python app.py

Step 6: Access the App
Open your web browser and go to the following URL to use the application:

[http://127.0.0.1:5000/](http://127.0.0.1:5000/)

You can now enter a review in the text box and click the "Predict" button to see the results.
