# Dokumentacja konfiguracja serwera FRONTEND

## Domeny

Staging: https://frontend-staging.culture.pl

Prod: https://culture.pl


## Nginx

Nie są wymagane szczególne wymagania jeśli chodzi o konfiguracje nginx. Konfiguracja w formie 
.htaccess (wymagana analogia w formacie konfiguracji nginx).

```
<IfModule mod_rewrite.c>
  RewriteEngine On
  RewriteBase /
  RewriteRule index.html index.php

  RewriteCond %{REQUEST_FILENAME} !-f
  RewriteCond %{REQUEST_FILENAME} !-d
  RewriteRule ^ index.php [L]
</IfModule>

<ifModule mod_gzip.c>
    mod_gzip_on Yes
    mod_gzip_dechunk Yes
    mod_gzip_item_include file .(html?|txt|css|js|php|pl)$
    mod_gzip_item_include handler ^cgi-script$
    mod_gzip_item_include mime ^text/.*
    mod_gzip_item_include mime ^application/x-javascript.*
    mod_gzip_item_exclude mime ^image/.*
    mod_gzip_item_exclude rspheader ^Content-Encoding:.*gzip.*
</ifModule>

```


## PHP
Frontend ma mieć możliwość wykonywania kod PHP (konfiguracja analogiczna jak w przypadku staging). 
Jedna dodatkowa zmiana: index.html ma być interepretowany jako plik PHP
