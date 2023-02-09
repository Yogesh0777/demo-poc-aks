# POC: creating AKS cluster using terraform in ADO pipeline 
## Prerequisites:
* azure account
* azure-cli
  >  To install azure-cli [click here](https://learn.microsoft.com/en-us/cli/azure/install-azure-cli)
  
* login the azure account using azure-cli 
  >  [login](https://learn.microsoft.com/en-us/cli/azure/authenticate-azure-cli)
* Terraform (latest version)
  >  [install terraform](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli)

## Inputs

|Name|Description|Type|Default|Required|
|--|--|--|--|--|
|resource_group_name|Name of azure resource group|string| | true|
|location|resource group and Aks location|string| | true|
|Aks cluster name|Name of Aks cluster|string| | true|
|k8s version for Aks cluster |k8s version|string| | true|
|node group|Aks cluster node group|number| | true|

## Output

|Name|Description|Type|sensitive|
|--|--|--|--|
|aks-id|Aks clusrer id|string|false|
|aks resource group|aks cluster resource group|string|false|

# Creating resource group and AKS cluster:
Terraform script to create azure resource group and AKS cluster
* terraform init
* terraform plan 
* terraform apply

Creating Resource group and AKS cluster in the azure portal.
* use terraform destroy command to delete the resouces.

# For the ADO 

## Prerequisites:
* azure DevOps portal.
* Create pool and deploy agent in your local or azure Vm.
* service conncetion or install azure-cli inside your agent.
* github repository for pipeline
* Existing yaml for the pipeline (if available) 

# Create Aks cluster using ADO pipeline. 
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


