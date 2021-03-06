<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"  "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<title>NotificationHub</title>
</head><body>
<table>
<colgroup><col/><col/><col/></colgroup>
<tr><th>Description</th><th>ControlSeverity</th><th>Automated</th></tr>
<tr><td>Notification Hub must be created through Azure Resource Manager model</td><td>High</td><td>No</td></tr>
<tr><td>All users/identities must be granted minimum required permissions using Role Based Access Control (RBAC)</td><td>Medium</td><td>Yes</td></tr>
<tr><td>Applications must not use &#39;namespace&#39; level access policies for the Notification Hub</td><td>High</td><td>No</td></tr>
<tr><td>Access policies must be defined with minimum required permissions at Notification Hub level</td><td>Medium</td><td>No</td></tr>
<tr><td>Access policies on Notification Hub must not have Manage access permissions</td><td>High</td><td>Yes</td></tr>
<tr><td>Registration management must not be done from a native client or device app</td><td>Medium</td><td>No</td></tr>
<tr><td>Message body of a push notification must not contain sensitive data</td><td>High</td><td>No</td></tr>
<tr><td>Developers of applications that use Notification Hubs must not be granted persistent access on the subscription</td><td>Medium</td><td>No</td></tr>
<tr><td>Audit logs for Notification Hub should be enabled</td><td>Medium</td><td>No</td></tr>
<tr><td>Backup and Disaster Recovery must be planned for Notification Hub</td><td>Medium</td><td>No</td></tr>
</table>
</body></html>
