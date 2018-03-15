# Wprowadzenie #

W przypadku cachewania całych adresów URL, culture3 skonfigurowany jest do korzystania z dwóch warstw cachewania

1. Varnish
2. Internal cache

Dla każdej podstrony, Drupal zarządza listą powiązań, tagów dzięki którym jest w stanie w inteligentny sposób czyścić
cache obiektów powiązanych z danym widokiem. Np. Cache strony głównej zostanie wyczyszczony, gdy np. zostanie zaktualizowany
zostanie artykuł wyświetlany na stronie głównej. 

Dzięki temu można osiągnąć dużo wyższy HIT-RATE i oszczędzić zasoby serwera. 


# Konfiguracja aplikacji #

Aplikacja generuje nagłówki trwania cache na okres **1 roku**. Przy wszystkich odpowiedziach z serwera, dodawany jest nagłówkek
**Cache-Tags**, zawierający listę powiązanych z daną odpowiedzią tagów.

Raz na minutę (za pomocą cron), wykonywane jest polecenie ```drush pqw```, które wykonuje zapytanie typu "BAN" do serwera varnisha (obecnie **10.20.30.201** port 81).
Serwer skonfigurowany jest, by wykonywać max 100 requestów BAN na wykonanie. 

Dodatkowo, w celu czyszczenia cache dla URL-i do obrazków, w przypadku modyfikacji obrazka, wykonywane jest zapytanie URIBAN do serwera varnisha.

# Wymagania od środowiska

Wymagane jest, by serwer varnish akceptował requesty BAN / URIBAN z serwera aplikacji. Przykładowa konfiguracja opisana jest
- [drupal.org - Cache tags](https://www.drupal.org/docs/8/api/cache-api/cache-tags-varnish)
- [drupal.org - dokumentacja modułu varnish purger](https://www.drupal.org/project/varnish_purge) - tutaj opisana jest konfiguracja URIBAN

# Wymuszenie czyszczenie cache (IAM)
Logując się na:
10.20.30.9 (aktualna produkcja):

Usuwanie cache:

`sudo czysc-api`
Usuwa cały cache z https://api.culture.pl

`sudo czysc-api-staging`
Usuwa cały cache z https://api-staging.culture.pl
​
`sudo czysc-frontend`
Usuwa cały cache z https://frontend.culture.pl

`sudo czysc-frontend-staging`
Usuwa cały cache z https://frontend-staging.culture.pl

`sudo listabanow-culture3`
Pokazuje całą listę banów.

Jeżeli cokolwiek Ci nie działa, to przeanalizuj reguły.
