# YouTube-Engagement-Score-Prediction

A regression deep learning problem for predicting the Engagement Score of YouTube videos based on various video-related features.


The dataset used in this project is obtained from Kaggle - [YouTube 2025 Dataset](https://www.kaggle.com/datasets/amansingh0000000/youtube-2025-dataset/data)
The dataset includes information about:

Video information – title, description, category, duration, resolution, etc.

Channel data – subscriber count, channel age, etc.


Target variable – Engagement Score, representing how engaging the video is based on interactions.

## Feature encoding
To prepare the data for deep learning models, a custom encoding function encode_dataframe(df) was created and applied to the dataset.

The function performs the following steps:

Label Encoding for binary categorical columns.

One-Hot Encoding for multi-class categorical features (with more than two unique values).

Boolean conversion: All boolean values resulting from encoding were converted into integer format using a lambda function to ensure model compatibility.

## Feature scaling
MinMaxScaler from sklearn.preprocessing was used to apply min-max scaling on the numerical.
