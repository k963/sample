<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"  "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<title>LogicApps</title>
</head><body>
<table>
<colgroup><col/><col/><col/></colgroup>
<tr><th>Description</th><th>ControlSeverity</th><th>Automated</th></tr>
<tr><td>Multiple Logic Apps should not be deployed in the same resource group unless they trust each other</td><td>High</td><td>Yes</td></tr>
<tr><td>Logic App connectors must use AAD-based authentication wherever possible</td><td>High</td><td>Yes</td></tr>
<tr><td>Logic App connectors must have minimum required permissions on data source</td><td>Medium</td><td>No</td></tr>
<tr><td>All users/identities must be granted minimum required permissions using Role Based Access Control (RBAC)</td><td>Medium</td><td>Yes</td></tr>
<tr><td>If Logic App fires on an HTTP Request (e.g. Request or Webhook) then provide IP ranges for triggers to prevent unauthorized access</td><td>High</td><td>Yes</td></tr>
<tr><td>Must provide IP ranges for contents to prevent unauthorized access to inputs/outputs data of Logic App run history</td><td>High</td><td>Yes</td></tr>
<tr><td>Data transit across connectors must use encrypted channel</td><td>High</td><td>Yes</td></tr>
<tr><td>Application secrets and credentials must not be in plain text in source code (code view) of a Logic App</td><td>High</td><td>Yes</td></tr>
<tr><td>Logic App access keys must be rotated periodically</td><td>Medium</td><td>No</td></tr>
<tr><td>Diagnostics logs must be enabled with a retention period of at least $($this.ControlSettings.Diagnostics_RetentionPeriod_Min) days.</td><td>Medium</td><td>Yes</td></tr>
<tr><td>Logic App Code View code should be backed up periodically</td><td>Medium</td><td>No</td></tr>
</table>
</body></html>
