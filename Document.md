## 1. Node.js 及 NPM


openssl dhparam -out /etc/ssl/certs/dhparam.pem 2048

mkdir -p /var/lib/letsencrypt/.well-known



certbot certonly --agree-tos --email admin@ssl.hiaoshojo.com --webroot -w /var/lib/letsencrypt/ -d ssl.hiaoshojo.com

```
Saving debug log to /var/log/letsencrypt/letsencrypt.log
Plugins selected: Authenticator webroot, Installer None

-------------------------------------------------------------------------------
Would you be willing to share your email address with the Electronic Frontier
Foundation, a founding partner of the Let's Encrypt project and the non-profit
organization that develops Certbot? We'd like to send you email about EFF and
our work to encrypt the web, protect its users and defend digital rights.
-------------------------------------------------------------------------------
(Y)es/(N)o:
```




## 參考資料
- How To Use Certbot Standalone Mode to Retrieve Let's Encrypt SSL Certificates on Ubuntu 18.04 : https://www.digitalocean.com/community/tutorials/how-to-use-certbot-standalone-mode-to-retrieve-let-s-encrypt-ssl-certificates-on-ubuntu-1804
- Secure Nginx with Let's Encrypt on Ubuntu 18.04 : https://linuxize.com/post/secure-nginx-with-let-s-encrypt-on-ubuntu-18-04/
