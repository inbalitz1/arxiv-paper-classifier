# Academic Paper Classification using Zero-Shot Learning
## Subject Indexing & NLP Project

### Project Overview
As a librarian in an academic setting, I developed this project to automate the classification of research papers from the arXiv dataset. Using Natural Language Processing (NLP), the system categorizes academic abstracts into broader disciplines (Physics, Computer Science, etc.) without requiring pre-labeled training data.

### How to Run
1. Clone this repository.
2. Install dependencies: `pip install transformers datasets pandas openpyxl torch`.
3. Open the notebook in **Google Colab**, ensure GPU is enabled (T4), and run all cells.
4. The output will be saved as an Excel file with predictions and accuracy metrics.
   
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
<img width="1310" height="292" alt="image" src="https://github.com/user-attachments/assets/8635ab5f-e420-4279-aa3d-d0b94ff11928" />

### Challenges & Future Directions
* **Ambiguity in Interdisciplinary Papers:** Some papers naturally span multiple categories (e.g., Physics and Math). Future iterations could explore multi-label classification.
* **Label Refinement:** Expanding the custom Crosswalk dictionary to cover the full spectrum of arXiv's 150+ subcategories.
* **Model Comparison:** Testing the performance of larger models like `BART-large` vs. the current `DistilBART` on larger datasets.
