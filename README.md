# CustomerLTVKedro
Phase 1: Project Setup & Environment
Objective: Establish a solid, reproducible foundation.
Key Tasks:
Initialize Repository & Virtual Environment (2 SP):
Set up Git locally and on GitHub for version control.
Create a Python virtual environment and document your dependencies.
Scaffold Kedro Project (3 SP):
Use kedro new to generate a project structure.
Organize folders for data, notebooks, source code, and configuration.
Phase 2: Data Ingestion & Storage
Objective: Ingest the static dataset and set up local data storage.
Key Tasks:
Data Ingestion (3 SP):
Configure the Kedro Data Catalog to load your customer data from CSV/Excel.
Implement error handling and logging in the ingestion node.
Local Database Setup (Optional for Extended Demo) (2 SP):
Use SQLite (or PostgreSQL if you’re comfortable) for storing processed data and prediction logs.
Integrate basic CRUD operations using SQLAlchemy (or omit if focusing on modeling).
Phase 3: Data Cleaning & EDA
Objective: Prepare and understand the dataset for effective modeling.
Key Tasks:
Data Cleaning Pipeline (4 SP):
Develop Kedro nodes to handle missing values, format corrections, and outlier removal.
Document cleaning assumptions.
Exploratory Data Analysis (4 SP):
Use a Jupyter Notebook to visualize key metrics (distributions, correlations, trends).
Summarize findings in a brief report to extract potential features.
Phase 4: Feature Engineering & Transformation
Objective: Create meaningful features that drive model performance.
Key Tasks:
Feature Engineering (4 SP):
Develop nodes to generate new features (e.g., activity ratios, tenure categories).
Iterate based on initial model insights.
Data Transformation & Catalog Update (2 SP):
Store the transformed dataset in your Kedro Data Catalog for training.
Phase 5: Modeling & Evaluation
Objective: Build, evaluate, and select the best model for customer attrition prediction.
Key Tasks:
Baseline Model Implementation (4 SP):
Train a simple logistic regression model as a starting point.
Advanced Model Experiments (6 SP):
Experiment with models like RandomForest, XGBoost, or LightGBM.
Use cross-validation and hyperparameter tuning.
Performance Evaluation (3 SP):
Generate metrics (accuracy, precision, recall, ROC-AUC) and compare model performance.
Select and document the final model.
Phase 6: Model Serialization & API Development
Objective: Package the final model and expose it via an API.
Key Tasks:
Serialize the Model (2 SP):
Save the trained model using joblib.
FastAPI Setup (3 SP):
Create a basic FastAPI application with a health-check endpoint.
Develop Prediction Endpoint (4 SP):
Build an endpoint that accepts customer data (with Pydantic validation) and returns predictions.
Integrate error handling and logging.
Phase 7: Business Reporting & Insights
Objective: Translate technical outcomes into actionable business insights.
Key Tasks:
Draft a Business Insights Notebook (4 SP):
Combine EDA, feature importance, and model performance into a single narrative.
Visualize key metrics and potential business impact (e.g., churn reduction strategies).
Create a Final Report/Slide Deck (4 SP):
Develop a polished report that summarizes project objectives, methodology, outcomes, and actionable recommendations.
Use clear visuals and business language to target non-technical stakeholders.
Phase 8: Containerization & Local Testing (Optional but Beneficial)
Objective: Simulate a production-ready environment.
Key Tasks:
Dockerize the Application (4 SP):
Write a Dockerfile to containerize your FastAPI app.
Local Integration Testing (2 SP):
Test the complete setup locally using Docker (and Docker Compose if including the database).
Phase 9: Testing & Documentation
Objective: Ensure robustness and clarity across your project.
Key Tasks:
Write Unit Tests (3 SP):
Use Pytest to cover key functions in your Kedro nodes and FastAPI endpoints.
Document the Project (3 SP):
Update README with setup instructions, project structure, and usage guidelines.
Include API documentation (Swagger UI is auto-generated with FastAPI).
