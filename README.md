#  Email Evaluation System

##  Project Overview

This project implements an evaluation system to assess the quality of generated emails based on predefined scenarios. The system uses custom metrics to measure content accuracy, similarity to reference emails, and structural quality.

---

##  Objective

* Generate emails based on intent and facts
* Evaluate emails using custom metrics
* Compute a final score using weighted evaluation
* Export results in JSON and CSV format

---

##  Project Structure

```
email-evaluation-system/
│
├── evaluation.ipynb        # Main notebook
├── results.json            # Evaluation output (JSON)
├── results.csv             # Evaluation output (CSV)
└── README.md               # Documentation
```

---

##  Setup & Execution

### 1. Install Requirements

```
pip install pandas
```

### 2. Run the Project

* Open Jupyter Notebook
* Run all cells in `evaluation.ipynb`
* Results will be generated automatically

---

##  Evaluation Metrics

### 1. Content Accuracy

Checks whether required facts are present in the generated email.

### 2. Reference Similarity

Measures similarity between generated and reference email using sequence matching.

### 3. Structure & Fluency

Ensures proper email format and readability.

### 4. Diversity

Measures variation in word usage to avoid repetition.

---

##  Scoring Formula

Final Score is computed as:

```
0.40 × Reference +
0.30 × Content +
0.20 × Structure +
0.05 × Fluency +
0.05 × Diversity
```

---

##  Output

* `results.json` → Detailed evaluation results
* `results.csv` → Tabular evaluation results

---

##  Results

* Final Average Score Achieved: **0.853**
* High consistency across all scenarios
* Strong structure and content alignment

---

##  Limitations

* Relies on keyword-based matching
* Limited semantic understanding
* May penalize valid paraphrases

---

##  Future Improvements

* Use semantic similarity models (BERT, embeddings)
* Improve paraphrase detection
* Add grammar checking

---

##  Author

Aneesh Sharma Vukanti
