<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"  "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<title>Batch</title>
</head><body>
<table>
<colgroup><col/><col/><col/></colgroup>
<tr><th>Description</th><th>ControlSeverity</th><th>Automated</th></tr>
<tr><td>All users/identities must be granted minimum required permissions using Role Based Access Control (RBAC)</td><td>Medium</td><td>Yes</td></tr>
<tr><td>Storage Account, linked with Batch account, must be protected using Storage Service Encryption (SSE)</td><td>High</td><td>Yes</td></tr>
<tr><td>Secrets must be protected on Batch account compute nodes</td><td>High</td><td>No</td></tr>
<tr><td>Batch account access keys must be rotated periodically</td><td>Medium</td><td>No</td></tr>
<tr><td>Remote desktop connection should be disabled on Batch account compute nodes</td><td>High</td><td>No</td></tr>
<tr><td>Batch account tasks and jobs should be configured to persist output to Azure Blob Storage</td><td>Medium</td><td>No</td></tr>
<tr><td>Diagnostics logs must be enabled with a retention period of at least $($this.ControlSettings.Diagnostics_RetentionPeriod_Min) days</td><td>Medium</td><td>Yes</td></tr>
<tr><td>Metric alert rules must be configured on Batch account</td><td>Low</td><td>Yes</td></tr>
</table>
</body></html>
