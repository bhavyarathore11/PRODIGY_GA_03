# Text Generation with Markov Chains

This project demonstrates text generation using Markov Chains. The goal is to create a simple, yet powerful, text generator that can learn from a given text corpus and produce coherent, contextually relevant sentences.

## Features

- **Text Training:** Train the Markov Chain model on a provided text corpus.
- **Text Generation:** Generate new text based on the trained model.
- **Customizable Parameters:** Adjust the order of the Markov Chain to control the coherence of the generated text.

## Getting Started

### Prerequisites

Ensure you have Python installed on your machine. You can download it from the [official Python website](https://www.python.org/).

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/your-username/text-generation-markov-chains.git
    ```

2. Navigate to the project directory:
    ```sh
    cd text-generation-markov-chains
    ```

3. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

## Usage

1. **Training the Model:**

   Provide a text file (`input.txt`) containing the corpus you want to train the model on. Run the following command:
    ```sh
    python train.py input.txt
    ```

2. **Generating Text:**

   Once the model is trained, you can generate text by running:
    ```sh
    python generate.py
    ```

   You can adjust the length of the generated text using the `--length` parameter:
    ```sh
    python generate.py --length 100
    ```

3. **Customizing Parameters:**

   You can change the order of the Markov Chain (default is 2) by using the `--order` parameter during training:
    ```sh
    python train.py input.txt --order 3
    ```

## Example

Here is an example of generating text using the provided sample corpus:

```sh
python train.py sample_corpus.txt
python generate.py --length 50
```

Output:
```
The quick brown fox jumps over the lazy dog. The lazy dog lies in the sun.
```

## Project Structure

- `train.py`: Script for training the Markov Chain model.
- `generate.py`: Script for generating text using the trained model.
- `markov_chain.py`: Contains the implementation of the Markov Chain class.
- `requirements.txt`: Lists the required Python packages.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Acknowledgements

This project was inspired by various text generation techniques and tutorials available online.

---

Feel free to customize this README file to better suit your project's specific details and requirements.
