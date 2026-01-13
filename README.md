📊 Predictive Model for Competitive Exam Success.
Hybrid Bat Algorithm + Particle Swarm Optimization (BSO)
📌 Project Overview

Competitive exams such as CAT, GATE, and UPSC require long-term preparation, but students often lack a clear, data-driven measure of readiness.
This project builds an AI-based predictive system that estimates a student’s selection probability using mock test performance data.

To improve prediction quality, the model uses a hybrid metaheuristic optimization technique combining:

Bat Algorithm (BA) – adaptive local search

Particle Swarm Optimization (PSO) – fast global convergence

The optimized features are then fed into a Gradient Boosting classifier for final prediction.

🎯 Problem Statement

Students do not know their true readiness level

Coaching institutes rely on raw scores, not intelligent analysis

Mock test data is under-utilized

💡 Solution Approach

Extract numerical features from mock test datasets

Normalize features using standard scaling

Optimize feature weights using Hybrid BA + PSO

Train a Gradient Boosting model on optimized features

Predict selection probability for each student

Visualize results using graphs and heatmaps

🧠 Algorithms Used
1️⃣ Bat Algorithm (BA)

Mimics echolocation behavior of bats

Excellent for local exploitation

Adjusts loudness and pulse rate dynamically

2️⃣ Particle Swarm Optimization (PSO)

Inspired by bird flocking behavior

Uses velocity and global best memory

Excellent for fast convergence

3️⃣ Hybrid BA + PSO (BSO)

BA improves local refinement

PSO ensures global search stability

Hybridization avoids premature convergence

4️⃣ Gradient Boosting Classifier

Best suited for structured/tabular exam data

Handles nonlinear feature interactions efficiently

🗂️ Dataset Used

File:

RS_Session_256_AU_2981_A_to_F.csv


Features may include:

Mock scores

Accuracy

Section-wise performance

Consistency indicators

Target:

Binary or implicit readiness indicator

⚠️ The system is single-class safe, making it suitable for real mock data where confirmed selections may not yet exist.

📁 Project Structure
Predictive Model for Competitive Exam Success/
│
├── models/
│   ├── bso_gb_ba_pso_model.pkl
│   └── bso_selection_model.h5
│
├── artifacts/
│   └── bso_scaler.pkl
│
├── outputs/
│   ├── bso_final_results.csv
│   └── bso_predictions.json
│
├── graphs/
│   ├── bso_heatmap.png
│   ├── bso_accuracy_graph.png
│   ├── bso_comparison_graph.png
│   └── bso_prediction_graph.png
│
├── configs/
│   └── bso_model_config.yaml
│
├── RS_Session_256_AU_2981_A_to_F.csv
└── README.md

📊 Outputs Generated
📈 Graphs

Feature correlation heatmap

Train vs Test accuracy graph

Model comparison graph


![Confusion Matrix Heatmap](bis_heatmap.png)


Selection probability prediction graph

📄 Files

CSV: Final results with predicted probabilities

JSON: Selection probabilities

PKL: Trained Gradient Boosting model

H5: Neural network approximation

YAML: Configuration and metadata

🧪 Model Evaluation Metric

Accuracy Score

Chosen instead of ROC-AUC to support single-class datasets

🚀 How to Run the Project
1️⃣ Install Dependencies
pip install numpy pandas scikit-learn matplotlib tensorflow pyyaml joblib

2️⃣ Run the Script
python hybrid_bso_model.py


All graphs will be displayed on screen and saved automatically.

📌 Use-Cases

🎓 Students: Readiness & confidence tracking

🏫 Coaching Institutes: Batch-level performance analytics

📊 EdTech Platforms: Personalized preparation strategies

🎯 Counselors: Data-driven guidance

🧠 Key Advantages

✔ Hybrid optimization improves prediction quality
✔ Works on real-world mock test data
✔ Fully visual & interpretable outputs
✔ Portfolio / IEEE / Viva-ready
✔ Easily extensible to other hybrids

🔁 Other Hybrid Models Implemented
Model	Hybrid
PIS	AIS + PSO
PSA	CSA + PSO
BIS	AIS + BA
BSA	BA + CSA
BSO	BA + PSO
🧾 One-Line Viva Explanation

This project uses a hybrid Bat Algorithm and Particle Swarm Optimization to optimize feature weights, improving the accuracy of selection probability prediction for competitive exams.

📌 Future Enhancements

Readiness score (0–100 scale)

Multi-exam specialization (CAT/GATE/UPSC)

Streamlit dashboard for students

Automatic label generation

Cross-hybrid comparison analysis

👨‍💻 Author

Sagnik Patra
AI / ML | Optimization Algorithms | Educational Analytics
