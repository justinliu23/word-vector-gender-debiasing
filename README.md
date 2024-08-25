# word-vector-gender-debiasing


## Table of Contents
- [Dependencies](#dependencies)
- [Usage](#usage)
  - [Running the Project](#running-the-project)
  - [Example Usage](#example-usage)
- [Configuration](#configuration)

## Dependencies

The following Python libraries are required for the project:

- `numpy`: Used for numerical computations, particularly in handling vectors and performing linear algebra operations.
- `matplotlib`: For visualizing data and displaying plots.
- `sklearn`: Utilized for additional utility functions related to machine learning tasks.
- `public_tests`: Contains additional test cases for validating the correctness of the functions.
- `planar_utils`: Custom utility functions that may include operations for plotting decision boundaries and handling datasets.

## Installation Instructions

### Prerequisites

Ensure that you have Python 3.x installed on your machine. You can verify this by running:

```bash
python --version
```

### Jupyter Notebook

This project is primarily designed to be run within a Jupyter notebook. If you don’t have Jupyter installed, you can do so via:

```bash
pip install jupyter
```

To start the Jupyter notebook, navigate to the project directory and run:

```bash
jupyter notebook
```

This command will open a new tab in your web browser with the Jupyter interface.

## Usage

### Running the Project

Once the environment is set up and all dependencies are installed, you can run the Jupyter notebook to interact with the project:

1. Navigate to the directory containing the notebook.
2. Run `jupyter notebook` in the terminal.
3. Open the relevant `.ipynb` file (e.g., `operations_on_word_vectors.ipynb`) in the browser.
4. Execute the cells in the notebook sequentially to see the output.

### Example Usage

- **Cosine Similarity Calculation**: You can use the function `cosine_similarity(u, v)` to compute the cosine similarity between two word vectors `u` and `v`.

- **Word Analogy Task**: Use the `complete_analogy(word_a, word_b, word_c, word_to_vec_map)` function to perform word analogy tasks like "man is to woman as king is to ____."

- **Debiasing Word Vectors**: The project includes an implementation to debias word vectors using techniques such as neutralization and equalization. For example, the `neutralize()` function projects a word vector onto the space orthogonal to the bias axis, effectively removing the bias.

- **Visualizing Results**: The notebook provides visualization capabilities to plot the results of the operations, such as showing how word vectors relate to each other in space.

## Configuration

There is minimal configuration required to run this project. However, ensure the following:

- The `word_to_vec_map` dictionary should be properly loaded with pre-trained word vectors (e.g., GloVe embeddings).
- Paths to any datasets or utility scripts must be correctly set relative to the project directory.
