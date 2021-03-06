<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"  "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<title>HTML TABLE</title>
</head><body>
<table>
<colgroup><col/><col/><col/></colgroup>
<tr><th>Description</th><th>ControlSeverity</th><th>Automated</th></tr>
<tr><td>Event Hub namespace must be created using the Azure Resource Manager (ARM) model</td><td>High</td><td>No</td></tr>
<tr><td>ACS mechanism must not be used to authenticate Event Hub entities</td><td>High</td><td>No</td></tr>
<tr><td>Event Hub clients (event senders or receivers) must not use &#39;namespace&#39; level access policies</td><td>Medium</td><td>Yes</td></tr>
<tr><td>Access policies must be defined with minimum required permissions to the Event Hub</td><td>Medium</td><td>Yes</td></tr>
<tr><td>Access policy keys must be protected at rest</td><td>High</td><td>No</td></tr>
<tr><td>Access policy keys must be rotated periodically</td><td>Medium</td><td>No</td></tr>
<tr><td>Audit logs for Event Hub entities should be reviewed periodically</td><td>Medium</td><td>No</td></tr>
<tr><td>Sensitive data must be encrypted in transit</td><td>High</td><td>No</td></tr>
<tr><td>Expiry time of SAS token should be minimum required</td><td>Medium</td><td>No</td></tr>
<tr><td>Use &#39;Publisher&#39; tokens to authenticate senders instead of &#39;Access Policy&#39; tokens</td><td>Medium</td><td>No</td></tr>
<tr><td>All users/identities must be granted minimum required permissions using Role Based Access Control (RBAC)</td><td>Medium</td><td>Yes</td></tr>
<tr><td>Diagnostics logs must be enabled with a retention period of at least $($this.ControlSettings.Diagnostics_RetentionPeriod_Min) days</td><td>Medium</td><td>Yes</td></tr>
</table>
</body></html>
