# 📊 Ad Campaign Performance Classifier
### Predicting digital ad campaign success — before the budget is spent

---

## Business Problem

Digital advertising platforms manage millions of active campaigns. Not all campaigns succeed — many waste budget due to poor targeting, weak creative, or suboptimal bidding strategies.

**Can we predict which campaigns will underperform — early enough to intervene?**

This project builds a machine learning classifier that predicts campaign success probability based on setup and early performance signals — and translates the model output into concrete product recommendations.

---

## Why I Built This

After 18 years running an ISP with 100,000+ subscribers and managing B2B client relationships at scale, I understand the advertiser's frustration firsthand: you invest in a campaign, spend real money, and only find out it failed *after* the budget is gone.

This project is my answer to that problem — built to demonstrate how AI and BI tools can proactively protect advertiser health at scale. It directly mirrors what Google's Customer Engagement and Advertiser BI teams build.

---

## Approach

**Dataset:** 5,000 simulated ad campaigns with 17 features reflecting real advertiser platform signals

**Models compared:**

| Model | Why |
|-------|-----|
| Logistic Regression | Interpretable baseline — fast, explainable |
| Random Forest | Captures non-linear feature interactions |
| Gradient Boosting | Best performance on structured tabular data |

**Evaluation metric:** ROC-AUC (we care about ranking campaigns by risk, not just binary accuracy)

---

## Key Findings

1. **Quality Score** is the single strongest predictor of campaign success
2. **Smart bidding** (Target CPA, Target ROAS) significantly outperforms manual CPC
3. **Negative keywords + ad extensions** are quick wins with outsized impact
4. Early flagging of at-risk campaigns could protect significant daily budget across the platform

---

## Product Recommendations

The model output feeds directly into three product features:

1. **Proactive Alert System** — flag campaigns with <30% predicted success probability and send advertiser-specific improvement suggestions
2. **AI Quality Score Coach** — step-by-step in-product assistant for improving the #1 success predictor
3. **Smart Bidding Recommendation Engine** — prompt manual bidders to switch when the model detects underperformance risk

---

## Tech Stack
`Python` `Scikit-learn` `Pandas` `NumPy` `Matplotlib` `Seaborn`

---

## Files
- `ad_campaign_performance_classifier.ipynb` — Full notebook with EDA, modeling, and product analysis

---

*Author: Mohamad Boroumand | [LinkedIn](https://linkedin.com/in/mohamad-boroumand) | UCSD MSBA 2026*
