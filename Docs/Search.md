<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"  "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<title>Search</title>
</head><body>
<table>
<colgroup><col/><col/><col/></colgroup>
<tr><th>Description</th><th>ControlSeverity</th><th>Automated</th></tr>
<tr><td>All users/identities must be granted minimum required permissions using Role Based Access Control (RBAC)</td><td>Medium</td><td>Yes</td></tr>
<tr><td>Users monitoring/supporting the Search service should be provided with minimum required permissions</td><td>Medium</td><td>No</td></tr>
<tr><td>Sensitive data at data source must be encrypted at rest</td><td>High</td><td>No</td></tr>
<tr><td>Sensitive data must be encrypted in transit</td><td>High</td><td>No</td></tr>
<tr><td>Admin keys must be furnished only for clients who need to manage the search catalog of Search service</td><td>High</td><td>No</td></tr>
<tr><td>Consumers who require read access on Search service must only be granted &#39;query&#39; keys</td><td>High</td><td>No</td></tr>
<tr><td>Search service must have at least three replicas for high availability</td><td>Medium</td><td>Yes</td></tr>
<tr><td>Diagnostics logs must be enabled with a retention period of at least $($this.ControlSettings.Diagnostics_RetentionPeriod_Min) days</td><td>Medium</td><td>Yes</td></tr>
</table>
</body></html>
