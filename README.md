# 🛡️ Comment Moderator - Offline Comment Filtering using Local LLM

This project is a **comment moderation system** that detects and flags **offensive, toxic, or profane comments** from a dataset using a **local AI model**—no API key required.

---

## 🔍 Features

- ✅ Detects offensive language using a pre-trained local model
- 🔥 Uses `transformers` pipeline for comment classification
- 🚫 Flags profanity using `better_profanity`
- 📊 Generates a report and a bar chart for offense types
- 📁 Supports CSV input and Excel output

---

## 🧠 How It Works

1. Loads comments from a CSV file
2. Analyzes each comment:
   - Checks for **profanity**
   - Uses a **local model** to classify comments as `toxic`, `hate speech`, etc.
3. Generates:
   - A CSV of flagged comments
   - A bar chart showing offense distribution

---

## 📂 Project Structure
COMMENT_MODERATOR/ │ ├── main.py # Entry point ├── comment_analyzer.py # Local classification logic ├── utils.py # Helper for plotting ├── sample_data/ │ └── comments.csv # Input comments ├── output/ │ ├── flagged_comments.xlsx # Output flagged comments │ └── offense_distribution.png ├── requirements.txt ├── .env # Optional env file (not needed for local LLM) └── README.md
