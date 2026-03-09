# Medical Transcription Classification using NLP

This project builds an NLP pipeline to classify medical transcription reports into specialties.

## Techniques Used
- Text preprocessing
- Tokenization and lemmatization
- Entity extraction
- Negation detection
- TF-IDF vectorization
- Logistic Regression classification

## Dataset
MT Samples medical transcription dataset<br>
Dataset link:  
https://www.kaggle.com/datasets/tboyle10/medicaltranscriptions

The dataset contains thousands of medical transcription reports categorized by medical specialty. Each record includes fields such as:

- **medical_specialty** – medical department of the report  
- **transcription** – full medical transcription text  
- **description** – short description of the case  
- **keywords** – related medical keywords  

The data was originally scraped from **MTSamples**, a collection of transcribed medical reports across multiple specialties.

## Results
Model achieved ~86% classification accuracy.

## How to Use

### 1. Clone the Repository
Clone the project to your local machine.

```bash
git clone https://github.com/yourusername/Medical-Transaction-Classification-System.git
cd Medical-Transcription-Classification-System
```

### 2. Install Dependencies
Make sure Python is installed, then install the required libraries.

```bash
pip install pandas numpy spacy scikit-learn matplotlib seaborn wordcloud
```

Download the spaCy language model:

```bash
python -m spacy download en_core_web_sm
```

### 3. Run the Notebook
Start Jupyter Notebook and open the project file.

```bash
jupyter notebook
```

Then open:

```
Medical_Transcript_Classification.ipynb
```

Run all cells sequentially to execute the full NLP pipeline.

### 4. Project Workflow
The notebook performs the following steps:

1. Text preprocessing and cleaning  
2. Tokenization and lemmatization  
3. Entity extraction using POS tagging  
4. Negation detection using dependency parsing  
5. TF-IDF feature extraction  
6. Machine learning classification of medical specialties  

### 5. Example Prediction

```python
predict_specialty("Patient presents with coronary artery blockage and chest pain")
```

Expected output:

```
Cardiovascular / Pulmonary
```
