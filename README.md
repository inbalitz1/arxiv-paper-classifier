# Academic Paper Classification using Zero-Shot Learning
## Subject Indexing & NLP Project

### Project Overview
As a librarian in an academic setting, I developed this project to automate the classification of research papers from the arXiv dataset. Using Natural Language Processing (NLP), the system categorizes academic abstracts into broader disciplines (Physics, Computer Science, etc.) without requiring pre-labeled training data.

### Key Features
* **Zero-Shot Classification:** Utilized the `DistilBART` model to categorize papers based on semantic understanding.
* **Data Normalization:** Built a custom mapping system (Crosswalk) to translate technical arXiv codes (e.g., `hep-ph`, `cs.AI`) into human-readable academic categories.
* **Performance Optimization:** Implemented batched processing using Hugging Face `Datasets` to leverage GPU acceleration in Google Colab.

### Tech Stack
* **Language:** Python
* **Environment:** Spyder (Local Development) & Google Colab (Production)
* **Libraries:** Pandas, Hugging Face Transformers, PyTorch, OpenPyXL.

### Results
The model achieved an initial accuracy of ~80% (after Label Alignment), proving that LLMs can effectively assist in academic subject indexing and metadata enrichment.