## Movie Recommendation System using Machine Learning

## Project Overview

This project is a **Content-Based Movie Recommendation System** built using Machine Learning techniques. It recommends movies similar to a user’s input by analyzing movie metadata such as genres, keywords, tagline, cast, and director.

The system uses **TF-IDF Vectorization** and **Cosine Similarity** to find and rank similar movies.

---

##  Key Features

*  Content-based recommendation system
*  Uses fuzzy matching to handle incorrect movie names
*  TF-IDF based feature extraction
*  Cosine similarity for accurate recommendations
*  Recommends top 30 similar movies

---

##  Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Scikit-learn**
* **difflib (for fuzzy matching)**

---

##  Dataset

The dataset used (`movies.csv`) contains the following features:

* Title
* Genres
* Keywords
* Tagline
* Cast
* Director

 *Note:* Missing values are handled by replacing them with empty strings.

---

##  How the System Works

### 1. Data Preprocessing

* Selected important features:

  * genres
  * keywords
  * tagline
  * cast
  * director
* Filled missing values with empty strings

### 2. Feature Engineering

* Combined selected features into a single text column

### 3. Text Vectorization

* Applied **TF-IDF Vectorizer** to convert text into numerical vectors

### 4. Similarity Calculation

* Used **Cosine Similarity** to measure similarity between movies

### 5. Movie Matching

* Used `difflib.get_close_matches()` to find closest movie name entered by user

### 6. Recommendation

* Sorted movies based on similarity score
* Displayed **Top 30 recommended movies**

---

##  How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/movie-recommendation-system.git
cd movie-recommendation-system
```

### 2. Install Dependencies

```bash
pip install pandas numpy scikit-learn
```

### 3. Run the Script

```bash
python your_script_name.py
```

### 4. Provide Input

```bash
Enter your favourite movie name: Avatar
```

---

##  Example Output

```
Movies Recommendation for you:

1. Guardians of the Galaxy
2. Star Trek
3. Avengers
...
```

---

##  Project Structure

```
movie-recommendation-system/
│── movies.csv
│── movie_recommendation.ipynb
│── README.md
```



