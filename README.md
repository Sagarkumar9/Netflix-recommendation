# Netflix-recommendation
Modern streaming platforms like Netflix rely heavily on content‑based recommendation systems. This project replicates that idea using the publicly available Netflix dataset.
Netflix Content‑Based Recommendation System
A machine‑learning project that builds two recommendation engines using the Netflix titles dataset:

Netflix‑style “Because you watched…” recommender

“Why this, not that” explanation system

This project uses content metadata (description, genres, cast size, country, rating group, seasons, runtime) to recommend similar titles and explain why they were recommended.

1. Content‑Based Recommender
Given a title (e.g., Kota Factory), the system finds the most similar titles using:

TF‑IDF description vectors

Genre multi‑hot encoding

Country one‑hot encoding

Rating group encoding

Numeric metadata (runtime, seasons, cast size, description length, number of genres)

Similarity is computed using cosine similarity or KNN nearest neighbors.

2. “Why This, Not That” Explanation System
This layer explains why a recommended title is similar.

It compares:

Shared genres

Shared countries

Shared rating groups

Similar cast sizes

Similar number of seasons

Overlapping TF‑IDF keywords in descriptions

Project Structure:
├── data/
│   └── clean/
│       ├── titles_clean.csv
│       ├── genres.csv
│       └── countries.csv
├── recommender.ipynb
├── README.md
└── requirements.txt


Author
B Sagar Kumar 
Machine Learning & Data Science Enthusiast
