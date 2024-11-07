This project is focused on fine-tuning a Large Language Model (LLM) using a dataset of surgical questions and answers. The model uses unsloth's Llama-3.2-3B as the base model, along with various customizations to create a conversational agent capable of assisting with clinical surgery-related questions.

Project Structure
1. Model and Dataset
Base Model: unsloth/Llama-3.2-3B-Instruct, loaded using the FastLanguageModel API.
Dataset: A surgical dataset in CSV format, with question-answer pairs used for supervised fine-tuning (SFT).
2. Key Features
LoRA (Low-Rank Adaptation): Used to train the model with reduced memory requirements and faster processing.
Chat Template: A structured template for chat-based conversations, set to "llama-3.1".
Training Setup: Training with supervised fine-tuning (SFT) using SFTTrainer, along with gradient accumulation, dynamic padding, and mixed-precision support.
3. Inference
After training, the model is set up for inference with native optimizations for faster generation of responses.
Installation
Requirements
Python 3.8 or later
CUDA (if running on a GPU)
Install the Dependencies
To run this project, you will need the packages listed in the requirements.txt file.
