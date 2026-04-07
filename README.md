# Grade Predictor Flask App

A Flask web app that calculates required midterm and final grades needed to pass (75%) or achieve Dean's Lister (90%) based on your prelim grade.

---

## How It Works

1. Enter your prelim grade (0-100)
2. Click calculate
3. Get required grades for midterm and finals

---

## Grading Weights

Prelim: 20%
Midterm: 30%
Final: 50%

---

## Formulas Used

Current Total = Prelim Grade x 0.20

Required Total to Pass = 75 - Current Total
Required Average = Required Total / (0.30 + 0.50)

Required Total for Dean's Lister = 90 - Current Total
Required Average for Dean's Lister = Required Total / (0.30 + 0.50)

---

## Messages

If Prelim Grade is below 70:
- "It is Difficult to Pass!"
- Dean's Lister message based on feasibility

If Prelim Grade is 70 or above:
- "You Have a Chance to Pass!"
- Dean's Lister message based on feasibility

---

## Installation

pip install flask
python app.py

---

## Project Structure

grade-predictor/
├── app.py
├── templates/
│   └── index.html
└── README.md

---

## Routes

/ (GET) - Shows calculator form
/ (POST) - Calculates required grades

---

## Built With

- Flask (Python)
- HTML/CSS

---

## License

MIT
