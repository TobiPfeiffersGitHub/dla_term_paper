# Deciphering Aesthetics: Investigating the Role of Image Resolution in Housing Price Prediction Models

This project aims to estimate the price of a house by leveraging both visual and textual features. Traditional methods for estimating house prices often rely solely on textual features, which may not capture the full extent of information available about a house, such as its condition and amenities. We are extending this by not only combining visual features extracted from house photographs and textual features, but also comparing the effect of the image resolution on the predictive accuracy of the model.

- Key Features
Utilizes a Convolutional Neural Network (CNN) to extract visual features from house photographs.
Compares the predictive performance of the model trained on low-resolution images versus high-resolution images.
Applies Grad-CAM heatmaps to interpret the regions in the images that the model is focusing on for its predictions.

Methodology
Data Acquisition: Obtain a dataset of houses, which includes images and corresponding textual descriptions.

- Preprocessing: Resize the images and encode the textual descriptions. The images are processed into two versions: low-resolution and high-resolution.

- Model Training: Build and train separate models for the textual features and the visual features, for both low-resolution and high-resolution images.

- Model Merging: Merge the models using a concatenation technique at a fully connected layer.

- Comparison and Analysis: Evaluate the model's performance using appropriate metrics such as mean squared error (MSE) and R-square value. Apply Grad-CAM to interpret the model's focus in the images.

- Results and Conclusion: 

The proposed method, which combines visual and textual features, has show slight improved accuracy in estimating house prices compared to traditional methods that rely solely on textual features. By comparing low-resolution and high-resolution images, we are able to analyze the impact of image quality on the model's predictive performance. The application of Grad-CAM further provides insights into how the model makes predictions based on visual features.
