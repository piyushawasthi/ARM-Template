# ARM Template to deploy multiple VM of windows server 2012

# Steps To Deploy using powershell

1. Login-AzureRMAccount
2. New-AzureRmResourceGroup -Name ExampleResourceGroup -Location "West US"
3. Change adminPassword and validation_key in Template.
4. New-AzureRmResourceGroupDeployment -Name ExampleDeployment -ResourceGroupName ExampleResourceGroup -TemplateFile C:\chef-repo\multiVM-Windows\deploy.json -TemplateParameterFile C:\chef-repo\multiVM-Windows\deploy.params.json
