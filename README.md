# AI Studio 2024 Challenge: Job Title Generalization

![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg) ![License](https://img.shields.io/badge/License-MIT-green.svg) ![Platform](https://img.shields.io/badge/Platform-Jupyter-orange.svg)

## Overview

This project is part of the AI Studio 2024 Challenge in collaboration with **Candogram Inc.**, a leading provider of job market education. The goal is to analyze and classify job postings with the word "engineer" in their titles to create meaningful job title clusters and visualize these clusters effectively. This is my version of the project, my peers also have their own iterations which you should check out too!

### Key Objectives

- Analyze ~20,000 job postings containing the word "engineer."
- Group job titles into clusters (e.g., software engineer, civil engineer) using natural language processing (NLP) and clustering techniques.
- Provide a scatterplot visualization of the clusters and assign job titles to each cluster.

## Dataset

The dataset contains **20,138 job postings** in a CSV format with the following fields:

- `RequisitionID`
- `OrigJobTitle`
- `JobTitle`
- `JobDescription`

📥 [Download the dataset](https://candogram-downloads.s3.amazonaws.com/Engineer_20230826.zip)

### Preprocessing Steps

1. **Remove HTML tags** from job descriptions.
2. **Isolate job description text** from other sections of the postings.
3. Convert job descriptions into embeddings for clustering.

---

## Built With

![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg) ![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-blue.svg) ![Scikit-learn](https://img.shields.io/badge/Scikit--learn-Machine%20Learning-orange.svg) ![FastText](https://img.shields.io/badge/FastText-Word%20Embeddings-red.svg) ![matplotlib](https://img.shields.io/badge/matplotlib-Visualization-green.svg) ![pyLDAvis](https://img.shields.io/badge/pyLDAvis-Topic%20Modeling-brightgreen.svg)

---

## Methodology

- **Data Cleaning:**
  - Remove HTML code from job postings.
  - Extract relevant job description sentences (marketing, requirements, legal, etc.).

- **Vectorization:**
  - Convert job descriptions into vectors using techniques like **FastText** or similar.

- **Clustering Algorithms:**
  - Apply **KMeans** and **Latent Dirichlet Allocation (LDA)** for clustering.

### Key Tools and Libraries

- **Development Tools:** Jupyter Notebook, Python Virtual Environment
- **Libraries:** Pandas, Scikit-learn, matplotlib, pyLDAvis, FastText, GPT-4o mini API

---

## Results

### Deliverables

1. Scatterplot of clustered jobs.
2. Cluster-wise job titles with insights into their common features.

---

## Getting Started

### Prerequisites

- Python 3.9+
- Virtual environment set up in the project directory

### Steps

1. Clone this repository:
   ```bash
   git clone https://github.com/iDaManall/job-title-generalization.git
   ```
2. Navigate to the project directory:
   ```bash
   cd your-repo-name
   ```
3. Create a virtual environment and install dependencies:
   ```bash
   python3 -m venv env
   source env/bin/activate  # or env\Scripts\activate on Windows
   pip install -r requirements.txt
   ```
4. Download and prepare the dataset in the `data/` folder.
5. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

---

## Contribution Guidelines

We welcome contributions to improve the clustering accuracy or add new features. Please follow these steps:

1. Fork this repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit changes and push to your branch:
   ```bash
   git push origin feature-name
   ```
4. Create a pull request.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- **Candogram Inc.** for providing the dataset and challenge framework.
- References:
  - [CRISP-DM Methodology](https://www.datascience-pm.com/crisp-dm-2/)
  - [Topic Modeling Resource](https://www.youtube.com/watch?v=N0crN8YnF8Y)

