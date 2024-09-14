# Apache + PHP + MySQL

To set up LAMP (Linux + Apache + PHP + MySQL) is really easy, and you only need to run a few commands.

You need to run all commands below as `root` or at start of every line put `sudo`

First you need to update repositories

```bash
apt update
```
Next you need to install required packages

```bash
apt install apache2 mariadb-server mariadb-client php libapache2-mod-php -y
```

Page files put in **/var/www/html** catalog

To test PHP working, write below command and next run via web browser file `test.php`

```bash
echo "<?php phpinfo(); " >**/var/www/html/**test.php
```

That is all, now is time to [set up own domain via Cloudflare](../podpiecie_domeny_przez_cloudflare), [get free subdomain from panel](https://mikr.us/panel/?a=domain) or [to set up quick subdomain from VPS](../szybka_subdomena).

- To set up database [read this tutorial](../konfiguracja_mysql_mariadb)
- Read also [how to send files to Mikrus VPS](../jak_wysylac_pliki_na_mikrusa) 

[Return to main page](/)