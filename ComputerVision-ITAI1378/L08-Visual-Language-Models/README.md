# L08 - Vision Transformers and Vision Language Models

## Course Information

- Student: Ali Abed
- Course: ITAI 1378 - Computer Vision
- Institution: Houston City College

## Problem Statement

This project explores how Vision Transformers and
Vision Language Models (VLMs) process images,
understand visual information, and respond to
natural language questions.

## Approach

The project uses pretrained SmolVLM models from
Hugging Face to perform multiple computer vision
tasks through natural language prompts.

The main exercises include:

- Vision Transformer image patch visualization
- Image captioning
- Visual question answering
- Object classification and counting
- Image text recognition
- Accessibility alt-text generation
- Chart reading and interpretation
- Hallucination detection
- Prompt engineering
- Model size and performance comparison

## Results

| Metric | Result |
|---|---|
| Primary model | SmolVLM-500M-Instruct |
| Comparison model | SmolVLM-256M-Instruct |
| Runtime GPU | NVIDIA Tesla T4 |
| Image dimensions | 384 x 384 |
| Small patch size | 48 x 48 |
| Small patch count | 64 |
| Large patch size | 96 x 96 |
| Large patch count | 16 |

The model successfully identified the main subject
of a sample image and answered visual questions.

In the receipt-reading experiment, the model
correctly extracted the total of $9.75 and the
bread price of $2.25.

The model also correctly recognized the small
text "EXIT 4B" in a generated test image.

The hallucination experiments demonstrated that
VLMs can produce incorrect or unsupported details,
especially when questions contain false assumptions.

The smaller 256M model showed weaker prompt-following
behavior compared with the 500M model in the
selected comparison examples.

## Key Findings

- Vision Transformers divide images into patches.
- Smaller patches preserve more visual detail.
- VLMs combine visual understanding with language.
- One model can perform multiple tasks through prompts.
- Prompt wording affects the quality of responses.
- Smaller models may struggle with instruction following.
- Confident AI responses are not always accurate.
- Human verification is important for critical applications.

## Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- Hugging Face Accelerate
- SmolVLM-500M-Instruct
- SmolVLM-256M-Instruct
- Pillow
- Matplotlib
- Pillow-HEIF
- Google Colab
- Jupyter Notebook

## Image Sources

This project uses publicly available sample images,
locally uploaded images, and programmatically
generated test images.

Sample image source:

https://huggingface.co/datasets/huggingface/documentation-images

Model sources:

https://huggingface.co/HuggingFaceTB/SmolVLM-500M-Instruct

https://huggingface.co/HuggingFaceTB/SmolVLM-256M-Instruct

## How to Run

1. Open the notebook in Google Colab.
2. Enable a GPU runtime if available.
3. Install the required Python libraries.
4. Upload the required sample images or substitute
   your own images and update the file paths.
5. Run the notebook cells in order.
6. Allow the pretrained models to download.
7. Review the model responses and visualizations.

## Real-World Applications

- Accessibility tools
- Automated image descriptions
- Document and receipt processing
- Visual assistants
- Multimodal AI systems
- Intelligent robotics
- Automated chart interpretation

## Limitations

Vision Language Models can hallucinate information,
misinterpret visual details, and produce inconsistent
responses when prompts are rephrased.

The experiments demonstrate model capabilities but
do not establish overall accuracy or reliability.

## Acknowledgments

This project was completed as part of the ITAI 1378
Computer Vision coursework.

Original lab author: Patricia McManus.
Original lab collaborator: Claude (Anthropic).
