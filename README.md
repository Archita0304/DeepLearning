# BLIP Visual Question Answering (VQA) Project

This repository demonstrates the use of the BLIP (Bootstrapped Language-Image Pretraining) model for Visual Question Answering (VQA) tasks. The project utilizes the `Salesforce/blip-vqa-base` model available on Hugging Face to answer user-provided questions about an input image.

## Overview
The BLIP model is a powerful tool for image-text tasks, such as generating captions, answering questions about images, and more. This project provides a Python script that takes an image and a question as input and generates an answer using the BLIP model.

## Features
- Load an image from the local filesystem.
- Display the loaded image using Matplotlib.
- Use the BLIP VQA model to process the image and answer a question.
- Output the generated answer in the terminal.

## Requirements
To run this project, you need the following dependencies:

- Python 3.7 or later
- PyTorch
- Transformers library from Hugging Face
- Pillow (PIL)
- Matplotlib

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Archita0304/DeepLearning.git
   cd DeepLearning
   ```

2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install the required dependencies:
   ```bash
   pip install torch transformers pillow matplotlib
   ```

## Usage
1. Place your image in the project directory or note its full path.

2. Run the notebook:
   - Open Google Colab.
   - Upload the `DL_project.ipynb` file to Colab.
   - Execute the cells step by step.

3. Follow the prompts:
   - Enter the path to the image (e.g., `path/to/your/image.jpg`).
   - Enter a question about the image (e.g., "What is in the image?").

4. The script will display the image and print the answer to your question in the output cell.

## Example
### Input:
- Image: A picture of a dog.
- Question: "What animal is in the image?"

### Output:
- Displayed image: The input image of the dog.
- Answer: "dog"

## File Structure
```
.
├── DL_project.ipynb  # Jupyter Notebook for the VQA task
├── requirements.txt  # List of dependencies (optional)
└── README.md         # Project documentation
```

## Customization
- You can modify the `image_path` and `question` variables directly in the code for testing purposes.
- Extend the notebook to handle batch processing or integrate it into a larger application.

## Limitations
- The BLIP model might not always produce accurate answers for complex or ambiguous questions.
- The model relies on pretrained weights, so performance depends on the training data.

## References
- [BLIP on Hugging Face](https://huggingface.co/Salesforce/blip-vqa-base)
- [Transformers Documentation](https://huggingface.co/docs/transformers/)

## License
This project is licensed under the MIT License. Feel free to use and modify it as needed.

## Acknowledgments
- Hugging Face for providing the BLIP model and tools.
- Salesforce Research for developing BLIP.

