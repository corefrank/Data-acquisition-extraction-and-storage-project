# Data-acquisition-extraction-and-storage-project
This is a group project that completed by Kanupriya Jain, Nan An and Othman Hicheur

## Team Members
- **Kanupriya Jain**
- **Nan An**
- **Othman Hicheur**

---
# Project Proposal
## 1. Objective and Data Sources

Our project focuses on extracting and structuring metadata from research papers published on **arXiv** and **Google Scholar**. Additional external sources may be used for cross-referencing. The main objectives are:

- **Crawling** these platforms to extract relevant metadata.
- **Analyzing trends over time** in scientific research.
- **Transforming extracted abstracts** into meaningful features using **Natural Language Processing (NLP)** techniques.
- **Creating a hierarchical structure** of research topics and subtopics.
- **Storing structured data** for further analysis, visualization, and machine learning tasks.

---

## 2. Data Crawling and Extraction

### 2.1 Data Extraction

We aim to extract the following metadata from each research paper:
- **Title** of the research paper
- **Authors**
- **Year of publication**
- **Main research fields**
- **Abstract**
- **Number of citations**
- **Keywords**

We also plan to process the **abstracts** further to extract key features. The methodology for this transformation is under consideration, but potential approaches include:
- **NLP-driven models** (e.g., TF-IDF, BERT embeddings, topic modeling)
- **Clustering similar papers** to build a hierarchical topic structure

### 2.2 Crawling Strategy

To ensure efficient and scalable data extraction, we will:
- Use **Scrapy** for web crawling.
- Implement **XPath/CSS selectors** for structured extraction.
- Handle **pagination** to crawl multiple pages.
- Implement **request throttling** to avoid bans.
- Store raw scraped data in **JSON format** before processing.

---

## 3. Data Cleaning

Cleaning the extracted data is crucial for ensuring its usability. Our data cleaning steps include:

- **Handling Missing Data:**
  - Fill missing values where possible.
  - Remove research papers with insufficient metadata.
- **Removing Duplicates:**
  - Identify and remove duplicate entries based on title, authors, and DOI (if available).
- **Standardizing Data Format:**
  - Ensure uniformity in field naming, date formats, and keyword representation.
  - Normalize author names and research fields for consistency.

---

## 4. Data Storage

We plan to store the structured dataset in a **NoSQL database**, such as **MongoDB**, due to its flexibility in handling unstructured and semi-structured data. 

- **Primary storage format:** JSON
- **Database choice:** MongoDB (preferred) or PostgreSQL (alternative)
- **Indexes:** Optimized for fast retrieval of research papers based on year, author, or keyword search

---

## 5. Applications

Once the dataset is cleaned and structured, it can be used for multiple applications, including:

- **Trend Analysis:**
  - Identifying popular research topics over time.
  - Generating histograms showing the rise and fall of research areas.
- **Author and Paper Popularity:**
  - Finding the most cited papers and authors.
- **Keyword-Based Analysis:**
  - Tracking emerging research subfields.
- **Field Intersections:**
  - Analyzing interdisciplinary research trends.
- **Topic Hierarchies:**
  - Clustering research papers into structured topics and subtopics.
