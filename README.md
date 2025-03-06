# Data-acquisition-extraction-and-storage-project
This is a group project that completed by Kanupriya Jain, Nan An and Othman Hicheur


Project Proposal
Dataset creation using Research Papers
Team Members:
Kanupriya Jain
Othman Hicheur
Nan An
1 Objective and Data Sources
Our project will involve researh papers published on arXiv and Google Scholar. We might refer to some external
sources as well for cross referencing. The main idea is to crawl these websites and extract relevant metadata to
analyze trends over time. This extracted data can also be utilized for analyzing how certain topics changed over
time. So, the data sources are scientific publications. Our primary goal is to develop well structured data that
can be useful for tasks such as training,visualization for data exploration etc.
2 Data Crawling and Extraction
2.1 Data Extraction
We would like to extract the following things -
• Title of the research paper
• Authors
• Year of publication
• Main research fields
• Abstract of the paper
• Number of citations
• Keywords
From each paper,we want to extract the abstract and transform the abstract in order extract more meaningful
features (using some machine learning model) that might be helpful in trend analysis and data exploration in general.
We have not decided on approach yet but we have some ideas. For example, we can use some NLP driven approach
or we can cluster similar paper together to create a hierarchical structure of topics and subtopics.
3 Data Cleaning
Cleaning process will include the following tasks -
• Handling Missing Data: Missing data can be filled either manually or exclusion of the corresponding research
paper.
• Handling duplicate data: We will identify and remove data duplicates.
• Structuring Data: We will structure our data well maintaining uniformity across different fields of the
dataset.
4 Data Storage:
We want to keep the structured dataset on NoSQL database (eg,PostgreSQL) because it will be able to handle various
data types easily providing more flexibility.
1
5 Applications
The final well structured dataset can be used for several applications such as-
• Trend analysis (e.g., identifying popular topics over time) using histograms for each year
• Extracting the most popular paper and author by using number of citations.
• Key words can be used to analyze the popular subfields emerging in a particular field and how it changed over
time.
• Intersections between different fields can also be analyzed over the years
• Hierarchical structure of topics and subtopics can also be craeted
