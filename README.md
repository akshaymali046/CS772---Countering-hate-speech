# Hate Speech Counter-Narration Generation

This repository contains the code and resources for generating counter-narrations against hate speeches using the CONAN dataset. The goal of this project is to leverage natural language processing techniques to automatically create counter narratives that provide factual information and real-world contexts to mitigate the impact of hate speech.

## Contributors
- Akshay EKnath Mali (213079006)
- Mahesh Abnave
- Sanjna Mohan
- Meet Joshi

## Table of Contents

- [Dataset](#dataset)
- [Architecture](#architecture)
- [Dependencies](#dependencies)

## Dataset

We used the CONAN dataset, which contains hate speech samples, as a basis for this project. Key phrases were extracted from these hate speeches to capture the essence of the content.

## Architecture

The architecture of this project consists of three main stages:

1. **Knowledge Sentence Extraction**: We extracted key phrases and sentences from the hate speeches in the CONAN dataset. These sentences form the basis for the counter-narration generation.

2. **Pair Creation**: Using preprocessing techniques, we designed an approach to create over 5,000 Hate Speech Knowledge Counter-Narration (HS-KN-CN) pairs. These pairs serve as the training data for the next stage.

3. **Fine-tuning GPT-2 and T5**: We fine-tuned the GPT-2 and T5 models on the HS-KN-CN pairs. The fine-tuned models are then capable of generating counter-narrations given hate speech inputs. The generated counter-narrations are focused on presenting facts and real-world contexts to counteract the hate speech content.

## Usage

1. **Data Preprocessing**: Run the data preprocessing scripts to extract key phrases from the CONAN dataset and create the HS-KN-CN pairs.

2. **Fine-tuning**: Use the provided scripts to fine-tune the GPT-2 and T5 models on the HS-KN-CN pairs. Make sure to adjust the hyperparameters as needed.

3. **Generation**: After fine-tuning, you can use the trained models to generate counter-narrations for hate speech inputs. Example scripts are provided to demonstrate the generation process.

## Dependencies

- Python 3.x
- TensorFlow
- Hugging Face Transformers Library
- CONAN dataset

## Sources
- CS772 -deep learning for NLP

