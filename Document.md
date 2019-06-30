## 1. Node.js 及 NPM


openssl dhparam -out /etc/ssl/certs/dhparam.pem 2048

mkdir -p /var/lib/letsencrypt/.well-known



certbot certonly --agree-tos --email admin@ssl.hiaoshojo.com --webroot -w /var/lib/letsencrypt/ -d ssl.hiaoshojo.com



- 是否願意接收訊息
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

```
Obtaining a new certificate
Performing the following challenges:
http-01 challenge for ssl.hiaoshojo.com
Using the webroot path /var/lib/letsencrypt for all unmatched domains.
Waiting for verification...
Cleaning up challenges

IMPORTANT NOTES:
 - Congratulations! Your certificate and chain have been saved at:
   /etc/letsencrypt/live/ssl.hiaoshojo.com/fullchain.pem
   Your key file has been saved at:
   /etc/letsencrypt/live/ssl.hiaoshojo.com/privkey.pem
   Your cert will expire on 2019-09-28. To obtain a new or tweaked
   version of this certificate in the future, simply run certbot
   again. To non-interactively renew *all* of your certificates, run
   "certbot renew"
 - Your account credentials have been saved in your Certbot
   configuration directory at /etc/letsencrypt. You should make a
   secure backup of this folder now. This configuration directory will
   also contain certificates and private keys obtained by Certbot so
   making regular backups of this folder is ideal.
 - If you like Certbot, please consider supporting our work by:

   Donating to ISRG / Let's Encrypt:   https://letsencrypt.org/donate
   Donating to EFF:                    https://eff.org/donate-le
```




## 參考資料
- How To Use Certbot Standalone Mode to Retrieve Let's Encrypt SSL Certificates on Ubuntu 18.04 : https://www.digitalocean.com/community/tutorials/how-to-use-certbot-standalone-mode-to-retrieve-let-s-encrypt-ssl-certificates-on-ubuntu-1804
- Secure Nginx with Let's Encrypt on Ubuntu 18.04 : https://linuxize.com/post/secure-nginx-with-let-s-encrypt-on-ubuntu-18-04/
