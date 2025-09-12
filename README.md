# Fake Review Detector App

This project is a machine learning based application that detects whether a review is **fake or genuine** and also performs **sentiment analysis**.  
You can run and test the project easily on **Google Colab** without any local setup.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/unrealayush/Fake-Review-Detector-App/blob/main/Review_Detection.ipynb)

---

## How to Use on Google Colab

1. **Open Google Colab**

   Go to [Google Colab](https://colab.research.google.com/).

2. **Clone the Repository**

   In a new Colab notebook, run:

   ```python
   !git clone https://github.com/unrealayush/Fake-Review-Detector-App.git
   %cd Fake-Review-Detector-App
   ```

3. **Install Dependencies**

   ```python
   !pip install -r requirements.txt
   ```

4. **Run the Jupyter Notebook**

   Open the training / analysis notebook:

   ```python
   from google.colab import drive
   drive.mount('/content/drive')   # optional if saving results to Google Drive
   ```

   Or directly run:

   ```python
   !jupyter nbconvert --to notebook --execute Review_Detection.ipynb --output=output.ipynb
   ```

   This will execute the notebook and generate results.

5. **Test the Model**

   Load the saved pipeline (`review_pipeline.pkl`) and predict on custom input:

   ```python
   import pickle

   with open("review_pipeline.pkl", "rb") as f:
       model = pickle.load(f)

   sample_review = "This product is amazing, I loved it!"
   prediction = model.predict([sample_review])[0]
   print("Prediction:", prediction)
   ```

   Output will show whether the review is **fake / genuine** and its **sentiment**.

---

## Notes

- You don’t need ChromeDriver or Flask when running on Colab (those are for the local web app).  
- On Colab, you can directly work with the **dataset CSV files** and the **model notebook**.  
- To deploy the web app version, you would need to run `app.py` locally.

---

## Author

[unrealayush](https://github.com/unrealayush)
