# Happy vs. Sad Image Classification Project

This project is a binary image classification model that distinguishes between happy and sad facial expressions. The model was developed using TensorFlow and Keras, achieving high accuracy, precision, and recall.

## Project Structure

- **`data/`**: This folder contains the training and validation datasets used in the project. Ensure you populate this folder with your data before training the model.
  
- **`models/`**: This folder contains the trained models. The `happysad.h5` model is the best-performing model trained during this project.

- **`logs/`**: Contains logs generated during training for analysis using TensorBoard.

- **`myenv/` and **`.venv/`**: These are virtual environments used for package and dependency management. You can use either of these or set up your environment as described below.

- **`happtest.jpg` and `sadtest.jpg`**: Example images for testing the model's predictions.

- **`Image Classification.ipynb`**: The main Jupyter notebook where the model is built, trained, and evaluated.

## Setup

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. **Create and Activate a Virtual Environment** (if not using the provided ones):
   ```bash
   python3 -m venv myenv
   source myenv/bin/activate  # On Windows: myenv\Scripts\activate
   ```

3. **Install Dependencies**:
   Install the necessary Python packages:
   ```bash
   pip install -r requirements.txt
   ```

4. **Prepare the Data**:
   Ensure the `data/` folder contains your training and validation images structured correctly for binary classification (e.g., `data/happy` and `data/sad` directories).

5. **Run the Notebook**:
   Open and run the `Image Classification.ipynb` file in Jupyter Notebook or Visual Studio Code.

   ```bash
   jupyter notebook Image\ Classification.ipynb
   ```

6. **Evaluate the Model**:
   After training, you can use the `happtest.jpg` and `sadtest.jpg` images to test your model's predictions.

## Model Details

The model architecture includes several Conv2D layers with ReLU activations, Dropout layers for regularization, and Dense layers for classification. The final trained model (`happysad.h5`) achieved the best performance with the following metrics:

- **Accuracy**: 100%
- **Precision**: 1.0
- **Recall**: 1.0

## Future Work

While this project focuses on binary classification (happy vs. sad), you can expand it to classify more emotions, enhance the dataset, or apply transfer learning for better results.

## Acknowledgments

This project was inspired by the completion of the happy vs. sad classification tutorial by Nicholas Renotte and extended to improve the model's performance.
