# IoTdeploy

This template deploys an IoT Hub with connected Device Provisioning Service and
a standard storage account.

| Parameters         |                                                                                     |
|--------------------|-------------------------------------------------------------------------------------|
| prefix (required)  | Short prefix for resource names                                                     |
| storageAccountType | Storage account type: "Standard_LRS", "Standard_GRS", "Standard_ZRS", "Premium_LRS" |

Deploy with PowerShell command: .\\Deploy-AzureResourceGroup.ps1
-ResourceGroupLocation centralus -UploadArtifacts

| Optional Flags       |                                                                                                                             |
|----------------------|-----------------------------------------------------------------------------------------------------------------------------|
| ResourceGroupName    | Default value = “IoTdeployRG”                                                                                               |
| StorageAccountName   | Storage account to upload artifacts. If not included, it will be created. If included, also specify ‘StorageContainerName’. |
| StorageContainerName | Storage account container to upload artifacts.                                                                              |
| ValidateOnly         | Run the template for validation; do not deploy.                                                                             |