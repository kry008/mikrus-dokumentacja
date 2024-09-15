# Free subdomain for VPS

VPS servers on Mikrus don't have their own IPv4 addresses, only shared TCP ports. However, it would not be so nice to have a website address like mywebsite:12345 ☹️

However, you have an IPv6 address at your disposal, so by connecting your domain in CloudFlare, you can tunnel IPv4 traffic to IPv6 and show your website to your readers without any problems. Only... first, you need to have/buy a domain.

It so happens that in the Mikrus panel you can click on a free subdomain in our domain and connect it to your server. (Works for paid Mikrus)

Another option (available mainly for [frog](/frog) servers but works for all servers) is the **wykr.es** domain!
- **server-port_number.wykr.es**

So if your VPS server is on machine **frog01** and your web application is listening on port **20100**, your domain address is:

- **frog01-20100.wykr.es**
- for port **30999** on **srv01** it will be **srv01-30999.wykr.es**

Important notes:

- the subdomain supports HTTP and HTTPS traffic
- SSL support is included. Do not configure any certificate, Let's Encrypt, etc. on your side. It is unnecessary, your own certificate may cause problems.
- The domain points to your IPv6 address, so your web server (e.g. Apache or nginX) must listen on this address (by default they listen on IPv4!)
- **the domain can NOT be used to log in via SSH** or to connect to ports other than 80/443

[Return to main page](/)