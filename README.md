🧠 Agile Resource Scheduler – Intelligent Task Allocation for Agile Teams

This project leverages machine learning to automate and optimise resource planning and task scheduling for Agile software development environments. By analyzing historical task data, team velocity, and individual availability, the model intelligently recommends task assignments and sprint schedules that maximize efficiency and productivity.

Built as part of a group capstone for our Minor Specialization, this project simulates real-world Agile resource management scenarios found in Scrum or Kanban setups.

⸻

🎯 Key Features:
	•	Synthetic Data Generation
Generates realistic employee and task datasets with features like skills, workload, availability, experience, and task priority.
	•	Feature Engineering
Constructs high-value features such as:
	•	skill_match, workload_ratio, priority_score, skill_gap, capacity_left
	•	Target Labeling
Uses rule-based logic combined with Gaussian noise to create a binary label (good_allocation) that simulates assignment suitability.
	•	Machine Learning Model – Random Forest Classifier
	•	Tuned for performance using cross-validation
	•	Balanced class distribution using SMOTE oversampling
	•	Predicts probability scores for each task-resource pair
	•	Ranks candidates and selects top resource for each task
	•	Final Output
Generates optimal_allocations.csv with top recommendations, including confidence scores and all relevant details.

⸻

📈 Visualization Dashboard (Tableau Prototype)

Though our primary focus was on the machine learning pipeline, we also built a lightweight Tableau dashboard to visualize:
	•	Sprint-wise task allocation
	•	Workload distribution by resource
	•	Priority vs skill alignment
This helped us verify allocation logic and communicate insights to stakeholders.

⸻

⚙️ Tech Stack:
	•	Python – Pandas, NumPy, scikit-learn, imbalanced-learn
	•	Modeling – Random Forest Classifier
	•	Imbalance Handling – SMOTE
	•	Development Environment – Google Colab / Jupyter Notebooks
	•	Visualization (Optional) – Tableau Public
