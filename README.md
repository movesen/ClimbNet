# ClimbNet Notebook

This notebook contains the implementation and evaluation of a neural network model for predicting grades of climbing routes based on graph data. The notebook is structured as follows:

## Table of Contents

1. Setup
2. Data Preparation
3. Model Definition
4. Training the Model
5. Evaluating the Model
6. Results

## Setup

### Importing Libraries

In this section, we import the necessary libraries required for data processing, model building, and evaluation.

## Data Preparation

### Loading Data

We load the graph data and corresponding labels from the source files. Each graph represents a climbing route, where nodes are holds and edges are connections between holds.

### Data Transformation

The graph data is transformed into a format suitable for model training. This includes converting the graphs into torch_geometric data objects.

### Helper Functions

Several helper functions are defined to facilitate data processing and transformation.

## Model Definition

### ClimbNet Model

The `ClimbNet` class defines the architecture of the neural network model. It consists of multiple graph convolutional layers to process the graph data.

### Loss Function and Optimizer

We define the loss function (criterion) and optimizer used for training the model. These are essential for guiding the training process.

## Training the Model

### Training Loop

The training loop iterates over the training data, performing forward and backward passes to update the model parameters. Training progress is logged, including loss and accuracy metrics.

### Logging

During training, the model's performance is logged to monitor its progress and detect any potential issues.

## Evaluating the Model

### Evaluation Loop

The evaluation loop processes the test data, making predictions and calculating accuracy and average test loss. This step is crucial to assess the model's performance on unseen data.

### Error Handling

Any errors encountered during the evaluation are handled gracefully and logged for further analysis.

## Results

### Metrics

The results of the evaluation, including accuracy and average test loss, are printed. These metrics provide insight into the model's performance on the test dataset.

## Usage

1. **Install Dependencies:** Ensure you have the necessary libraries installed, such as `torch` and `torch_geometric`.
2. **Run the Notebook:** Open the notebook and run each cell sequentially to execute the code and obtain results.
3. **Modify Parameters:** You can modify the model architecture, training parameters, and data transformation functions as needed to experiment with different configurations.

## Conclusion

This notebook provides a comprehensive workflow for developing and evaluating a neural network model for predicting climbing route grades using graph data. The code is well-commented for better understanding and ease of modification.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Thanks to the creators of PyTorch and PyTorch Geometric for providing powerful tools for deep learning and graph processing.
- Special thanks to the dataset providers for making the data available for this project.

Feel free to modify this README to better fit your specific project requirements and details.
