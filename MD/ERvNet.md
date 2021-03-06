<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"  "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<title>HTML TABLE</title>
</head><body>
<table>
<colgroup><col/><col/><col/></colgroup>
<tr><th>Description</th><th>ControlSeverity</th><th>Automated</th></tr>
<tr><td>There must not be any Public IPs (i.e., NICs with PublicIP) on ExpressRoute-connected VMs</td><td>High</td><td>Yes</td></tr>
<tr><td>There must not be multiple NICs on ExpressRoute-connected VMs</td><td>Medium</td><td>Yes</td></tr>
<tr><td>The &#39;EnableIPForwarding&#39; flag must not be set to true for NICs in the ExpressRoute-connected vNet</td><td>High</td><td>Yes</td></tr>
<tr><td>There must not be any NSGs on the GatewaySubnet of the ExpressRoute-connected vNet</td><td>Medium</td><td>Yes</td></tr>
<tr><td>There must not be a UDR on *any* subnet in an ExpressRoute-connected vNet</td><td>High</td><td>Yes</td></tr>
<tr><td>There must not be another virtual network gateway (GatewayType = Vpn) in an ExpressRoute-connected vNet</td><td>High</td><td>Yes</td></tr>
<tr><td>There must not be any virtual network peerings on an ExpressRoute-connected vNet</td><td>High</td><td>Yes</td></tr>
<tr><td>Only internal load balancers (ILBs) may be used inside an ExpressRoute-connected vNet</td><td>High</td><td>Yes</td></tr>
<tr><td>Only resources of type Microsoft.Network/* must be added in the ERNetwork resource group</td><td>High</td><td>Yes</td></tr>
<tr><td>Ensure that the ERNetwork resource group is protected with a resource lock</td><td>High</td><td>Yes</td></tr>
</table>
</body></html>
