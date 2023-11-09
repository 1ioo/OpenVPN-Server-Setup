<h1>OpenVPN-Server-Setup</h1>
<p>This python scripts automates the creation of an OpenVPN Server. Unfortunately only Linux is supported. Keys and Certificates are currently managed with Easy-RSA.</p>
<p><b>Menu</b>:\n1.Server Set Up\n2.Client Certificate Creation\n3.Revoke Client Certificates\n</p>
<span><b>1. Server Set Up\n</b></span>
<span>This choice sets up the server automatically for you. Relevant packages are automatically downloaded. OpenVPN Server is set up on port 2876. Hardening is done on SSH (port changed to 2244) IPTable Rules are added for hardening as well. Fail2ban was added for blacklisting IPs\n\n</span>
<span><b>2. Client Certificate Creation\n</b></span>
<span>Client Certificate is created based on name specified and Client OS System. Created certificate will then be moved to the /tmp folder for transfer. Note that on Linux clients, the package "openvpn-systemd-resolved" needs to be installed ("apt install openvpn-systemd-resolved") to prevent DNS Leaks.\n\n</span>
<span><b>3. Revoke Client Certificates\n</b></span>
<span>Client Certificates are revoked, making them unable to authenticate and connect with the server.</span>
