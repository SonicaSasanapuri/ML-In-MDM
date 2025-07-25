# ML-In-MDM
# Master Data Management (MDM): Deduplication & Classification using Machine Learning

This project solves two key challenges in Master Data Management (MDM) using machine learning:

1. Deduplication – Identifying and merging duplicate records based on similarity across fields.
2. Classification – Predicting the Contact Function (e.g., CEO, CIO, Board Member) based on contact attributes like Name, Title, Organization, Country, etc.

----------------------------------------
📁 Project Structure

- deduplication.ipynb
- classification.ipynb
- datasets/
    - raw_data.csv
    - clean_data.csv
    - dirty_data_with_duplicates.csv
- output/
    - deduplicated_clean_data.csv
    - final_combined_contact_function.csv
- requirements.txt
- README.md

----------------------------------------
🧠 Techniques Used

Deduplication:
- Fuzzy string matching using fuzzywuzzy
- Weighted field-wise similarity scoring (Name, Email, Org, Country, etc.)
- Manual threshold tuning to detect duplicates
- Anomaly Detection using Isolation Forest
- Clustering using KMeans and DBSCAN

Classification:
- Preprocessing with pandas (cleaning NaNs and unknown values)
- Feature encoding using LabelEncoder
- Feature scaling using StandardScaler
- Classification using Random Forest
- SMOTE used to handle class imbalance
- Evaluation using Accuracy, Precision, Recall, and F1-Score

----------------------------------------
📊 Model Performance (Random Forest)

- **Training Accuracy**: 64.25%
- **Test Accuracy**: 62.03%

The model generalizes well without significant overfitting.

----------------------------------------
🛠️ Libraries Used

- pandas, numpy
- scikit-learn (including RandomForestClassifier)
- fuzzywuzzy
- matplotlib)

----------------------------------------
📌 How to Run

1. Clone the repository:
   git clone https://github.com/your-username/mdm-deduplication-classification.git
   cd mdm-deduplication-classification

2. Install the required libraries:
   pip install -r requirements.txt

3. Run the notebooks:
   jupyter notebook deduplication.ipynb
   jupyter notebook classification.ipynb

----------------------------------------
✅ Output Files

- deduplicated_clean_data.csv – Final cleaned dataset with duplicates removed
- final_combined_contact_function.csv – Final output with predicted Contact Functions

----------------------------------------
🙋 About Me

Sonica Sasanapuri  
T
hird-Year Mechanical Engineering Student, IIT Kanpur  
Intern at Franklin Templeton (2025)  
LinkedIn: https:www.linkedin.com/in/sonica-sasanapuri-sasana19
----------------------------------------
📬 Contact

Email: sonicasasanapuri19@gmail.com  
GitHub: https://github.com/SonicaSasanapuri


----------------------------------------
