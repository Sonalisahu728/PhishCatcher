# 🎣 PhishCatcher
### Client-Side Defense Against Web Spoofing Attacks Using Machine Learning

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)
![XGBoost](https://img.shields.io/badge/XGBoost-99%25_Accuracy-brightgreen?style=for-the-badge)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange?style=for-the-badge&logo=scikit-learn)
![BPUT](https://img.shields.io/badge/BPUT-Final_Year_Project_2026-red?style=for-the-badge)

---

## 🚀 Live Demo
👉 **[View Live Site](https://sonalisahu728.github.io/PhishCatcher)**

---

## 📌 About The Project

**PhishCatcher** is a machine learning-based phishing URL detection system that classifies any given URL as **Safe** or **Phishing** in real-time — without inspecting the webpage content at all.

It works purely by analyzing the **structural features of the URL** — length, dots, hyphens, special characters, HTTPS usage, and more — to catch phishing attacks before the user even visits the site.

> 🏆 Achieved **99% accuracy** using XGBoost — the best among all tested models.

---

## 📊 Model Performance

| Algorithm | Accuracy | Precision | Recall | F1 Score |
|-----------|----------|-----------|--------|----------|
| SVM (Baseline) | 96% | 95.8% | 95.2% | 95.5% |
| Random Forest | 98% | 97.9% | 97.7% | 97.8% |
| **XGBoost ⭐** | **99%** | **98.9%** | **98.8%** | **98.9%** |

---

## ⚙️ How It Works

1. **URL Parsing** — Split URL into protocol, domain, path, query, fragment using urllib.parse
2. **Feature Extraction** — Extract 17+ structural signals per component
3. **Normalization** — Scale all features to [0,1] using MinMaxScaler
4. **Classification** — XGBoost model predicts: Legitimate or Phishing

---

## 🧪 Features Extracted

| Feature | Description |
|---------|-------------|
| URL Length | Longer URLs often indicate phishing |
| Dot Count | Excess dots signal subdomain abuse |
| Hyphen Count | Hyphens used to mimic real brands |
| @ Symbol | Forces browser to ignore preceding text |
| HTTPS | HTTP-only sites are more likely phishing |
| IP Address | Raw IP in URL is a red flag |
| Query Params | Excessive params common in phishing |
| Subdomain Depth | Deep subdomains are suspicious |
| Slash Count | Deep paths used to hide endpoints |

---

## 🛠️ Tech Stack

- **Language** — Python 3
- **ML Models** — SVM, Random Forest, XGBoost
- **Libraries** — scikit-learn, pandas, NumPy, Matplotlib, Seaborn
- **Dataset** — PhishTank (phish_tank_storm.csv)
- **Tools** — Jupyter Notebook, pickle, urllib.parse

---

## 👥 Team — Group 29

| Name | Role |
|------|------|
| Ashwini Kumar Bisoyi | ML Pipeline · Model Training |
| Gopal Sahu | Feature Engineering · Dataset |
| Sonali Sahu | Research · Documentation |
| Sagar Gouda | Evaluation · Testing |

> B.Tech CSE · BPUT · Final Year Major Project · 2026
> 🏅 **Project Score: 10/10 SGPA**

---

## 📄 License

This project was built for academic purposes under BPUT university guidelines.

---

Made with ❤️ by Group 29 · PhishCatcher 2026

