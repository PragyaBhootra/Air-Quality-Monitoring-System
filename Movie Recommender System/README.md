# **Movie Recommendation System**

## **Overview**
This project implements a movie recommendation system that suggests movies similar to a given input. It uses **TF-IDF Vectorization** and **cosine similarity** to calculate the similarity between movie descriptions or features.

---

## **Features**
- Calculates similarity between movies using textual data.
- Sorts movies based on similarity scores.
- Recommends a list of the most similar movies.

---

## **Requirements**
| Library        | Version (Recommended) |
|----------------|------------------------|
| scikit-learn   | Latest                 |
| pandas         | Latest                 |
| NumPy          | Latest                 |
| Python         | 3.x                    |

---

## **Project Structure**
1. **Data Loading**:
   - Loads the dataset containing movie titles and features.
2. **Feature Engineering**:
   - Combines relevant text features into a single feature for similarity calculations.
3. **Similarity Calculation**:
   - Uses TF-IDF vectorization to convert text features into numerical vectors.
   - Computes cosine similarity between feature vectors.
4. **Recommendation**:
   - Sorts movies based on similarity scores and displays top suggestions.

---



