# Startup Health Scoring Model

Hi, I'm Sakshi Vedi  
The goal is to evaluate and rank startups based on key business metrics like team strength, market size, traction, funding, and burn rate.

---

## About the Project

This model scores 100 startups using a custom formula that reflects their overall business health and growth potential. Each feature is normalized using Min-Max scaling, and a weighted scoring system is applied to rank the startups from best to worst.

### Features Used:
- Team Experience
- Market Size (USD)
- Monthly Active Users
- Funds Raised (INR)
- Monthly Burn Rate (INR) → *inverted, since lower burn is better*

---

## Scoring Formula

| Feature                | Weight |
|------------------------|--------|
| Team Experience        | 15%    |
| Market Size            | 25%    |
| Monthly Users          | 25%    |
| Funds Raised           | 15%    |
| Burn Rate (Inverted)   | 20%    |

The score is calculated as a weighted sum and scaled out of 100.

---

## How to Run
# Step 1: Navigate to project folder
cd path/to/startup_scoring

# Step 2: Install required libraries
pip install -r requirements.txt

# Step 3: Run the full pipeline
python main.py


## Visualizations
Bar chart of all startup scores

Histogram of score distribution

Correlation heatmap of input features
