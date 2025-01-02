# Customer Satisfaction Topic Modeling Analysis

This project explores customer satisfaction within the e-commerce domain, specifically analyzing reviews related to women's clothing. The analysis employs Structural Topic Modeling (STM) to identify latent topics within customer reviews and their relationship with customer satisfaction ratings. The methodology includes data preprocessing, topic modeling, and the extraction of actionable insights from customer reviews.

## Methodology

### 1. Data Preprocessing

The data preprocessing phase involved several steps to ensure the dataset was suitable for modeling and analysis.

#### 1.1. Inspection and Cleaning
- **Missing Values and Outliers**: The dataset was examined for missing values, outliers, and inconsistencies to ensure data quality.
- **Text Cleaning**: The raw review text (Review Text column) was cleaned to remove unnecessary noise, such as punctuation, special characters, and excessive whitespace, producing the `Clean Text` column.

#### 1.2. Tokenization and Text Processing
- **Tokenization**: The cleaned text was tokenized, breaking sentences into individual words, stored in the `Token Text` column.
- **POS Tagging**: Part-of-speech tagging was applied to label each token with its grammatical role, producing the `POS Tagged` column.
- **Stopword Removal & Lemmatization**: Stopwords and irrelevant tokens were removed, and stemming or lemmatization was performed to ensure consistent word forms, resulting in the `Final Text` column.

#### 1.3. Feature Extraction
- **Word Count**: A `Word Count` column was added to quantify the length of each review, facilitating further analysis on verbosity and its relation to satisfaction ratings.
- **Categorical Features**: Structured attributes such as `Rating`, `Recommended IND`, `Division Name`, `Department Name`, and `Class Name` were retained for use in the modeling phase.

### 2. Topic Modeling with Structural Topic Model (STM)

The primary objective of this analysis was to identify underlying themes in customer reviews using the STM framework.

#### 2.1. Text Preprocessing for STM
The processed text data from the `Final Text` column, along with relevant metadata (e.g., `Rating`), was passed through the `textProcessor` function to prepare the data for STM analysis. This function performed:
- Tokenization
- Vocabulary cleaning
- Alignment of metadata with the text

#### 2.2. Document Preparation
The prepared data was then fed into the `prepDocuments` function, which structured the input documents, vocabulary, and metadata required for STM analysis.

#### 2.3. Fitting the STM Model
- **Model Configuration**: An STM model was fit with 5 topics, using the `Rating` column as a prevalence covariate. This setup enabled the model to capture how different topics are associated with varying levels of customer satisfaction.
  
### 3. Analysis and Interpretation of Topics

After fitting the STM model, the results were analyzed using the `labelTopics` function. Key metrics for each topic were extracted:
- **Highest Probability Words**: The most likely words associated with each topic.
- **FREX Words**: Words that are both frequent and exclusive to a given topic.
- **Lift Words**: Words that are distinctive and unique to the topic compared to other topics.

These key terms provided insight into the underlying themes driving customer satisfaction. The relationship between topics and ratings revealed critical factors influencing customer satisfaction with women’s clothing in the e-commerce context.

## Key Insights

The analysis provided actionable insights into customer satisfaction, focusing on:
- Common themes in high-rated reviews.
- The correlation between specific topics and satisfaction ratings.
- Factors driving customer satisfaction in the online clothing retail space.

## Installation and Setup

### Prerequisites

This project requires the following Python libraries:
- `numpy`
- `pandas`
- `stm`
- `nltk`
- `sklearn`



