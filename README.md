# 🎬 YouTube Video Recommendation System using Deep Reinforcement Learning (DDQN)

This project implements a **personalized video recommendation system** using **Double Deep Q-Learning (DDQN)**.  
It simulates sequential user-video interactions and optimizes long-term engagement by going beyond traditional collaborative filtering and matrix factorization approaches.  

---

## 📌 Project Overview
- Built a **custom reinforcement learning environment** to model user–video interactions.  
- Designed a **DDQN agent** in PyTorch with epsilon-greedy exploration, experience replay, and reward shaping.  
- Compared performance against baselines such as **Non-negative Matrix Factorization (NMF)** and random recommendation.  
- Evaluated using **precision, recall, F1-score, and AUC**, demonstrating the effectiveness of RL for recommendation tasks.  

---

## 📊 Dataset
- **Source:** Trending YouTube video datasets (8 countries including US, IN, GB, CA).  
- **Features:** Video metadata (views, likes, dislikes, categories), country tags, user interaction history.  
- **Preprocessing:** Cleaning duplicates, handling encoding issues, enriching with contextual features.  

---

## ⚙️ Technical Workflow
1. **Data Preparation** – Aggregated, cleaned, and enriched datasets with categorical and numerical features.  
2. **Exploratory Data Analysis (EDA)** – Analyzed video categories, view counts, like/dislike ratios, and global content trends.  
3. **Baseline Model** – Implemented NMF for collaborative filtering as a benchmark.  
4. **RL Environment** – Defined state space (video metadata + user history), action space (video recommendations), and rewards (clicks, views, likes).  
5. **DDQN Implementation** – Built and trained agent with replay buffer, target network updates, and epsilon-greedy policy.  
6. **Evaluation** – Compared DDQN with NMF and random baselines across multiple metrics.  

---

## 📈 Key Visualizations
- Distribution of Views, Likes, and Dislikes (log scale)  
- Video Count by Category  
- Model Performance Comparison: DDQN vs. NMF vs. Random  

---

## 🛠️ Technologies Used
- **Python**  
- **PyTorch**  
- **Pandas, NumPy**  
- **Matplotlib, Seaborn**  
- **Reinforcement Learning (DDQN)**  
- **Non-negative Matrix Factorization (NMF)**  

---

## 🚀 Results
- DDQN outperformed both **NMF** and **Random** baselines in **precision, recall, F1, and AUC**.  
- Demonstrated RL’s ability to adapt to user behavior sequences and optimize recommendations over time.
