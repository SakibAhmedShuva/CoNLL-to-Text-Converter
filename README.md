# CoNLL-to-Text-Converter

Convert your CoNLL files to text files where each line is separated by a new sentence. This tool allows you to easily import the resulting raw text file into Label Studio or other annotation platforms.

## Features

- Extracts complete sentences from CoNLL format files
- Handles document start markers and empty lines
- Preserves punctuation (except single hyphens)
- Outputs a clean text file with one sentence per line
- Easy to use with customizable input and output file paths

## Requirements

- Python 3.6+
- Jupyter Notebook (optional, for running the provided notebook)

## Usage

1. Clone this repository:
   ```
   git clone https://github.com/SakibAhmedShuva/CoNLL-to-Text-Converter.git
   cd CoNLL-to-Text-Converter
   ```

2. Open the `conll2text.ipynb` notebook in Jupyter, or use the provided Python script.

3. Modify the `input_file` variable to point to your CoNLL file:
   ```python
   input_file = r"path/to/your/conll/file.conll"
   ```

4. Run the script or notebook cells.

5. The converted text file will be saved as `sentences.txt` in the same directory by default.

## Function Details

The script contains two main functions:

1. `extract_sentences_from_conll_file(input_file)`:
   - Reads the CoNLL file and extracts sentences
   - Handles document start markers and empty lines
   - Returns a list of sentences

2. `write_sentences_to_text_file(sentences, output_file)`:
   - Writes the extracted sentences to a text file
   - Each sentence is on a new line

## Error Handling

The script includes basic error handling for file not found and general exceptions during file reading and writing operations.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

- The NLP community for establishing and maintaining the CoNLL format standard
- Label Studio and other annotation platforms for inspiring easier data import methods
