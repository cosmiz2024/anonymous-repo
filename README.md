
# README.md

## BERTopic Analysis and Visualization Project

### Overview
This project provides a comprehensive pipeline for topic modeling and analysis using BERTopic. The focus is on clustering textual data, analyzing clusters, extracting meaningful insights, and visualizing results. It also includes steps for preprocessing data, evaluating topic quality, and extracting metadata such as domain and TLD from URLs. The final outputs include visualizations, enriched datasets, and topic coherence scores.

### Key Features
- **Data Preprocessing**: Cleaning and preparing text data for analysis, including tokenization, lemmatization, and stopword removal.
- **Topic Modeling**: Using BERTopic to group text into topics based on semantic similarity.
- **Topic Evaluation**: Calculating coherence scores to evaluate the quality of topics.
- **Visualization**: Interactive and static visualizations of topics, including hierarchy, document distribution, and word clouds.
- **Domain and TLD Extraction**: Enriching datasets by extracting and appending domain and top-level domain (TLD) information from URLs.
- **Cluster Analysis**: Quantifying and analyzing the distribution of documents across clusters.

### Workflow
1. **Data Preparation**:
   - Upload and load datasets using Pandas.
   - Perform text preprocessing, including cleaning, tokenization, lemmatization, and stopword removal.

2. **BERTopic Application**:
   - Fit the BERTopic model to the preprocessed data.
   - Assign topics to each text document and extract the most representative words for each topic.

3. **Topic Quality Evaluation**:
   - Calculate coherence scores for each topic using Gensim's `CoherenceModel`.
   - Visualize topic coherence scores as a bar chart.

4. **Visualizations**:
   - Generate hierarchical topic structures using BERTopic's `visualize_hierarchy()`.
   - Display document distribution across topics with `visualize_barchart()`.
   - Create word clouds for each topic to highlight dominant words.

5. **Cluster Analysis**:
   - Analyze the size of each topic cluster by counting documents per cluster.
   - Visualize cluster sizes with bar charts.

6. **Domain and TLD Extraction**:
   - Extract domains and TLDs from URLs.
   - Populate missing domain and TLD fields in the dataset.

7. **Exporting Results**:
   - Save updated datasets to CSV files.
   - Automatically download results for local use when running in Google Colab.

### Key Scripts
- **Preprocessing**: 
  - Prepares text data by cleaning, tokenizing, and lemmatizing, ensuring consistency across the dataset.
- **Topic Modeling**: 
  - Uses BERTopic to discover topics and assign them to text documents.
- **Coherence Evaluation**: 
  - Measures the quality of topics using `c_v` coherence scores.
- **Visualization**: 
  - Produces hierarchical visualizations, bar charts, and word clouds to illustrate topic characteristics.
- **Domain and TLD Extraction**: 
  - Parses and extracts domain and TLD information from raw URLs for metadata enrichment.

### Visualizations
- **Topic Hierarchy**: Displays relationships between topics in a tree-like structure.
- **Document Distribution**: Bar charts showing the number of documents per topic.
- **Word Clouds**: Highlighting dominant words in each topic.
- **Coherence Scores**: Bar charts representing the coherence scores for each topic.

### Files
- `Smishiviz_code.ipynb`: Handles text preprocessing tasks, Contains the main BERTopic modeling and visualization logic, Extracts and processes domain and TLD information from URL
- `graph_generator.ipynb`: Generate JSON code to feed D3js graph visualization tool
- `graph.json`: Example of generated json file
- `campaign-operations.html`:Example of Visualization of graph with D3js


### How to Use
1. **Setup**:
   - Clone the repository.
   - Install necessary dependencies (e.g., `bertopic`, `gensim`, `matplotlib`, `pandas`).
   - Ensure your dataset is available in CSV format.

2. **Run the Pipeline**:
   - Execute the scripts step-by-step or run the provided Jupyter Notebook.
   - Inspect intermediate outputs for accuracy and insights.



### Dependencies
- Python 3.8+
- Libraries:
  - `pandas`
  - `bertopic`
  - `matplotlib`
  - `gensim`
  - `nltk`
  - `wordcloud`
  - `spacy`
  - `urllib`


