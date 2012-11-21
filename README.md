yasca-rules
===========

Additional signatures for source code security scanning with [Yasca](http://www.yasca.org/). 
These rules were mostly ported from [WCSA](http://code.google.com/p/wcsa/source/browse/#svn%2Ftrunk%2FWCSA%2FVulnFiles).

Installation
------------
1. Download and install [Yasca](http://www.yasca.org/).
2. Copy all *.grep files into `plugins/default/grep` in Yasca directory

WCSA Mapping
------------
<table>
<thead>
<tr><th colspan=2>WCSA  <th>Yasca
<tr><th>File  <th>Rule  <th>File
</thead>
<tbody>
<tr><td>compilation.xml <td>Debugging Enabled <td>InfoDisclosure.Debug.grep
<tr><td>credentials.xml <td>Clear-text credentials <td>Authentication.StoredPassword.grep
<tr><td>customErrors.xml  <td>Custom Errors Disabled  <td>InfoDisclosure.customErrors.grep
<tr><td>forms.xml <td>Cookieless Authentication Enabled <td>Session.Cookieless.grep
<tr><td>forms.xml <td>Doesn't Require SSL for Auth. Cookies <td>Session.SSL.grep
<tr><td>forms.xml <td>Non-Unique Authentication Cookie Used <td>Session.ASPXAUTH.grep
<tr><td>forms.xml <td>Sliding Expiration Used <td>Session.SlidingExpiration.grep
<tr><td>forms.xml <td>Liberal Path Defined  <td>Session.LiberalPath.grep
<tr><td>forms.xml <td>URL Redirection is enabled  <td>Session.CrossApp.grep
<tr><td>forms.xml <td>Your form tickets are not both encrypted-validated  <td>Session.FormTicketsProtection.grep
<tr><td>forms.xml <td>Your form tickets are not validated <td>Session.FormTicketsValidation.grep
<tr><td>forms.xml <td>Your form tickets are not encrypted <td>Session.FormTicketsEncryption.grep
<tr><td>httpCookies.xml <td>Web cookies are not HttpOnly  <td>Session.httpOnly.grep 
<tr><td>httpCookies.xml <td>Web cookies doesn't require SSL  <td>Session.Secure.grep 
<tr><td>
</tbody>
</table>
