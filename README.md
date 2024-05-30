# Vector Space Semantics for Similarity between Friends Characters

## Overview
This project focuses on constructing vector representations of dialogues from the TV show "Friends" to uniquely identify characters based on their spoken lines. By enhancing these vectors through sophisticated pre-processing and feature extraction techniques, the project aims to maximize the distinction between each character's vector from those of others. The ultimate goal is to accurately classify documents in the validation and test datasets as belonging to the correct character using simple information retrieval methods.

## Dataset
The dataset consists of scripted lines from "Friends" and is structured into training, validation, and test sets. The following data attributes are included:
- **Episode:** The episode of the show
- **Scene:** The scene within the episode
- **Character_name:** The name of the character speaking the line
- **Line:** The actual dialogue line spoken by the character
- **Gender:** The gender of the character (not used directly in feature extraction)

### Data Accessibility
The dataset is derived from publicly available scripts of the "Friends" TV show and formatted for this project's specific requirements.

## Project Structure
This project is divided into several analytical tasks, each designed to improve the model's ability to distinguish between different characters based on their lines:
- **Task 1:** Improve Pre-processing
- **Task 2:** Enhance Linguistic Feature Extraction
- **Task 3:** Incorporate Dialogue Context and Scene Features
- **Task 4:** Execute Systematic Parameter Search
- **Task 5:** Analyze Similarity Results
- **Task 6:** Final Testing on Test Data

## File Structure
- **CNN_for_Enhanced_Image_Classification.ipynb**: Jupyter notebook containing all the code and documentation for executing the tasks mentioned above.

## Methodology
The methodology involves several stages of processing and analysis:
1. **Pre-processing**: Standardizing text data, expanding contractions, removing stopwords, and applying stemming and lemmatization.
2. **Feature Extraction**: Utilizing techniques such as TF-IDF, n-grams, part-of-speech tagging, and sentiment analysis to convert text data into feature vectors.
3. **Context Integration**: Modifying scripts to include dialogue from surrounding lines based on the scene context, which provides additional data points for more accurate classification.
4. **Parameter Optimization**: Using grid search techniques to find the best model parameters for feature selection and classifier settings.
5. **Similarity Analysis**: Computing similarity scores between character vectors to analyze which characters have more in common linguistically.
6. **Testing**: Applying the trained model on a test dataset to evaluate its performance in terms of mean rank and accuracy.

## Results
The project achieved a Mean Rank of 1.8 on the test data, indicating the model's effectiveness in matching characters to their lines accurately. The accuracy was 60%, and the Mean Cosine Similarity score was approximately 0.949, demonstrating a high degree of semantic alignment between the training and testing dialogues.

