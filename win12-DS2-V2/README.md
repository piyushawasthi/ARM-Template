# Deployment of a Windows Server 2012 DataCenter VM

# Steps To Deploy using powershell

1. Login-AzureRMAccount
2. New-AzureRmResourceGroup -Name ExampleResource -Location "West US"
3. Change adminPassword and validation_key in Template.
4. New-AzureRmResourceGroupDeployment -Name ExampleDeployment -ResourceGroupName ExampleResource -TemplateFile  C:\chef-repo\azure-templates\win12-D2-V2\azuredeploy.json -TemplateParameterFile C:\chef-repo\azure-templates\win12-D2-V2\azuredeploy.parameters.json