This project leverages machine learning to automate and optimize resource planning and task scheduling for Agile software development teams. By analyzing historical task data, team velocity, and member availability, the model intelligently recommends task assignments and sprint schedules that improve overall efficiency.

This project implements a machine learning pipeline to predict optimal task-to-resource allocations for Agile software development teams. Using a Random Forest Classifier, the model evaluates task requirements and resource capabilities to assign the most suitable employee to each task, maximizing productivity while respecting constraints like skill match, availability, priority, and complexity.

📂 Built as part of a group project for our Minor specialization, this solution simulates real-world resource management scenarios in Agile environments like Scrum or Kanban.



🎯 Key Features:
	•	Synthetic Data Generation: Simulates realistic employee (resource) and task datasets with features like skills, workload, availability, experience, and priority.
	•	Feature Engineering: Constructs derived features like skill match, capacity availability, skill gap, workload ratio, and priority score.
	•	Target Labeling: Creates a good_allocation binary label using rule-based logic and Gaussian noise to reflect real-world assignment suitability.
	•	Modeling with Random Forest:
	•	Includes oversampling with SMOTE to balance classes.
	•	Uses cross-validation to evaluate F1-score performance.
	•	Allocation Ranking: Predicts allocation probabilities and selects the top resource for each task based on model confidence.
	•	Output File: Saves final assignments to optimal_allocations.csv with details like task info, resource details, and allocation score.

⸻

⚙️ Tech Stack:
	•	Python (Pandas, NumPy, scikit-learn, imbalanced-learn)
	•	Random Forest Classifier (with hyperparameters tuned)
	•	SMOTE Oversampling (to handle class imbalance)
	•	Colab / Jupyter Notebook – Used for prototyping and visualization

⸻

📁 Outputs:
	•	resources.csv – Simulated employee dataset
	•	tasks.csv – Simulated tasks with constraints
	•	optimal_allocations.csv – Final task-to-resource assignments
	•	Console logs – Model metrics, cross-validation results, and sample predictions

⸻

📊 Sample Output Columns:
	•	task_id, project_name, priority, required_skill
	•	employee_name, employee_primary_skill, allocation_score
	•	employee_availability, skill_level, task_complexity

