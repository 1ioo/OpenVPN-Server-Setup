<h1>OpenVPN-Server-Setup</h1>
<p>This python scripts automates the creation of an OpenVPN Server. Unfortunately only Linux is supported. Keys and Certificates are currently managed with Easy-RSA.</p>
<p><b>Menu</b>:<br>1.Server Set Up<br>2.Client Certificate Creation<br>3.Revoke Client Certificates<br></p>
<span><b>1. Server Set Up<br></b></span>
<span>This choice sets up the server automatically for you. Relevant packages are automatically downloaded. OpenVPN Server is set up on port 2876. Hardening is done on SSH (port changed to 2244) IPTable Rules are added for hardening as well. Fail2ban was added for blacklisting IPs</span><br><br>
<span><b>2. Client Certificate Creation</b></span><br>
<span>Client Certificate is created based on name specified and Client OS System. Created certificate will then be moved to the /tmp folder for transfer. Note that on Linux clients, the package "openvpn-systemd-resolved" needs to be installed ("apt install openvpn-systemd-resolved") to prevent DNS Leaks.</span><br><br>
<span><b>3. Revoke Client Certificates</b></span><br>
<span>Client Certificates are revoked, making them unable to authenticate and connect with the server.</span>
