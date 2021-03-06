<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"  "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<title>HTML TABLE</title>
</head><body>
<table>
<colgroup><col/><col/><col/></colgroup>
<tr><th>Description</th><th>ControlSeverity</th><th>Automated</th></tr>
<tr><td>Publicly exposed microservice endpoints must have authentication and authorization enforced</td><td>High</td><td>No</td></tr>
<tr><td>Publicly exposed endpoints must be secured using SSL</td><td>High</td><td>No</td></tr>
<tr><td>Application secrets must be encrypted with a certificate</td><td>High</td><td>No</td></tr>
<tr><td>Data replication must be secured with certificate</td><td>Medium</td><td>No</td></tr>
<tr><td>Sensitive data must not be stored inside DataPackage</td><td>High</td><td>No</td></tr>
<tr><td>Replica set size for stateful services must be set to a minimum of 3</td><td>Medium</td><td>No</td></tr>
<tr><td>Instance count for stateless service must be set to a minimum of 3</td><td>Medium</td><td>No</td></tr>
<tr><td>Stateful microservices must be backed up to a geo-redundant Storage Account</td><td>Medium</td><td>No</td></tr>
<tr><td>Service Fabric cluster security must be enabled using security mode option</td><td>High</td><td>Yes</td></tr>
<tr><td>Service Fabric cluster must contain only microservices which trust each other</td><td>High</td><td>No</td></tr>
<tr><td>Self-signed certs must not be used for Service Fabric cluster primary certificate</td><td>High</td><td>Yes</td></tr>
<tr><td>Client authentication must be performed only via Azure Active Directory</td><td>High</td><td>Yes</td></tr>
<tr><td>The ClusterProtectionLevel property must be set to EncryptAndSign</td><td>High</td><td>Yes</td></tr>
<tr><td>Network security group (NSG) must be enabled on subnets of Service Fabric cluster</td><td>Medium</td><td>Yes</td></tr>
<tr><td>Encryption must be enabled on all storage accounts which store VHDs of Service Fabric cluster VMs</td><td>High</td><td>Yes</td></tr>
<tr><td>Diagnostics must be enabled for Service Fabric cluster</td><td>Medium</td><td>Yes</td></tr>
<tr><td>Monitor publicly exposed ports on load balancers used by Service Fabric cluster</td><td>Medium</td><td>No</td></tr>
</table>
</body></html>
