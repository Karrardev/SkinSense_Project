SkinSense

SkinSense is a simple, rule-based skin assessment tool created for the Machine Learning 2 course (Group Project 1).  
It guides users through a short questionnaire about their skin habits and concerns, then generates a skin type classification and basic skincare routine using a scoring system.  
**No machine learning is used**—instead, it relies on straightforward heuristics that can be easily explained.

## Features

- **Interactive questionnaire:** A Streamlit web app with 12 questions about skin condition, habits, and environment.  
- **Rule‑based scoring engine:** Calculates dryness, oiliness, acne, barrier, and sensitivity scores.  
- **Skin type determination:** Classifies into Dry, Oily, Combination, or Normal and appends a “Sensitive” tag if needed.  
- **Concern prioritization:** Highlights the top two skin concerns based on scores.  
- **Routine recommendations:** Provides simple morning (AM) and evening (PM) routines tailored to the user’s scores.  
- **Ingredient suggestions:** Lists helpful ingredients and cautions based on skin needs.  
- **Downloadable summary:** Lets users download a text file of their results and routine.  
- **Transparent logic:** Every recommendation comes from explicit rules; nothing is a black box.

## Installation

1. Clone or download this repository.  
2. Ensure you have Python 3.8 or newer installed.  
3. (Optional) Create a virtual environment:

   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

4. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

Run the Streamlit app from the project folder:

```bash
streamlit run app.py
```

The app will open in your default web browser (usually at `http://localhost:8501`).  
Answer all the questions, and your results and recommendations will appear.  
You can click the **“Download your routine”** button to save a text summary of your skin type and routine.

## Files

- `app.py` – Main Streamlit application that implements the questionnaire, scoring engine, and recommendations.  
- `requirements.txt` – List of Python packages required to run the app (Streamlit only).  
- `technical_documentation.md` – Short technical documentation including architecture overview and a data flow diagram.  
- `progress_log.md` – Logs of development activities.  
- `AI_use_statement.md` – Explanation of how AI was used to assist in this project.  
- `group_contract.md` – Template group contract outlining team roles and expectations.

## Statement of AI Use

This project was developed with assistance from an AI language model (ChatGPT).  
The AI was used to help brainstorm ideas, draft the questionnaire, design the scoring logic, and generate initial code structure and documentation templates.  
All AI‑generated outputs were reviewed and edited by the student to ensure understanding and suitability for the course.  
The final code and documentation were vetted for correctness and clarity.

## Disclaimer

SkinSense is intended for educational purposes and should not be used as a substitute for professional dermatological advice.  
Always consult a healthcare provider for serious skin concerns.
