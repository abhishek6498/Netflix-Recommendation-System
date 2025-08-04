# Netflix Recommendation System 🎬📊

This project builds a collaborative filtering-based movie recommendation system using Netflix’s user rating data. It uses Singular Value Decomposition (SVD) via the `Surprise` library to generate personalized movie recommendations.

---

## 📁 Dataset

The dataset consists of user ratings for movies, extracted from the Netflix Prize data:
- `combined_data_1.txt`: Contains user IDs and ratings for various movies (⚠️ ~472 MB).
- `movie_titles.csv`: Contains movie metadata (Movie ID, Year, Title).

> Note: Due to file size limits, `combined_data_1.txt` is not hosted on GitHub. You can download it [from here](https://drive.google.com/file/d/1--JGb9rLK2VpC60spIjwF6aJoAhieCUV/view?usp=sharing, https://drive.google.com/file/d/1agNJSJDrNg83rEeM5mxjakDqKeTk0kpV/view?usp=sharing)) and place it in the project folder.

---

## 🚀 Project Features

- Load, clean, and preprocess sparse Netflix ratings data.
- Trim dataset to the top 30% most active users and movies for better performance.
- Build a **User-Item Ratings Matrix**.
- Train an SVD model using the **Surprise** library.
- Evaluate model performance using **RMSE** and **MAPE**.
- Generate personalized movie recommendations for a specific user.

---

## 📈 Model Performance

- Algorithm: **Singular Value Decomposition (SVD)**
- Evaluation Metrics:
  - **RMSE**: Calculated using 5-fold cross-validation
  - **MAPE**: Achieved **22.3%**
