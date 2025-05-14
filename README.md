# Gendered Abuse Detection in Indic Languages 🌐

![Gendered Abuse Detection](https://img.shields.io/badge/Gendered_Abuse_Detection_in_Indic_Languages-brightgreen.svg)

Online gender-based violence limits marginalized voices. Detection in Indic languages is hard due to limited data and linguistic complexity. This work builds better classifiers for improved abuse detection in such settings. 

## Table of Contents
- [Introduction](#introduction)
- [Problem Statement](#problem-statement)
- [Dataset](#dataset)
- [Models](#models)
  - [BERT](#bert)
  - [Convolutional Neural Networks](#convolutional-neural-networks)
  - [GRU](#gru)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Releases](#releases)

## Introduction

Gender-based violence is a significant issue affecting many communities. In many cases, the voices of those most impacted are silenced. Detecting instances of abuse in Indic languages poses unique challenges. The linguistic diversity and limited resources complicate the development of effective detection systems. 

This repository aims to tackle these challenges by creating advanced classifiers. We focus on improving detection capabilities for gender-based violence in Indic languages.

## Problem Statement

The existing models for detecting gender-based violence often fail in Indic languages. The primary reasons include:

- **Limited Data**: There is a scarcity of labeled datasets for training models.
- **Linguistic Complexity**: Indic languages have diverse structures, making it hard for standard NLP models to perform well.
  
By addressing these issues, we hope to enhance the detection of gendered abuse and provide better support for marginalized voices.

## Dataset

We use various datasets that include text from social media, forums, and other platforms where abuse may occur. The datasets are curated to include instances of gender-based violence. 

### Data Sources

- Social media platforms
- Online forums
- Community reports

### Data Preparation

Data preprocessing involves:
- Tokenization
- Normalization
- Removing noise

This step ensures that the models receive clean and relevant data for training.

## Models

We explore several models to improve detection accuracy. 

### BERT

BERT (Bidirectional Encoder Representations from Transformers) has shown promise in understanding context in language. We fine-tune BERT for our specific task, allowing it to learn nuances in Indic languages.

### Convolutional Neural Networks

CNNs are effective in capturing local patterns in text. We adapt CNNs to analyze sequences of words, which helps in identifying abusive language.

### GRU

Gated Recurrent Units (GRUs) are another option for sequence modeling. They help in understanding context over longer sequences, making them suitable for our needs.

## Installation

To set up the project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/Tanlouie/Gendered_Abuse_Detection_In_Indic-Languages.git
   ```

2. Navigate to the project directory:
   ```bash
   cd Gendered_Abuse_Detection_In_Indic-Languages
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Ensure you have the necessary libraries:
   - PyTorch
   - Transformers
   - Scikit-learn

## Usage

After installation, you can start using the models. 

1. **Load the model**:
   ```python
   from model import load_model
   model = load_model('path_to_model')
   ```

2. **Make predictions**:
   ```python
   predictions = model.predict(input_text)
   ```

3. **Evaluate the model**:
   ```python
   from evaluator import evaluate
   results = evaluate(model, test_data)
   ```

## Results

We present the results of our models on a validation dataset. The metrics include:

- **Accuracy**: The percentage of correct predictions.
- **Precision**: The ratio of true positives to the sum of true and false positives.
- **Recall**: The ratio of true positives to the sum of true positives and false negatives.

Our models show promising results, demonstrating improved accuracy in detecting gender-based violence in Indic languages.

## Contributing

We welcome contributions to improve this project. If you have ideas or want to report issues, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push to your fork and submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For questions or feedback, feel free to reach out:

- **Email**: your-email@example.com
- **Twitter**: [@yourhandle](https://twitter.com/yourhandle)

## Releases

For the latest updates and versions, please visit the [Releases](https://github.com/Tanlouie/Gendered_Abuse_Detection_In_Indic-Languages/releases) section. Here, you can find downloadable files and execute them as needed.

![Download Releases](https://img.shields.io/badge/Download_Releases-blue.svg)

By improving detection methods, we can help amplify marginalized voices and address gender-based violence more effectively. Your support and contributions are invaluable in this mission.