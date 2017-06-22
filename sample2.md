## Security controls covered by the Secure DevOps Kit for Azure 

This page displays security controls that are automated via the devops kit and also controls that have to manually verified. Controls have a 'Severity' field to help teams distinguish issues by degree of risk. Apart from that the automated flag indicates whether a particular control is automated and the enabled flag tells whether the check for that control is currently enabled or not. Apart from security checks for Subscription Security and for multiple Azure Services, other features such as Security IntelliSense and Alerting & Monitoring are also covered. 

| Resource Name |Resource Type|
|-------|---------- |
|<a href=#go>Analysis Services<a> |Microsoft.AnalysisServices/servers|
|App Services|Microsoft.Web/sites|
|Batch accounts |Microsoft.Batch/batchAccounts|
|CDN profiles |Microsoft.Cdn/profiles|
|Cloud Services|Microsoft.ClassicCompute/domainNames|
|Data Factories |Microsoft.DataFactory/dataFactories|
|Data Lake Analytics|Microsoft.DataLakeAnalytics/accounts|
|Data Lake Store|Microsoft.DataLakeStore/accounts|
|Express Route-connected Virtual ERvNet |Microsoft.Network/virtualNetworks|
|Event Hubs|Microsoft.Eventhub/namespaces|
|Key Vaults|Microsoft.KeyVault/vaults|
|Logic Apps|Microsoft.Logic/Workflows|
|Notification Hubs|Microsoft.NotificationHubs/namespaces/notificationHubs|
|On-premises Data Gateways |Microsoft.Web/connectionGateways|
|Redis Caches |Microsoft.Cache/Redis|
|Search services|Microsoft.Search/searchServices|
|Service Bus |Microsoft.ServiceBus/namespaces|
|Service Fabric clusters |Microsoft.ServiceFabric/clusters|
|SQL Databases|Microsoft.Sql/servers|
|Storage Accounts|Microsoft.Storage/storageAccounts|
|Traffic Manager profiles |Microsoft.Network/trafficmanagerprofiles|
|Virtual Machines|Microsoft.Compute/virtualMachines|
| Virtual Networks|Microsoft.Network/virtualNetworks|

<h3 id=go> Controls for Analysis Service</h3>

|Description	|Severity|Automated|Enabled|Recommendation|
|------|--------|------|-----|----|
|All users/identities must be granted minimum required permissions using Role Based Access Control (RBAC)	|Medium|Yes|True|Remove any excessive privileges granted on the Analysis Service. Run command Remove-AzureRmRoleAssignment -SignInName '{signInName}' -Scope '{scope}' -RoleDefinitionName '{role definition name}'. Run 'Get-Help Remove-AzureRmRoleAssignment -full' for more help. Refer: https://docs.microsoft.com/en-us/sql/analysis-services/multidimensional-models/roles-and-permissions-analysis-services, https://docs.microsoft.com/en-us/azure/analysis-services/analysis-services-manage-users, https://docs.microsoft.com/en-us/azure/active-directory/role-based-access-control-manage-access-powershell|
|Minimize the number of Analysis Service admins	|Medium|Yes|True|Minimize the number of Analysis Service admins. Run command Set-AzureRmAnalysisServicesServer -Name '{AnalysisServicesServerName}' -ResourceGroupName '{ResourceGroupName}' -Administrator '{Administrator}'. Refer: https://docs.microsoft.com/en-us/powershell/module/azurerm.analysisservices/set-azurermanalysisservicesserver?view=azurermps-3.8.0|
|Database users must be added to database roles with minimum required permission	|Medium|No|True|Make sure that users are granted the least required privileges to databases and tabular models. Refer: https://docs.microsoft.com/en-us/azure/analysis-services/analysis-services-manage-users, https://docs.microsoft.com/en-us/sql/analysis-services/tabular-models/create-and-manage-roles-ssas-tabular|
|Analysis Service clients should authenticate users using Azure Active Directory backed credentials|High|No|True|Analysis Services clients such as 'Power BI', 'Excel' or any BI Tools should authenticate users using Azure Active Directory backed credentials. Refer: (Power BI) https://docs.microsoft.com/en-us/azure/power-bi-embedded/power-bi-embedded-app-token-flow and (Excel) https://docs.microsoft.com/en-us/azure/analysis-services/analysis-services-connect-excel|
|Sensitive data must be encrypted in transit|High|No|True|Ensure that sensitive data is transmitted only on an encrypted channel through out the Analysis Service. Refer: https://blogs.msdn.microsoft.com/jason_howell/2013/02/26/how-do-i-ensure-analysis-services-client-tcp-connectivity-is-encrypted/|
|Sensitive data must be encrypted at rest	|High|No|True|Azure Analysis Service utilizes Blob Storage to persist storage and metadata for Analysis Services databases. Azure Blob Server Side Encryption (SSE) must be turned on for the Blob container. Run command 'Set-AzureRmStorageAccount -Name '<StorageAccountName>' -ResourceGroupName '<RGName>' -EnableEncryptionService 'Blob''. Run 'Get-Help Set-AzureRmStorageAccount -full' for more help.|
|Backup and Disaster Recovery must be planned for Analysis Services|Medium|Yes|True|Go To Azure Portal => Analysis Services => Select Analysis Service => Go To Settings => Select Backups => Select Storage account details and enable backups, Refer: https://docs.microsoft.com/en-us/azure/analysis-services/analysis-services-backup|
