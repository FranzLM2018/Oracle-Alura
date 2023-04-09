# IMPORTANT:
This script has been tested on ubuntu 20.04.

# Odoo script install(odoofranz.sh):

This script works on ubuntu 20.04(not tested on 22.04 or higher); the script is a merger of the Yenthe666(https://github.com/Yenthe666/InstallScript) 
script and the OdooPeru(https://odooperu.org/?cat=50) script, after installing odoo with the script activate the proxymode to True and the workers to 2,
in the odoo.conf file found in the path /etc/odoo/odoo.conf.

# Ngnix-Certbot script install (nginxfranz.sh):

Script install ngnix-cerbot(nginxfranz.sh):<br>
This script is for those who want to add a domain to odoo, with nginx and cerbot; this script is taken from Yenthe666(https://github.com/Yenthe666/InstallScript#odoo-install-script).

# Installation procedure(for both scripts only rename the file):

1. Download the script:<br>

<pre><code class="language-javascript">sudo wget https://raw.githubusercontent.com/FranzLM2018/Odoo/16.0/odoofranz.sh</code></pre>
<pre><code class="language-javascript">sudo wget https://raw.githubusercontent.com/FranzLM2018/Odoo/16.0/nginxfranz.sh</code></pre>


2. Modify the parameters as you wish:<br>
Configure:<br>
WEBSITE_NAME="_" Switch to your personal domain.<br>
INSTALL_NGINX="True" True install nginx , False do not install nginx.<br>
ADMIN_EMAIL="odoo@example.com" Email is needed to register for Let's Encrypt registration.<br>
ENABLE_SSL="True" True to enable nginx and certbot.<br>
VERSION=15.0 Odoo version<br>
3. We give permission to the file:

<pre><code class="language-javascript">sudo chmod u+x odoofranz.sh</code></pre>
<pre><code class="language-javascript">sudo chmod u+x nginxfranz.sh</code></pre>

4.Run:

<pre><code class="language-javascript">sudo sh odoofranz.sh</code></pre>
<pre><code class="language-javascript">sudo sh nginxfranz.sh</code></pre>
