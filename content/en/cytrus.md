# Cytrus

Cytrus is a shared web server service (this is Nginx) that allows you to host websites without having to install a web server.

This service natively supports static pages and those created in PHP (e.g. Wordpress).

> 💡 If you want to add your own DOMAIN to Cytrus, you need to point its “A” entry to IP:
> **135.181.95.85**

> 💡 If you want to add your own SUB-DOMAIN to Cytrus, you need to point its “CNAME” entry to:
> **backend.strony.me**

**Additional benefits of Cytrus are::**

- ability to redirect a domain to any IP address and port (the WWW service does not have to listen on port 80)
- ability to access the server using a shared FTP server
- support for any number of domains

**Limitations:**
- Cytrus is shared, so to ensure a comfortable experience for all users, keep all files under 3 GB
- Since cytrus is on a separate, more powerful machine, following symlinks to a VPS is not possible

**Ciekawostki**

- if instead of the target directory you provide a domain address or server IP address along with the port number, Cytrus will redirect traffic to it (for example, provide: http://1.2.3.4:3000)
- as the 'target directory' you can provide the URL of the page in Notion. You will then be able to host pages from Notion on your own domain/subdomain.

Cytrus is NOT required to host your own sites on Mikrus.

It is only an optional convenience.

[Return to main page](/)
