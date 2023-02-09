# Prerequisites:
* azure account
* install azure-cli in local
  
* az login Run this command in your local
* install terraform latest version

# Creating resource group and AKS cluster:
* terraform init
* terraform plan 
* terraform apply

Creating Resource group and AKS cluster in the azure portal.
* use terraform destroy command to delete the resouces.

# For the ADO 

# Prerequisites:
* azure DevOps portal.
* Create pool and deploy agent in your local or azure Vm.
* service conncetion or install azure-cli inside your agent.
* terraform code 
* and use the starter pipeline.

# Create Aks cluster using ADO pipeline.

create resource group and the AKS cluster to use the script in the azure devops pipeline.

steps:-
 * go to the azure devops pipeline
 * add the git hub repo
 * use starter pipeline
 * add the pipeline script and yaml 
 * and add the agent pool in the pipeline yaml.
   ex. pool: Default 
 * save and run.
 * see the logs inside the agent, pipeline successful or not

AKS cluster is cretaed inside the azure portal.