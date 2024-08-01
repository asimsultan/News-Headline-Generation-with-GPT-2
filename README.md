
# News Headline Generation with GPT-2

Welcome to the News Headline Generation with GPT-2 project! This project focuses on generating news headlines using the GPT-2 model.

## Introduction

News headline generation involves creating catchy and relevant headlines based on news content. In this project, we leverage the power of GPT-2 to generate news headlines using a dataset of news articles.

## Dataset

For this project, we will use a custom dataset of news articles and their headlines. You can create your own dataset and place it in the `data/headline_data.csv` file.

## Project Overview

### Prerequisites

- Python 3.6 or higher
- PyTorch
- Hugging Face Transformers
- Datasets
- Pandas

### Installation

To set up the project, follow these steps:

```bash
# Clone this repository and navigate to the project directory:
git clone https://github.com/your-username/gpt2_news_headline_generation.git
cd gpt2_news_headline_generation

# Install the required packages:
pip install -r requirements.txt

# Ensure your data includes news articles and their headlines. Place these files in the data/ directory.
# The data should be in a CSV file with one column: text.

# To fine-tune the GPT-2 model for news headline generation, run the following command:
python scripts/train.py --data_path data/headline_data.csv

# To evaluate the performance of the fine-tuned model, run:
python scripts/evaluate.py --model_path models/ --data_path data/headline_data.csv
