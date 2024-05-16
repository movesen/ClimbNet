# ClimbNet Notebook

This notebook contains the implementation and evaluation of a Node embedding and a Graph neural network model for predicting grades of climbing routes based on graph data. The notebook is structured as follows:

## Setup

### Dataset
[Link to dropbox download of dataset](https://www.dropbox.com/scl/fo/92ntgb4vdsfartckqtav8/ACh25SZRk7pFYexn9Zh7w0U?rlkey=nfvqoonba0cdjwq361mrrjlf6&st=gru0s7b3&dl=0)

### Dependencies

- `os`: Standard library module for interacting with the operating system.
- `random`: Standard library module for generating random numbers.
- `json`: Standard library module for parsing and creating JSON data.
- `numpy`: Library for numerical computing with Python. Install using `pip install numpy`.
- `pandas`: Library for data manipulation and analysis. Install using `pip install pandas`.
- `matplotlib`: Library for creating static, animated, and interactive visualizations in Python. Install using `pip install matplotlib`.
- `plotly`: Library for creating interactive plots. Install using `pip install plotly`.
- `sklearn`: Library for machine learning in Python. Install using `pip install scikit-learn`.
- `networkx`: Library for the creation, manipulation, and study of complex networks of nodes and edges. Install using `pip install networkx`.
- `torch`: Deep learning library from Facebook's AI Research lab. Install using `pip install torch`.
- `torch_geometric`: Library for geometric deep learning extension library for PyTorch. Install using `pip install torch-geometric`.
- `gensim`: Library for unsupervised topic modeling and natural language processing. Install using `pip install gensim`.

### Loading Data

We load the graph data and corresponding labels from the source files. Each graph represents a climbing route, where nodes are holds and edges are connections between holds.

### Data Transformation

The graph data is transformed into a format suitable for model training. This includes converting the graphs into torch_geometric data objects and attaching embeddings to all nodes.

### Helper Functions

Several helper functions are defined to facilitate data processing and transformation.

## Model Definition

### Graph Nerual Net Model

The `GCN` class defines the architecture of the neural network model. It consists of multiple graph convolutional layers to process the graph data.

## Training the Model

### Training Loop

The training loop iterates over the training data, performing forward and backward passes to update the model parameters. Training progress is logged, including loss and accuracy metrics.

## Evaluating the Model

### Evaluation Loop

The evaluation loop processes the test data, making predictions and calculating accuracy and average test loss. This step is crucial to assess the model's performance on unseen data.

## Results

### Metrics

The results of the evaluation, including accuracy and average test loss, are printed. These metrics provide insight into the model's performance on the test dataset.

### Future work

We want to leverage both embeddings and the spacial information of our graphs better by better defining the Grapch neural network framework, specifically tailored towards subgraph classification as opposed to naive graph classification

