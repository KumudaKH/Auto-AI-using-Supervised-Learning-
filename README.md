**Steps to Run in IBM Cloud**
**1. Setup Environment**
   1.Go to IBM Cloud.
   2.Add the following services:
        Watsonx.ai Studio
        Runtime environment
   3.Create a new project with the name Crop-ML (or your desired project name).

**2. Manage & Associate Services**
    1.Open the project and go to Manage.
    2.Associate the required service (AutoAI needs runtime to execute data).

  **3. Data Preparation**
    1.Go to Overview.
    2.Upload your dataset (.csv file). Example: Crop Recommendation Dataset.
    3.AutoAI will analyze data and create a Machine Learning pipeline automatically.

  **4. Define Project Details**
    1.Project Name: Crop-ML
    2.AutoAI will handle data preprocessing, feature engineering, and model selection automatically.

  **5. API Key**
    1.Create an API Key in IBM Cloud.
    2.This API key is required to access ML resources (datasets, algorithms, data analysis, etc.).
    3.A new window will open → copy and save the API key safely.

 **6. Running AutoAI Experiment**
    1.Select the target column (label) you want to predict.
    2.Click Run Experiment.
    3.AutoAI will:
    4.Use resources
    5.Train models
    6.Test performance
    7.Finally, it will show the best model with accuracy score

  **7. Model Selection**
      1.From the ranked models, select the first one (highest accuracy).
      2.Click Save As → Model.
      3.Select Model → Create (not Notebook, since no code is needed).
      4.View the model in the project.

      **8. Promote Model to Deployment Space**
        1.On the right, click Promote to space.
        2.If no space exists, create a new space:
        3.Name it Crop-Deploy.
        4.Click Create.
        5.The model is now promoted to the deployment space.

        
