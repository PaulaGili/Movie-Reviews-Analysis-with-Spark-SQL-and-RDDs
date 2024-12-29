# 🎬 Movie Reviews Analysis with Spark SQL and RDDs

## 📖 Project Overview
This project utilizes **Apache Spark** to analyze heterogeneous datasets from multiple sources. It focuses on movie-related data sourced from [IMDB](https://www.imdb.com/), including user reviews and detailed movie information. By leveraging **SparkSQL**, **RDDs**, and **DataFrames**, it aims to uncover insights, handle complex data structures, execute advanced SQL queries, and effectively visualize trends.

The main objective is to perform a series of technical analyses to extract meaningful knowledge. These operations include analyzing structured data, identifying patterns, visualizing trends, and comparing values across datasets.

---

##  Project Structure

The project is divided into the following key stages:

### 1️⃣ Environment Initialization and Data Loading
- **Environment Setup**:
  - Configure the **Apache Spark** environment.
  - Ensure all dependencies are installed and the environment is optimized for distributed data processing.

- **Data Loading**:
  - Import JSON files from **HDFS** stored in `/aula_B0.485/data/`.
  - Perform initial data exploration:
    - Validate schemas.
    - Inspect for null or inconsistent values.

### 2️⃣ Data Exploration and Transformation
- **Datasets**:
  - **`movie_details`**: Contains metadata like title, genre, release year, and ratings.
  - **`reviews`**: Includes user reviews, ratings, and spoiler flags.

- **Key Operations**:
  - Extract and inspect critical fields such as `movie_id`, `rating`, and `genre`.
  - Utilize **RDDs** for fine-grained data control and **DataFrames** for structured analysis.
  - Handle data partitioning for efficient processing.

### 3️⃣ Advanced Queries and Insights
- **SQL Queries**:
  - Use **SparkSQL** to execute structured queries directly on the data.

- **Key Analyses**:
  - **Rating Distribution**: Examine the spread of ratings across movies.
  - **Top Reviewers**: Identify users with the most reviews and analyze spoiler tendencies.
  - **Rating Discrepancies**: Compare rating inconsistencies between datasets.
  - **Metrics Calculation**: 
    - Average movie age by genre.
    - Proportion of spoilers for specific genres like action.

### 4️⃣ Data Visualization
- **Tools**:
  - Use **Matplotlib** to create clear, visually appealing plots.
  
- **Visual Insights**:
  - Rating distributions.
  - Yearly trends in movie releases.
  - Genre-specific analyses, such as average ratings and spoiler proportions.

---

## ⚙️ Technologies Used

| Technology       | Purpose                                |
|-------------------|----------------------------------------|
| **Apache Spark**  | Distributed processing of large datasets. |
| **HDFS**          | Distributed file system for input data storage. |
| **PySpark SQL**   | SQL-like query execution for structured data. |
| **Matplotlib**    | Generating data visualizations.        |

---

## 📊 Key Results and Insights

1. **Movies with High Ratings**:
   - Identified **276 movies** with ratings above **8**.

2. **Rating Distribution**:
   - Created visual representations of rating distributions across all movies.

3. **Most Active Users**:
   - Found the most active user, `ur4248714`, with the highest number of reviews.
   - Analyzed less active users to understand engagement trends.

4. **Inconsistent Ratings**:
   - Detected discrepancies in ratings between movie details and user reviews datasets.

5. **Genre-Based Analysis**:
   - Spoiler proportions for action movies: **28.26%**.
   - Average age difference between horror and action movies: **~1.68 years**.

6. **Average Ratings by Genre**:
   - Computed average ratings for each genre, providing insights into audience preferences.

7. **Top Movie Release Years**:
   - Highlighted the top **10 years** with the highest number of movies released.
