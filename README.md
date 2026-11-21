 CYBERSHIELD AI 🛡️
 Hinglish Cyberbullying Detection Using NLP and Machine Learning

A Machine Learning Mini Project – Experiment 10  
School of Computer Science, UPES

📌 Overview
CyberShield AI is a machine learning-based cyberbullying detection system designed to identify potentially harmful content in Hinglish text. It analyses text using Natural Language Processing (NLP) and classifies it into different cyberbullying categories.

The project uses TF-IDF feature extraction and compares five machine learning algorithms to identify the best-performing model.


    
 Architecture

mermaid
flowchart TD
    A["MC-Hinglish 1.0 Dataset"] --> B["Data Loading & Exploration"]
    B --> C["Text Preprocessing & Cleaning"]
    C --> D["TF-IDF Feature Extraction"]
    D --> E["Train-Test Split"]

    E --> F["Linear SVM"]
    E --> G["SGD Classifier"]
    E --> H["Logistic Regression"]
    E --> I["Complement Naive Bayes"]
    E --> J["Multinomial Naive Bayes"]

    F --> K["Model Evaluation"]
    G --> K
    H --> K
    I --> K
    J --> K

    K --> L["Compare Performance Metrics"]
    L --> M["Best Model: Linear SVM"]

    N["New Hinglish Text Input"] --> O["Text Cleaning"]
    O --> P["TF-IDF Transformation"]
    P --> M
    M --> Q["Cyberbullying Category Prediction"]
    Q --> R["Predicted Category"]

    classDef dataset fill:#DBEAFE,stroke:#2563EB,color:#1E3A8A,stroke-width:2px
    classDef preprocess fill:#FEF3C7,stroke:#D97706,color:#78350F,stroke-width:2px
    classDef features fill:#F3E8FF,stroke:#9333EA,color:#581C87,stroke-width:2px
    classDef models fill:#CFFAFE,stroke:#0891B2,color:#164E63,stroke-width:2px
    classDef evaluation fill:#FFEDD5,stroke:#EA580C,color:#7C2D12,stroke-width:2px
    classDef best fill:#DCFCE7,stroke:#16A34A,color:#14532D,stroke-width:3px
    classDef output fill:#FCE7F3,stroke:#DB2777,color:#831843,stroke-width:2px

    class A,B dataset
    class C,O preprocess
    class D,P features
    class E,F,G,H,I,J models
    class K,L evaluation
    class M best
    class N,Q,R output


 ✨ Features
- Hinglish cyberbullying detection
- Text cleaning and preprocessing
- TF-IDF feature extraction
- Classification into seven categories
- Comparison of five machine learning models
- Prediction on new user-input text
- Performance evaluation using accuracy, precision, recall and F1-score

🧠 Problem Statement
Cyberbullying through online communication is a growing concern, especially when harmful messages are written in mixed languages such as Hindi and English (Hinglish). Traditional detection systems may struggle to understand such mixed-language content.

CyberShield AI aims to identify potentially abusive and harmful Hinglish text using NLP techniques and machine learning classification models.

 📊 Performance

The five machine learning models were evaluated and compared using the validation dataset.

| Model | Accuracy | Precision | Recall | F1 Score |
|---|---:|---:|---:|---:|
| Linear SVM | *80.87%* | 0.8076 | 0.8031 | *0.8047* |
| SGD Classifier | 80.12% | 0.8003 | 0.7960 | 0.7975 |
| Logistic Regression | 78.97% | 0.7944 | 0.7859 | 0.7887 |
| Complement Naive Bayes | 73.77% | 0.7597 | 0.7259 | 0.7265 |
| Multinomial Naive Bayes | 69.78% | 0.7441 | 0.6802 | 0.6822 |

*Best Performing Model:* Linear SVM

 ⚙️ System Architecture
The project follows this workflow:

1. *Dataset Collection* — Uses MC-Hinglish 1.0 training and testing datasets.
2. *Data Preprocessing* — Cleans and prepares the text data.
3. *Feature Extraction* — Converts text into numerical features using TF-IDF.
4. *Model Training* — Trains five machine learning classification algorithms.
5. *Model Evaluation* — Compares model performance using evaluation metrics.
6. *Prediction* — Uses the trained model to classify new Hinglish text.

## 🛠️ Tech Stack
- *Programming Language:* Python
- *Development Environment:* Google Colab
- *Data Processing:* Pandas, NumPy
- *Visualization:* Matplotlib, Seaborn
- *Machine Learning:* Scikit-learn
- *NLP Technique:* Text Preprocessing and TF-IDF Vectorization
- *Algorithms:* Linear SVM, SGD Classifier, Logistic Regression, Complement Naive Bayes, Multinomial Naive Bayes

🧪 Evaluation Metrics
- *Accuracy* — Measures the overall correctness of predictions.
- *Precision* — Measures how many predicted classifications were correct.
- *Recall* — Measures how many actual classifications were identified correctly.
- *F1 Score* — Combines precision and recall into one score.
- *Confusion Matrix* — Helps analyse correct and incorrect classifications.

📈 Future Scope
- Develop a web-based cyberbullying detection application.
- Add real-time detection for social media messages.
- Improve detection accuracy for different Hinglish writing styles.
- Extend support to additional Indian languages.
- Integrate the model with online platforms for harmful-content monitoring.

Contact
*Name:* Suhani Ahuja  *Education:* MCA(AI & ML), UPES, Dehradun   *Email:* suhaniahuja2105@gmail.com / suhani.33021@stu.upes.ac.in  *GitHub:* suhaniahujaa

*Name:* Aryan Sethi  *Education:* MCA(AI & ML), UPES, Dehradun   *Email:* aryansethi2206@gmail.com / aryan.31882@stu.upes.ac.in  *GitHub:* aryan2206

 Mentor
*Dr. Sahinur Rahman Laskar* Assistant Professor (Senior Scale) School of Computer Science, UPES, Dehradun, India Email: sahinurlaskar.nits@gmail.com / sahinur.laskar@ddn.upes.ac.in

Citation
If you use this project, please cite it as:

bibtex
@misc{cybershieldai2026,
  title={CyberShield AI: Hinglish Cyberbullying Detection Using NLP and Machine Learning},
  author={Aryan Sethi},
  year={2026},
  note={Machine Learning Mini Project, Experiment 10}
}
