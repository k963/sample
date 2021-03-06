<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"  "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<title>DataLakeStore</title>
</head><body>
<table>
<colgroup><col/><col/><col/></colgroup>
<tr><th>Description</th><th>ControlSeverity</th><th>Automated</th></tr>
<tr><td>All users/applications are authenticated using Azure Active Directory (AAD) based credentials</td><td>High</td><td>No</td></tr>
<tr><td>All users/identities must be granted minimum required permissions using Role Based Access Control (RBAC)</td><td>Medium</td><td>Yes</td></tr>
<tr><td>Access to Data Lake Store file system must be limited by using appropriate Access Control List (ACL). The &#39;Other&#39; group must not have any access</td><td>High</td><td>Yes</td></tr>
<tr><td>Firewall should be enabled on Data Lake Store</td><td>Medium</td><td>Yes</td></tr>
<tr><td>AdlCopy tool must be used securly while copying data from storage blobs to Data Lake Store</td><td>High</td><td>No</td></tr>
<tr><td>Data Factory must be used securely while moving data to or from the Data Lake Store</td><td>High</td><td>No</td></tr>
<tr><td>Clients such as web jobs, standalone apps should use a service principal identity to access Data Lake Store</td><td>High</td><td>No</td></tr>
<tr><td>Sensitive data must be encrypted at rest</td><td>High</td><td>Yes</td></tr>
<tr><td>Sensitive data must be encrypted in transit</td><td>High</td><td>No</td></tr>
<tr><td>Diagnostics logs must be enabled with a retention period of at least $($this.ControlSettings.Diagnostics_RetentionPeriod_Min) days.</td><td>Medium</td><td>Yes</td></tr>
<tr><td>Diagnostic logs for Data Lake Store should be reviewed periodically</td><td>Medium</td><td>No</td></tr>
<tr><td>Backup and Disaster Recovery must be planned for Data Lake Store</td><td>Medium</td><td>No</td></tr>
<tr><td>Data in Data Lake Store should be cleaned up using file retention</td><td>Medium</td><td>No</td></tr>
</table>
</body></html>
