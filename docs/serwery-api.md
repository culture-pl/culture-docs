# Dokumentacja konfiguracji serwera API

## Cron 

Dla każdego środowiska (prod, preprod), wymagane są dwa wpisy w crontab:

``` bash
*/10 * * * * /usr/local/bin/drush -y -l http://api-staging.culture.pl --root=/data/staging/culture3/api/app core-cron
*/1  * * * * /usr/local/bin/drush -y -l http://api-staging.culture.pl --root=/data/staging/culture3/api/app pqw
```

Pierwszy wpisy powoduje odpalanie zadań aplikacji (wg wewnętrznego schedulera aplikacji). Drugi wpis powoduje czyszczenie 
cache dla zmodyfikowanych treści, dlatego wymagana jest duża częstliwość.

## PHP

### Lista modułów
Core
- ctype
- curl
- date
- dom
- exif
- filter
- gd
- hash
- iconv
- json
- libxml
- mbstring
- mysqli
- mysqlnd
- openssl
- pcre
- PDO
- pdo_mysql
- pdo_sqlite
- Phar
- posix
- redis
- Reflection
- session
- SimpleXML
- SPL
- sqlite3
- standard
- tokenizer
- xml
- xmlreader
- xmlwriter
- Zend OPcache

### Ustawienia niestandardowe CLI
- Globalny konfig dla PHP wykonujący się jako CLI, z następującymi zmianami
```
opcache.enable_cli => 1
memory_limit => 1024M
max_execution_time => 0
```

### Ustawienia niestandardowe - WEB
Należy pamiętać o zwiększeniu limiti dla uploadu plików, w szczególności
```
upload_max_filesize => 32M
post_max_size => 8M
```

## Elastic search

## Serwer redis 

## Mariadb 

Wymagane są dwie bazy danych
1. Bieżąca, z której aplikacja będzie korzystać przez cały czas działania
2. Pomocniczna, z której będą zaciągane dane na czas migracji. 

Szczegóły: https://redmine.culture.pl/issues/2172

## Serwer nginx

Wzorcową konfiguracją jest konfiguracja z [nginx for Drupal 8](https://www.nginx.com/resources/wiki/start/topics/recipes/drupal/)


## Logi aplikacji

- PHP
- Slow query
- Syslog
- Nginx

