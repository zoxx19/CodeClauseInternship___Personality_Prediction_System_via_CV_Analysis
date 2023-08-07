# Personality Prediction from CV Analysis
This project aims to predict personality traits from resumes/CVs using natural language processing and machine learning techniques. It categorizes personality based on the Big Five model - openness, conscientiousness, extraversion, agreeableness, and neuroticism.

The system uses a parsed resume as input. It extracts text from PDF, DOCx, and TXT resume files using pyresparser. For feature extraction, it searches for predefined keywords related to each of the Big Five traits using spaCy's PhraseMatcher. Based on the keyword occurrences, it assigns a score for each trait on a scale of 0-10.

Various supervised machine learning models are trained on the dataset including LogisticRegression, Naive Bayes, KNN, SVC, XGBClassifier, and Random Forest. To improve performance, ensemble techniques like bagging and stacking are used. The features are the five trait scores and the target is one of five personality types.

The personality prediction can help streamline recruiting by filtering candidates beyond just skills and experience. The system automates manual screening, saving time and providing insights into applicants' personalities.

## Future Work
 * Increase dataset size for better model training
 * Try deep learning approaches like CNNs or RNNs
 * Optimize ensemble and stacking techniques
 * Expand beyond text to analyze other application material
