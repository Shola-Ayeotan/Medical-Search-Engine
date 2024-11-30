
# Medical Word Embedding and Search Engine

## Overview
This project focused on building a machine learning-based search engine for the medical domain using word embeddings. The system used **Word2Vec** and **FastText** models to generate vector representations of medical terms and enables efficient search functionality based on those embeddings. The solution is deployed and scaled on **Azure**.

## Tech Stack
- **Language**: Python
- **Libraries**: NLTK, Scikit-Learn, Pandas, Numpy, Streamlit
- **Cloud**: Azure (Azure Data Factory, Azure Blob Storage, Azure Databricks)
- **Version Control**: Git, GitHub
- **Containerization**: Docker

## Data
The dataset used is the **Dimensions COVID-19 Publications and Clinical Trials Dataset**. The dataset can be accessed [here](https://dimensions.figshare.com/articles/dataset/Dimensions_COVID-19_publications_datasets_and_clinical_trials/11961063).

## Approach
1. **Data Preprocessing**:

2. **Model Training**:
   - Trained **Word2Vec** and **FastText** models using Azure Databricks.
   - Stored the trained models in **Azure Blob Storage** and set up periodic retraining.

3. **Search Engine**:
   - Built a search engine to retrieve similar records based on query input using cosine similarity between word embeddings.

4. **UI Deployment**:
   - Developed an interactive user interface with **Streamlit**.
   - Deployed the application to **Azure App Services**.

## Running the Project

### Prerequisites
- Python 3.x
- Install dependencies:
  ```bash
  pip install -r requirements.txt
  ```

### Steps to Run
1. **Train the Model**:
   - Execute `engine.py` to train the models and save them in **Azure Blob Storage**.

2. **Run the Streamlit UI**:
   - Start the UI by running:
     ```bash
     streamlit run medical.py
     ```

3. **Deploy the Solution**:
   - Deploy the model and application to **Azure Databricks** and **Azure App Services** for scalability.
