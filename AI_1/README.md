Task 1: Exploring and Visualizing a Simple Dataset
Objective
To perform initial data exploration and visualization on a simple, well-known dataset to understand its structure and relationships between variables.

Dataset Used
Iris Dataset: A classic dataset in machine learning, commonly used for classification and clustering examples. It contains measurements of sepal length, sepal width, petal length, and petal width for three species of Iris flowers.
Models Applied
No specific machine learning models were applied in this task. The focus was on exploratory data analysis (EDA) techniques.

Key Results and Findings
The dataset consists of 150 entries with 5 columns (4 numerical features and 1 categorical target species). There were no missing values.
Summary statistics provided insights into the distribution of numerical features.
Scatter Plot (Sepal Length vs. Sepal Width by Species): Clearly showed distinct clusters for setosa species, while versicolor and virginica had some overlap but were generally separable.
Box Plot (Petal Length Distribution per Species): Illustrated the differing distributions of petal length across the three species, highlighting setosa having significantly shorter petals than the other two.
Task 3: Heart Disease Prediction
Objective
To build and evaluate a machine learning model for predicting heart disease based on various health indicators.

Dataset Used
Heart Disease Dataset: Loaded from KaggleHub (arezaei81/heartcsv). This dataset likely contains features related to patient health (e.g., age, sex, chest pain type, blood pressure, cholesterol) and a binary target variable indicating the presence or absence of heart disease.
Models Applied
Logistic Regression: A linear model used for binary classification. It was chosen for its interpretability and effectiveness in many classification tasks.
Key Results and Findings
The model achieved an overall accuracy of approximately 89% on the test set.
Precision, Recall, and F1-score for both classes (0 and 1) were consistently high, ranging from 0.86 to 0.91, indicating good predictive performance.
The confusion matrix visually confirmed the model's ability to correctly classify a high percentage of both positive and negative cases, with relatively few false positives and false negatives.
Task 4: General Health Query Chatbot (Prompt Engineering)
Objective
To develop a conversational AI chatbot that provides general health information while incorporating safety mechanisms through prompt engineering and rule-based checks to prevent harmful or inappropriate responses.

Dataset Used
Not directly applicable. This task uses a pre-trained large language model.

Models Applied
google/flan-t5-large: A large language model from Google, specifically fine-tuned for a variety of tasks, including question answering and text generation. It was loaded using Hugging Face Transformers.
Key Results and Findings
The chatbot successfully loads and utilizes the google/flan-t5-large model for generating responses.
Safety Layer 1 (Emergency Detection): Implemented to identify keywords related to medical emergencies (chest pain, heart attack, suicide, etc.) and advises the user to seek immediate medical attention.
Safety Layer 2 (Dosage Blocking): Designed to prevent the chatbot from providing specific dosage instructions by detecting keywords (dosage, how many mg, etc.) and advising consultation with a doctor or pharmacist.
System Prompt Engineering: A detailed system prompt (SYSTEM_PROMPT) guides the LLM to act as a helpful and friendly medical assistant, follow ethical rules (no diagnosis, no prescriptions, general info only), and maintain a calm and supportive tone.
The chatbot demonstrates its ability to engage in general health conversations while adhering to the defined safety and ethical guidelines.
