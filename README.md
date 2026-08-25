# 🧠 Persian Social Media Topic Modeling & Semantic Network Analysis

<p align="center">
  <b>A Comparative NLP Framework for Persian Social Media Analysis</b>
</p>

<p align="center">
  LDA • TF-IDF • Word2Vec • BERT • Clustering • Network Analysis • Temporal Modeling • Statistical Evaluation
</p>

---

## 🚀 Project Overview

Understanding large-scale social media conversations requires more than identifying frequently used words.

This project presents an **end-to-end Natural Language Processing (NLP) pipeline for Persian social media text**, combining classical topic modeling, semantic representations, transformer-based embeddings, network analysis, temporal analysis, and statistical model comparison.

The repository explores multiple approaches to discovering hidden thematic structures in Persian text and provides a comparative framework for evaluating how different NLP representations capture semantic patterns.

Rather than relying on a single topic-modeling algorithm, the project investigates several complementary approaches:

* 🧩 **Latent Dirichlet Allocation (LDA)**
* 📊 **TF-IDF-based Topic Modeling**
* 🔗 **N-gram Analysis**
* 🧠 **Word2Vec Semantic Representations**
* 🤖 **BERT-based Semantic Embeddings**
* 🕸️ **Semantic Network Analysis**
* ⏳ **Temporal Topic Analysis**
* 📈 **Friedman & Nemenyi Statistical Comparison**

---

## 🎯 Research Motivation

Persian social media presents several challenges for conventional NLP pipelines, including morphological variation, informal writing, sparse representations, and context-dependent semantics.

Traditional bag-of-words approaches can identify lexical patterns but often fail to capture deeper semantic relationships.

This project therefore compares **lexical, probabilistic, embedding-based, and transformer-based representations** within a unified analytical workflow.

The central question is:

> **How effectively can different NLP representations uncover meaningful thematic and semantic structures in Persian social media discourse?**

---

## 🧬 Analysis Pipeline

```text
                    Persian Social Media Text
                              │
                              ▼
                    ┌───────────────────┐
                    │ Text Preprocessing │
                    └─────────┬─────────┘
                              │
              ┌───────────────┼────────────────┐
              │               │                │
              ▼               ▼                ▼
             LDA           TF-IDF          N-grams
              │               │                │
              └───────────────┼────────────────┘
                              │
                              ▼
                     Word2Vec Embeddings
                              │
                              ▼
                       BERT Embeddings
                              │
                              ▼
                  Semantic Representation
                              │
                    ┌─────────┴─────────┐
                    ▼                   ▼
             Topic Discovery      Network Analysis
                    │                   │
                    └─────────┬─────────┘
                              ▼
                     Temporal Analysis
                              │
                              ▼
                Statistical Model Comparison
                              │
                              ▼
                    Friedman + Nemenyi
```

---

# 🔬 Methods

## 1. Latent Dirichlet Allocation

LDA is used as a probabilistic baseline for discovering latent topics from word co-occurrence patterns.

The approach provides interpretable topic-word distributions and establishes a baseline against which more advanced semantic representations can be evaluated.

📓 `Topic_Modeling_LDA.ipynb`

---

## 2. TF-IDF Topic Representation

TF-IDF weighting is applied to emphasize discriminative terms while reducing the influence of extremely common words.

This representation provides a stronger lexical baseline for identifying topic-specific vocabulary.

📓 `Topic_Modeling_TF_IDF.ipynb`

---

## 3. N-gram Analysis

N-gram representations capture frequently occurring multi-word expressions that cannot always be identified using isolated tokens.

This is particularly useful for identifying recurring expressions, entities, and discourse patterns.

📓 `Topic_Modeling_N_gram.ipynb`

---

## 4. Word2Vec Semantic Modeling

Word2Vec embeddings are used to move beyond purely lexical representations and model semantic similarity between words in a continuous vector space.

This allows related concepts to be identified even when they do not frequently appear in exactly the same lexical form.

📓 `Topic_Modeling_Word2vec.ipynb`

---

## 5. Transformer-Based Semantic Modeling

Contextual embeddings are used to represent text based on semantic meaning rather than simple word frequency.

BERT-based representations provide a richer representation of contextual relationships and enable semantic clustering of Persian social media content.

📓 `Topic_Modeling_Bert.ipynb`

---

## 🕸️ Semantic Network Analysis

Topic modeling is complemented by a graph-based representation of semantic relationships.

Terms and concepts can be represented as nodes, while their relationships form edges, allowing the analysis of:

* Semantic communities
* Highly connected concepts
* Network structure
* Topic relationships
* Community formation

📓 `Topic_Modeling_Graph.ipynb`

---

## ⏳ Temporal Topic Analysis

Social media conversations are dynamic.

The temporal component of the project investigates how thematic structures change across time, making it possible to identify:

* Emerging topics
* Declining themes
* Persistent discussions
* Temporal fluctuations
* Changes in discourse structure

📓 `Topic_Modeling_by_Time.ipynb`

---

# 📊 Statistical Model Comparison

Simply producing different topic models does not establish whether their performance differs systematically.

The project therefore includes statistical comparison using:

### Friedman Test

The Friedman test evaluates whether statistically significant differences exist among multiple modeling approaches.

### Nemenyi Post-hoc Test

When significant differences are detected, the Nemenyi procedure is used for pairwise comparison between methods.

📓 `Friedman_Nemenyi.ipynb`

This provides a statistical layer to the model-comparison process rather than relying exclusively on visual inspection.

---

# 🧠 Why Multiple Models?

Different NLP techniques capture different dimensions of language.

| Method                | Main Strength                             |
| --------------------- | ----------------------------------------- |
| **LDA**               | Interpretable probabilistic topics        |
| **TF-IDF**            | Discriminative lexical representation     |
| **N-grams**           | Multi-word expression discovery           |
| **Word2Vec**          | Semantic word similarity                  |
| **BERT**              | Context-aware semantic representation     |
| **Graph Analysis**    | Structural relationships between concepts |
| **Temporal Analysis** | Topic evolution over time                 |
| **Friedman/Nemenyi**  | Statistical model comparison              |

The objective is therefore not simply to identify a single “best” algorithm, but to examine how different representations reveal complementary dimensions of Persian social media discourse.

---

# 📁 Repository Structure

```text
Topic_Modeling/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── Topic_Modeling_Bert.ipynb
├── Topic_Modeling_LDA.ipynb
├── Topic_Modeling_TF_IDF.ipynb
├── Topic_Modeling_N_gram.ipynb
├── Topic_Modeling_Word2vec.ipynb
├── Topic_Modeling_Graph.ipynb
├── Topic_Modeling_by_Time.ipynb
├── Friedman_Nemenyi.ipynb
│
├── figures/
│   ├── bert_topic_clusters.png
│   ├── semantic_network.png
│   ├── topic_evolution.png
│   └── model_comparison.png
│
└── results/
```

---

# 🖼️ Visual Results

## Semantic Topic Clusters

<p align="center">
  <img src="figures/bert_topic_clusters.png" width="800">
</p>

---

## Semantic Network

<p align="center">
  <img src="figures/semantic_network.png" width="800">
</p>

---

## Topic Evolution Over Time

<p align="center">
  <img src="figures/topic_evolution.png" width="800">
</p>

---

## Model Comparison

<p align="center">
  <img src="figures/model_comparison.png" width="800">
</p>

---

# 🛠️ Technology Stack

### Programming

`Python` · `Jupyter Notebook`

### NLP & Machine Learning

`Transformers` · `BERT` · `Gensim` · `Scikit-learn` · `Word2Vec`

### Data Processing

`Pandas` · `NumPy`

### Network Analysis

`NetworkX`

### Visualization

`Matplotlib` · `WordCloud`

### Statistical Analysis

`SciPy` · `Friedman Test` · `Nemenyi Post-hoc Analysis`

---

# ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/MonaFaghfouri/Topic_Modeling.git
```

Move into the project directory:

```bash
cd Topic_Modeling
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Then launch Jupyter:

```bash
jupyter notebook
```

---

# 🔁 Reproducibility

The repository separates different analytical approaches into individual notebooks so that each method can be inspected and executed independently.

For reproducible use:

1. Install the dependencies from `requirements.txt`.
2. Prepare the input dataset according to the expected notebook structure.
3. Run the relevant preprocessing steps.
4. Execute the selected modeling notebook.
5. Compare model outputs using the statistical evaluation workflow.

> **Note:** The original research dataset may not be publicly distributed due to data-access, privacy, or platform-related restrictions. A sample or anonymized dataset can be provided separately when appropriate.

---

# 🌍 Potential Applications

The framework can be adapted to several computational social science and NLP applications, including:

* Social media discourse analysis
* Public opinion analysis
* Crisis communication research
* Environmental discourse analysis
* Political communication
* Risk communication
* Trend detection
* Persian NLP research
* Computational social science

---

# ✨ Key Contribution

The main contribution of this project is the integration of **traditional topic modeling, semantic embeddings, transformer-based representations, network analysis, temporal modeling, and statistical comparison** within a single Persian NLP workflow.

This enables social media discourse to be examined from multiple perspectives:

**lexical → semantic → structural → temporal → statistical**

---

# 🚧 Future Development

Future extensions may include:

* BERTopic-based topic discovery
* Sentence Transformer embeddings
* Automated hyperparameter optimization
* Interactive topic visualization
* Dynamic topic modeling
* LLM-assisted topic interpretation
* Cross-lingual topic comparison
* Automated NLP pipelines

---

# 👩‍💻 Author

### Mona Faghfouri Azar

**Data Analyst | NLP & AI Researcher**

Research interests include:

`Natural Language Processing` · `Artificial Intelligence` · `Computational Social Science` · `Social Media Analytics` · `Network Analysis`

GitHub: [MonaFaghfouri](https://github.com/MonaFaghfouri)

---

# 📚 Citation

If you use this repository or build upon its methodology, please cite the project:

```bibtex
@software{faghfouri_persian_topic_modeling,
  author = {Faghfouri Azar, Mona},
  title = {Persian Social Media Topic Modeling and Semantic Network Analysis},
  url = {https://github.com/MonaFaghfouri/Topic_Modeling},
  year = {2026}
}
```

---

<p align="center">
  <b>⭐ If you find this project useful, consider giving the repository a star.</b>
</p>

<p align="center">
  Built for research in NLP, AI and Computational Social Science.
</p>
