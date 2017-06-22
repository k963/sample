## Security controls covered by the Secure DevOps Kit for Azure 

This page displays security controls that are automated via the devops kit and also controls that have to manually verified. Mandatory controls are listed with controlType as 'Severity' and advisory ones as 'Best Practice'. Apart from that the automated flag indicates whether a particular control is automated and the enabled flag tells whether the check for that control is currently enabled or not. 
Apart from security checks for Subscription Security and for multiple Azure Services, other features such as Security IntelliSense and Alerting & Monitoring are also covered.

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

|ID|Description	|ControlSeverity|Automated|
|----|------|--------|------|
|Azure_AnalysisServices_AuthZ_Grant_Min_RBAC_Access|All users/identities must be granted minimum required permissions using Role Based Access Control (RBAC)	|Medium|Yes|
|Azure_AnalysisServices_AuthZ_Min_Admin|Minimize the number of Analysis Service admins	|Medium|Yes|
|Azure_AnalysisServices_AuthZ_Users_Min_DB_Permission|Database users must be added to database roles with minimum required permission	|Medium|No|
|Azure_AnalysisServices_AuthN_Analysis_Service_Clients|Analysis Service clients should authenticate users using Azure Active Directory backed credentials|High|No|
|Azure_AnalysisServices_DP_Encrypt_In_Transit|Sensitive data must be encrypted in transit|High|No|
|Azure_AnalysisServices_DP_Encrypt_At_Rest|Sensitive data must be encrypted at rest	|High|No|
|Azure_AnalysisServices_BCDR_Plan|Backup and Disaster Recovery must be planned for Analysis Services|Medium|Yes|
