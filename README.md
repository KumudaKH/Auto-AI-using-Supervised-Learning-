**Steps to Run in IBM Cloud**
### 1. Setup Environment
  - Go to IBM Cloud.
  - Add the following services:
       - Watsonx.ai Studio
       - Runtime environment
  - Create a new project with the name Crop-ML (or your desired project name).

### 2. Manage & Associate Services
   - Open the project and go to Manage.
   - Associate the required service (AutoAI needs runtime to execute data).

  ### 3. Data Preparation
   - Go to Overview.
   - Upload your dataset (.csv file). Example: Crop Recommendation Dataset.
   - AutoAI will analyze data and create a Machine Learning pipeline automatically.

  ### 4. Define Project Details
   - Project Name: Crop-ML
   - AutoAI will handle data preprocessing, feature engineering, and model selection automatically.

  ### 5. API Key
   - Create an API Key in IBM Cloud.
   - This API key is required to access ML resources (datasets, algorithms, data analysis, etc.).
   - A new window will open → copy and save the API key safely.

 ### 6. Running AutoAI Experiment
   - Select the target column (label) you want to predict.
   - Click Run Experiment.
   - AutoAI will:
   - Use resources
   - Train models
   - Test performance
   - Finally, it will show the best model with accuracy score

 ### 7. Model Selection
   - From the ranked models, select the first one (highest accuracy).
   - Click Save As → Model.
   - Select Model → Create (not Notebook, since no code is needed).
   - View the model in the project.

 ### 8. Promote Model to Deployment Space
  - On the right, click Promote to space.
  - If no space exists, create a new space:
  - Name it Crop-Deploy.
  - Click Create.
  - The model is now promoted to the deployment space.

 ###  9. Deployment
 - Go to Space settings.
 - Add Watsonx.ai Runtime Service → Associate instance.  
 - (This is required to run the project on IBM Cloud).
 - Save changes.
 - In the Deployment space:
   	 - Click the Model name.
   	 -Create a New Deployment → Select Online Deployment.
       - Provide a deployment name (e.g., Crop-Deploy-1).
       - Click Create.
 - The model is now fully deployed and integrated with IBM services.

   ### 10. Public Endpoint
    - Open the deployed model.
    - Copy the Public Endpoint URL.
    - This endpoint can be used in applications (frontend, backend, or API calls).
    - It is accessible to all stakeholders.

        
