# movie-recommender-system
This project is a part of the course Big Data UE18CS322 at PES University. We make use of the MovieLens 25 Million dataset to make recommendations to users based on the Popularity model and Alternating Least Squares.  

Multiple versions of the project are available as you can see from the contents of this repository, but our final submission is available in the file [DefinitiveEdition.ipynb](https://github.com/vishnureddys/movie-recommender-system/blob/main/DefinitiveEdition.ipynb).  

## Main Requirements
```
1. Hadoop
2. Python
3. Jupyter Notebook 
4. PySpark
```

## Potential Improvements to our Recommender System

- Hybrid recommender systems: The major weakness of collaborative filtering is that forgoing the actual characteristics of items (for movies, meta-information such as genres, actor/actresses, director, country of origin) hurts both recommender accuracy and interpretability of recommendations. In practice, industrial recommender systems use hybrid approaches that combine both user similarity (collaborative filtering) and item characteristics (content-based approach).
- Reducing dataset size and user-item segmentation: One reason why our collaborative filtering model struggled to generate sound recommendations for all users is that our model training included every user (e.g. single rating users, users with few ratings or many ratings). A more ideal strategy would be to segment our ratings data into seperate but homogeneous user datasets and train different recommender systems on those separate data chunks, potentially improving our results.
- Buildng a flask app to collect user input and accordingly show the output to the user. 
