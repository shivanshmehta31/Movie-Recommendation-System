# Movie Recommendation System using AutoEncoders

This repository contains an implementation of a **Movie Recommendation System** using **AutoEncoders** and the **MovieLens dataset**. The model is trained on user-movie ratings to generate personalized movie recommendations.

## 📂 Repository Structure

```
📁 Movie-Recommendation-System
│── 📄 README.md            # Project documentation
│── 📄 AutoEncoders.ipynb   # Jupyter Notebook implementing the AutoEncoder model
│── 📄 ml.1m/               # MovieLens 1M dataset
│   ├── ratings.dat         # User ratings
│   ├── users.dat           # User demographic data
│   ├── movies.dat          # Movie metadata
│── 📄 ml.100k/             # MovieLens 100K dataset (alternative dataset)
│   ├── u.data              # User ratings
│   ├── u.user              # User demographic data
│   ├── u.item              # Movie metadata
```

## 📊 Dataset

The **MovieLens** dataset consists of user ratings for movies, along with demographic data and movie metadata.

- **MovieLens 1M (`ml.1m`)**: Contains **1,000,209** ratings from **6,040** users on **3,900** movies.
- **MovieLens 100K (`ml.100k`)**: Contains **100,000** ratings from **943** users on **1,682** movies.

Each rating is on a **1-5 star** scale. Users have rated at least **20 movies** each.

### 📜 Data Files
- **ratings.dat** (UserID, MovieID, Rating, Timestamp)
- **users.dat** (UserID, Gender, Age, Occupation, Zip-code)
- **movies.dat** (MovieID, Title, Genres)

For more details, visit [MovieLens](https://grouplens.org/datasets/movielens/).

## 🏗 Model Implementation

The `AutoEncoders.ipynb` notebook contains the following steps:

- Data Preprocessing (handling missing values, normalizing ratings, etc.)
- Creating the **AutoEncoder-based** collaborative filtering model
- Training and evaluating the model
- Making movie recommendations for users

## 🔧 How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Movie-Recommendation-System.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook "AutoEncoders.ipynb"
   ```
4. Run the notebook to train the model and generate recommendations.

## 📌 Future Improvements

- Experiment with different **Neural Network architectures**.
- Incorporate **content-based filtering** alongside collaborative filtering.
- Deploy the model as a **web application** using Flask or FastAPI.

## 🏛 License & Citation

This project uses the **MovieLens dataset**, which is provided by **GroupLens Research**. If you use the dataset, cite:

```
F. Maxwell Harper and Joseph A. Konstan. 2015. The MovieLens Datasets: History
and Context. ACM Transactions on Interactive Intelligent Systems (TiiS) 5, 4,
Article 19 (December 2015), 19 pages. DOI=http://dx.doi.org/10.1145/2827872
```

For more details, visit [GroupLens Research](https://www.grouplens.org/).
