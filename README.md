
# 📚 BookMatchML

An AI/ML-powered book recommender system built using NLP embeddings. Given a favorite book or genre, it recommends similar books using semantic search.

## 🔧 Tech Stack
- **NLP Embeddings**: `sentence-transformers` (HuggingFace)
- **Search**: FAISS (for efficient similarity retrieval)
- **UI**: Streamlit (interactive web interface)
- **MLOps**: MLflow (experiment tracking), DVC (data versioning)
- **CI/CD**: GitHub Actions (automated testing)

## 📁 Project Structure
```
BookMatchML/
├── data/              # Datasets (e.g., Goodreads data)
├── notebooks/         # Jupyter notebooks for EDA and experiments
├── src/               # Source code
│   ├── data_processing/  # Data cleaning and preprocessing
│   ├── embedding/        # Embedding generation with Sentence Transformers
│   ├── recommendation/   # Recommendation logic with FAISS/cosine similarity
│   └── ui/               # Streamlit UI components
├── models/            # Trained models and embeddings
├── app/               # Main application scripts
├── tests/             # Unit tests with pytest
├── requirements.txt   # Python dependencies
├── README.md          # Project documentation
├── .gitignore         # Git ignore file
```

## ⚙️ Local Setup
To set up the project directory structure locally (Windows), run the following commands in your terminal:
```bash
mkdir BookMatchML
cd BookMatchML
mkdir data
mkdir notebooks
mkdir src
mkdir src\data_processing
mkdir src\embedding
mkdir src\recommendation
mkdir src\ui
mkdir models
mkdir app
mkdir tests
type nul > requirements.txt
type nul > README.md
type nul > .gitignore
```

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/BookMatchML.git
   cd BookMatchML
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Launch the Streamlit app:
   ```bash
   streamlit run src/ui/app.py
   ```

## 💡 Features
- **Input**: Enter a favorite book title or genre.
- **Output**: Get the top 5 book recommendations with short summaries.
- Powered by Sentence Transformers for embedding book summaries and FAISS for fast similarity search.

## 📦 Dependencies
See `requirements.txt` for the full list. Key libraries include:
- `sentence-transformers`
- `faiss-cpu` (or `faiss-gpu` for GPU support)
- `streamlit`
- `mlflow`
- `dvc`

## 📝 Notes
- Dataset: Uses the Goodreads dataset (place in `data/`).
- Experiments and EDA are in `notebooks/`.
- Add your own Goodreads API key or dataset for extended functionality.


