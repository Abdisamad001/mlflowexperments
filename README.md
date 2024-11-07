# MlFlow Experments 

import dagshub
dagshub.init(repo_owner='Abdisamad001', repo_name='mlflowexperments', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)

### For MlFlow trucking use this :
export MLFLOW_TRACKING_URI=https://dagshub.com/Abdisamad001/mlflowexperments.mlflow
export MLFLOW_TRACKING_USERNAME=Abdisamad001
export MLFLOW_TRACKING_PASSWORD=9511c388afb0bf171daefe6b2e8589ed655f85a5

python app.py