# TripleTen Sprint 15 Project - Computer Vision and Age Verification

This is the 15th project I worked on in the TripleTen Data Science program. The goal was to explore whether Data Science can help the Good Seed Supermarket Chain adhere to alcohol laws by making sure they do not sell alcohol to people underage. The project contains two Jupyter Notebook files and a python file. The Jupyter Notebook files are the first and second half of this project. The exploratory data analysis was done in the file labled as EDA, and the GPU output was explored in the file labled as GPU. The GPU notebook file still has the EDA observations, but the code outputs are missing. 

## Project Goals

The goal of the project was to solve the following tasks:

1. Build and evaluate a model for verifying people's age. This will help the company adhere to alcohol laws.
2. Perform exploratory data analysis to get an overall impression of the dataset.
3. Train and evaluate the model on a GPU platform, reaching an MAE of below 8. 
4. Combine your code, output, and findings in the final Jupyter notebook.

### The Data

The dataset includes a set of photographs of people with their ages indicated.

### The Process

1. Performed exploratory data analysis to get an overall impression of the dataset.
2. Trained and evaluated the model on a GPU platform using the Keras API from TensorFlow. The model uses the ResNet50 architecture with pre-trained weights from ImageNet. It processes image data, trains with the Adam optimizer and Mean Squared Error loss function, and evaluates performance using Mean Absolute Error.
3. Combined the code, output, and findings in the final Jupyter notebook.

## Results

After preprocessing and analyzing the data, a computer vision model was trained on the age data of many faces. The model seems to be ready to be implemented in the field after some further testing. A company could use such a model to analyze the ages of customers to great effect based on the above data. The test MAE of the final model was 5.825, far under the threshold value of 8.

## Conclusion

The project has provided strategic insights for the Good Seed Supermarket Chain. These insights have the potential to guide future strategies and optimize revenue generation. For more details, please refer to the following:

1. **EDA_computer_vision_age_verification.ipynb**: This contains the exploratory data analysis and preperation of the project
2. **GPU_output_computer_vision_age_verification.ipynb**: This contains a detailed description of the results of the GPU training.
3. **test.py**: It includes the model that can be uploaded to a GPU platform.

Unfortunately, the photo dataset was too large to post on GitHub. Additionally, the GPU output will not appear when viewing the Jupyter Notebook file directly through GitHub. To access the full output, please download the Jupyter Notebook file and view them using Visual Studio Code.
