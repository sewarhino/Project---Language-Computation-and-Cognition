
# Surprisal and Reading Times Analysis

## Overview

This repository contains the code and data used in the project that investigates the relationship between surprisal and reading times. The project extends the findings from Smith and Levy (2013) by comparing surprisal estimates derived from N-gram and RNN (LSTM) models. Additionally, it explores the cross-linguistic consistency of this relationship across different languages.

## Project Description

The project involves the following key tasks:

- Training an RNN language model on the Penn Treebank dataset.
- Obtaining surprisal values from both N-gram and RNN models.
- Aligning surprisal values with human reading times.
- Comparing the correlation between surprisal estimates and reading times for both models.
- Exploring spillover effects, where the surprisal of a word impacts the reading time of the next word.
- Investigating how surprisal and reading times correlate across different languages in an open-ended task.

## Installation

To get started with this repository, follow the steps below:

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/your-repository-name.git
   cd your-repository-name
   ```

2. **Install the required dependencies:**

   - Python 3.7+
   - Required Python packages are listed in the `requirements.txt` file. Install them using:

     ```bash
     pip install -r requirements.txt
     ```

3. **Set up the environment:**

   - Make sure you have access to Google Colab or a similar environment for running the notebooks.

4. **Data Preparation:**

   - Download the required datasets (Penn Treebank, reading time data, etc.) and place them in the appropriate directories.


## Data

The repository includes the following data:

- **ptb_train.txt**: Training data from the Penn Treebank dataset - dowanloads directly in code
- **dev.txt**: Validation data from the Penn Treebank dataset - dowanloads directly in code 
- **passage_data.csv** and **sentence_data.csv**: Summarized eye-tracking measures by sentence and passage, available from the MECO (The Multilingual Eye-movement Corpus) dataset on OSF【OSF, 2024†source】.
- **joint_data_trimmed.rda**: Detailed eye-tracking measures for each word (interest area) in the texts, sourced from the MECO dataset on OSF【OSF, 2024†source】.
- **joint.readrate.rda**: Reading rates for each participant in each passage, obtained from the MECO dataset on OSF【OSF, 2024†source】.
- **Surprisal Estimates**: Surprisal estimates for ten languages in the MECO corpus, provided by the MECO dataset on OSF【OSF, 2024†source】.

## Experiments and Results

The results are discussed in the following sections:

1. **Structured Tasks**:
   - Training of the RNN model and obtaining surprisal estimates.
   - Comparison of the N-gram and RNN model correlation with reading times.
   - Analysis of spillover effects for both models.

2. **Semi-structured Tasks**:
   - Analysis of surprisal and reading times using General Additive Models (GAM).
   - Cross-linguistic analysis of the surprisal-reading time relationship.

## Open-ended Task

The open-ended task explores the relationship between surprisal and reading times across different languages. This section provides insights into how this relationship varies across languages, using the MECO corpus as the primary dataset.


## Acknowledgments

This project was guided by the work of Smith and Levy (2013) and inspired by the challenges posed in the course. Special thanks to the course instructor and teaching assistants for their invaluable support and guidance throughout the project.
