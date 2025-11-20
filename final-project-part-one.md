| [home page](https://nikki-lemon.github.io/nikki-chen-portfolio/) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |


# Outline

## High-level summary

In this project, I will explore how users think about their own preferences before they watch a movie. The MovieLens Beliefs Dataset includes both the ratings that users *predict* for movies they have not seen, and the ratings they later *give* after watching these movies. This allows me to study the pattern of expectation versus experience. I will focus on the Romance genre because this genre often involves emotional expectations, and users may form stronger opinions before watching compared to other genres.

The goal of my project is to show how often users misjudge their interest in Romance movies, and how large this bias can be. I also compare user predictions with the system’s predicted ratings from MovieLens to understand when the recommendation system predicts better than the users themselves, and when the system needs improvement. Through several visualizations, I want to build a clear story that explains how these mismatches happen, why they matter, and what the recommendation team can learn from them.

---

## Project structure

### Summary
Users often mispredict how much they will enjoy Romance movies, and this mismatch can affect their satisfaction with the recommendation system.

### User stories
- As a product manager, I want to understand when user expectations do not match real ratings so I can reduce negative user experiences.  
- As a data scientist, I want to compare user prediction error with system prediction error so I know where the algorithm performs better or worse.  
- As a designer, I want to understand if user confidence is a useful signal when predicting future behavior.

### Story arc

**Opening:**  
Introduce the Romance genre and show the overall difference between predicted ratings and actual ratings. This builds the foundation of the story by showing that expectation mismatch exists.

**Rising tension:**  
Show that the prediction error varies across users. Some users overestimate, some underestimate, and others are unsure. Also show that confidence does not always lead to better predictions. These patterns increase the tension and show why the problem is important.

**Climax (key insight):**  
Compare user prediction error with system prediction error. Highlight the key insight: in some cases, the recommendation system predicts Romance movie ratings better than the users, even when the users feel confident. This reveals a gap between intuition and data-driven prediction.

**Resolution:**  
Explain what these insights could mean for the recommendation team. Suggest how these findings can improve ranking strategies, support exploration, or refine personalization methods. End with the idea that understanding prediction bias is useful for improving long-term satisfaction.

---

## Initial sketches

<div style="display: flex; justify-content: space-between;">
  <img src="https://raw.githubusercontent.com/nikki-lemon/nikki-chen-portfolio/main/sketch_1.png" height="220">
  <img src="https://raw.githubusercontent.com/nikki-lemon/nikki-chen-portfolio/main/sketch_2.png" height="220">
  <img src="https://raw.githubusercontent.com/nikki-lemon/nikki-chen-portfolio/main/sketch_3.png" height="220">
</div>

<br>

<div style="display: flex; justify-content: space-between;">
  <img src="https://raw.githubusercontent.com/nikki-lemon/nikki-chen-portfolio/main/sketch_4.png" height="220">
  <img src="https://raw.githubusercontent.com/nikki-lemon/nikki-chen-portfolio/main/sketch_5.png" height="220">
  <img src="https://raw.githubusercontent.com/nikki-lemon/nikki-chen-portfolio/main/sketch_6.png" height="220">
</div>

---

# The data

The primary data source for this project is the **MovieLens Beliefs Dataset (2024)**. The dataset is publicly available on the GroupLens website at the link below. It contains movie metadata, user rating history, belief elicitation responses, recommendation logs, and the set of movies that were shown to users during the belief process. I will mainly use three files: `movies.csv`, `belief_data.csv`, and `user_rating_history.csv`.

## Dataset links

| Name | URL | Description |
|------|-----|-------------|
| MovieLens Beliefs Dataset (2024) | https://grouplens.org/datasets/movielens/ml_belief_2024/ | Public dataset providing predicted ratings, actual ratings, certainty, and system predictions. |
| Processed dataset for this project | *(Link to be added after upload)* | Filtered dataset containing only Romance movies and merged belief–rating records. |

---

# Method and medium

I plan to complete my final project using **Shorthand** as the main storytelling platform and **Tableau** for all data visualizations. I will also use Python to clean and merge the dataset before importing it into Tableau.

---

## References

- MovieLens Beliefs Dataset (2024), GroupLens Research  
  https://grouplens.org/datasets/movielens/ml_belief_2024/
