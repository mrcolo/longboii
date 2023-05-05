# README.md

## MPT-7B-StoryWriter Text Generation

This repository contains a Python script that demonstrates how to use [MosaicML's MPT-7B-StoryWriter model](https://huggingface.co/mosaicml/mpt-7b-storywriter) for text generation. The model is based on the transformers library and is designed to generate coherent and contextually relevant text based on a given input.

Tested on a 3090.

### Prerequisites

To use this script, you need to have Python 3.7 or later installed. Additionally, you will need the following Python packages:

- torch
- transformers

You can install these packages using the following command:

```bash
pip install torch transformers
```

### Usage

The `run.py` script contains a function called `generate_text(input_text: str) -> str` that takes an input text string and generates relevant text based on the input.

First, import the `generate_text` function from the script:

```python
from run import generate_text
```

Then, call the function with your desired input text:

```python
input_text = "Once upon a time in a faraway land,"
output_text = generate_text(input_text)
print(output_text)
```

The `generate_text` function will return a string containing the generated text based on the input. You can adjust the input text to suit your needs and generate different text outputs.

### Customization

You can customize the behavior of the text generation by modifying the configuration settings in the `run.py` script. For example, you can change the `max_seq_len` parameter to control the maximum length of the generated text. Please refer to the [transformers documentation](https://huggingface.co/transformers/) for more information on the available configuration settings.

### License

This project is licensed under the MIT License. See the `LICENSE` file for details.

### Acknowledgments

- [Hugging Face](https://huggingface.co/) for providing the [transformers library](https://github.com/huggingface/transformers).
- [EleutherAI](https://www.eleuther.ai/) for providing the [GPT-NeoX model](https://github.com/EleutherAI/gpt-neox).
- [MosaicML](https://mosaicml.com/) for providing the [MPT-7B Storywriter model](https://huggingface.co/mosaicml/mpt-7b-storywriter).
