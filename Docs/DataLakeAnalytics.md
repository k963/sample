<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"  "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<title>DataLakeAnalytics</title>
</head><body>
<table>
<colgroup><col/><col/><col/></colgroup>
<tr><th>Description</th><th>ControlSeverity</th><th>Automated</th></tr>
<tr><td>Data Lake Analytics creator must be granted only required Role Based Access Control (RBAC) access on Subscription/Resource Group/Resource</td><td>Medium</td><td>No</td></tr>
<tr><td>All Data Lake Analytics users/service principal must be authenticated using AAD backed credentials</td><td>High</td><td>No</td></tr>
<tr><td>All users/identities must be granted minimum required permissions using Role Based Access Control (RBAC)</td><td>Medium</td><td>Yes</td></tr>
<tr><td>Data Lake Analytics developer (user/service principal) must have least required ACLs on Catalog/Database and Data Lake Store file system</td><td>Medium</td><td>No</td></tr>
<tr><td>Storage account data source must be added securely</td><td>Medium</td><td>No</td></tr>
<tr><td>Secrets to access SQL Azure/SQL VM/SQL Data Warehouse must be securely stored under Catalog database credentials</td><td>High</td><td>No</td></tr>
<tr><td>U-SQL script file(s) must be uploaded from a secured/trusted location</td><td>High</td><td>No</td></tr>
<tr><td>Diagnostics logs must be enabled with a retention period of at least $($this.ControlSettings.Diagnostics_RetentionPeriod_Min) days.</td><td>Medium</td><td>Yes</td></tr>
<tr><td>Sensitive data must be encrypted at rest</td><td>High</td><td>Yes</td></tr>
<tr><td>Sensitive data must be encrypted in transit</td><td>High</td><td>No</td></tr>
<tr><td>Backup and Disaster Recovery must be planned for the default Data Lake Store account</td><td>Medium</td><td>No</td></tr>
<tr><td>Diagnostic and activity logs for Data Lake Analytics should be reviewed periodically</td><td>Medium</td><td>No</td></tr>
</table>
</body></html>
