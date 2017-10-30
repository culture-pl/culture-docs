# Rodzaje zawartości migracja z Culture 2.0 do Culture 3.0

## Artykuł - (Nazwa systemowa: article)

Pełna lista pól: https://docs.google.com/spreadsheets/d/1PQ03X3oNQGFTX10DbkY-0hIfTGYOpSYJUzXbmV7Dvuk/edit#gid=0
 - Pole tytuł (title)
 - Język - wybór dostępnych jezyków.
 - Rodzaj treści - Referencja do słownika rodzajów treści, dla statystyk wiedzy. (pole niewidoczne)
 - Top photo **Migracja do paragrafu**
 - Okładki:  **3.0 nowe pole**
   - Prostokątna pole wyboru pliku zdjęcia.    
   - Kwadratowa pole wyboru pliku zdjęcia.   
 - Treść artykułu – Długi tekst i podsumowanie. (Nazwa systemowa: body) **Migracja do paragrafu**
 - Powiązane elementy – referencja do encji  
 - Youku – zastepstwo filmów iframe z youtube i vimeo w Chinach. **Brak decyzji**
 - Kategoria – Referencja do słownika kategorii.  
 - Tagi - Referencja do słownika tagów.  
 - Artykuł polecany – Boolean  
 - Artykuł przekrojowy - Boolean 
 - Aktualność - Boolean  **Brak decyzji**
 - Pokaż obrazek w zajawce - Boolean   **Brak decyzji**
 - Azja Kategorie – select list - powiązane kraje w Azja  
 - Treści dot. projektów IAM – statystyka wpisów dotyczących IAM  
 - Mapa XML witryny  
 - Alias  
 - Metatagi   
 - Przekierowania URL  
 - Artykuł promowany w stopce – ukryte pole  
 - Autor  
 - Data publikacji  
 - Data aktualizacji  
 - Rewizje  


### Pola dodane w Culture 3.0

- Paragraf top_photo 
  - Paragraf top_photo_default 
      - Field top_photo_default_img (**Tu migrujemy top_photo z Culture 2.0**)  
      - Title
      - Alt
    - top_photo_full 
      - Field top_photo_full_img (Nowe pole Culture 3.0)
      - Title
      - Alt
- Paragraf body, do wyboru: 
    - Node embed article  
    - Pole tekstowe - text area
    
- Okładki, pola z wybore zdjeć:
   - Prostokątna pole wyboru pliku zdjęcia (poziom).    
   - Kwadratowa pole wyboru pliku zdjęcia.  
   - Prostokątna pole wyboru pliku zdjęcia (pion, **nowe pole**).  

### Pole nie migrowane

 - Link - Link wyszukiwania.  
 - Editing time – pole tekstowe – liczba całkowita  
 - Liferay: LR UUID, LR Group Id  
 - Chars count – ukryte pole  
 - A-Z – Referencja do słownika A-Z – ukryte pole  
 - Domain Access – wybór domen w których ma być wyświetlany wpis. (Potrzeba decyzji czy migrujemy to do jakiegoś osobnego słownika)  


## Dzieło (Nazwa systemowa: works)
 Typ zawartości opisujące dzieło danego twórcy.
 
- Tytuł – Pole tytuł (Nazwa systemowa: title)
- Język - wybór języka treści
- Twórca – Pole referencja do twórcy.
- Opis dzieła – Długi tekst i podsumowanie. (Nazwa systemowa: body)
- Data premiery – pole z kalendarzem
- Okładki
    - Okładka dzieła (kwadratowa) pole wyboru pliku zdjęcia.
    - Okładka dzieła (prostokątna) pole wyboru pliku zdjęcia.
- Kategoria - Referencja do słownika kategorii.
- Tagi - Referencja do słownika tagów, w których ma wyświetlać się slide.
- A-Z – Referencja do słownika A-Z.
- Rodzaj treści – lista wyboru do filtrowania statystyk (Dużo wiedzy, Trochę wiedzy, zero
wiedzy)
- Mapa XML witryny, 
- Alias
- Meta tagi 
- Przekierowania URL
- Treści dot. projektów IAM – statystyka wpisów dotyczących IAM
- Autor 
- Data publikacji
- Data aktualizacji
- Opublikowane 
- Promowane na głównej
- Rewizje


### Pole nie migrowane
- Domain Access – wybór domen w których ma być wyświetlany wpis.



## Formularz (Nazwa systemowa: webform)
 Rodzaj zawartości do tworzenia formularzy kontaktowych lub do
zbierania ankiet.
- Tytuł – Pole tytuł (Nazwa systemowa: title)
- Język - wybór języka treści
- Opis, długi tekst i podsumowanie. (Nazwa systemowa: body)
- Mapa XML witryny, 
- Alias
- Meta tagi 
- Przekierowania URL
- Autor 
- Data publikacji
- Data aktualizacji
- Opublikowane 
- Promowane na głównej
- Rewizje

### Pole nie migrowane
- Domain Access – wybór domen w których ma być wyświetlany wpis.

## Galeria (Nazwa systemowa: gallery)
 Rodzaj zawartości do załaczania kolekcji zdjeć. Galerię można dołączyć potem do
artykułu.
- Tytuł – Pole tytuł (Nazwa systemowa: title)
- Język - wybór języka treści
- Opis galerii, długi tekst i podsumowanie. (Nazwa systemowa: body)
- Autor zdjęć - Jednowierszowe pole tekstowe – podpis autora
- Rodzaj treści - Referencja do słownika rodzajów treści, dla statystyk wiedzy.
- Kategoria – Referencja do słownika kategorii.
- Tagi - Referencja do słownika tagów.
- Treści dot. projektów IAM – statystyka wpisów dotyczących IAM
- Lista zdjęć – pole wielowartościowe z plikami zdjęciowymi.
- Multimedia 
- Polecane na multimediach – lista wyboru
- Sekcja Specjalna – Lista wyboru
- Mapa XML witryny, 
- Alias
- Meta tagi 
- Przekierowania URL
- Autor 
- Data publikacji
- Data aktualizacji
- Opublikowane 
- Promowane na głównej
- Rewizje

### Pole nie migrowane
- Domain Access – wybór domen w których ma być wyświetlany wpis.
- Galeria polecana – Boolean - ukryty• 
- Dodaj do menu – Boolean


## Miejsce (Nazwa systemowa: venue)
 
 Miejsce dowiązywane do wydarzeń.
 
- Nazwa miejsca – Pole tytuł (Nazwa systemowa: title)
- Język - wybór języka treści
- Opis miejsca, długi tekst i podsumowanie. (Nazwa systemowa: body)
- Youku – zastepstwo filmów iframe z youtube i vimeo w Chinach.
- Kategoria – Referencja do słownika kategorii.
- Tagi - Referencja do słownika tagów.
- Okładki
    - Okładka dzieła (kwadratowa) pole wyboru pliku zdjęcia.
    - Okładka dzieła (prostokątna) pole wyboru pliku zdjęcia.
- Polecane miejsce – Boolean
- Rodzaj miejsca – Referencja do słownika terminów Rodzaje miejsca.
- Rodzaj treści - Referencja do słownika rodzajów treści, dla statystyk wiedzy. (ukryte)
- Treści dot. projektów IAM – statystyka wpisów dotyczących IAM
- Mapa XML witryny, 
- Alias
- Meta tagi 
- Przekierowania URL
- Autor 
- Data publikacji
- Data aktualizacji
- Opublikowane 
- Promowane na głównej
- Rewizje

### Pole nie migrowane
- Domain Access – wybór domen w których ma być wyświetlany wpis.
 

## Porównanie wczoraj i dziś (Nazwa systemowa: beforeafter)
- Tytuł – Pole tytuł (Nazwa systemowa: title)
- Język - wybór języka treści
- Obraz wczoraj - pole wyboru pliku zdjęcia.
- Obraz dziś - pole wyboru pliku zdjęcia.• Treści dot. projektów IAM – statystyka wpisów dotyczących IAM
- Mapa XML witryny, 
- Alias
- Meta tagi 
- Przekierowania URL
- Autor 
- Data publikacji
- Data aktualizacji
- Opublikowane 
- Promowane na głównej
- Rewizje

### Pole nie migrowane
- Domain Access – wybór domen w których ma być wyświetlany wpis.


## Statyczna strona (Nazwa systemowa: page)
 Prosta, statyczna strona przydatna do podstron informacyjnych.
- Tytuł – Pole tytuł (Nazwa systemowa: title)
- Język - wybór języka treści
- Treść - długi tekst i podsumowanie. (Nazwa systemowa: body)
- Załączone pliki – pole plik
- Kategoria – Referencja do słownika kategorii.
- Tagi - Referencja do słownika tagów.
- Treści dot. projektów IAM – statystyka wpisów dotyczących IAM
- Mapa XML witryny, 
- Alias
- Meta tagi 
- Przekierowania URL
- Autor 
- Data publikacji
- Data aktualizacji
- Opublikowane 
- Promowane na głównej
- Rewizje

### Pole nie migrowane
- Domain Access – wybór domen w których ma być wyświetlany wpis.


## Strona książki (Nazwa systemowa: book)
Książki posiadają wbudowaną nawigację hierarchiczną. Do
wykorzystania przy podręcznikach i przewodnikach.
- Tytuł – Pole tytuł (Nazwa systemowa: title)
- Język - wybór języka treści
- Treść - długi tekst i podsumowanie. (Nazwa systemowa: body)
- Mapa XML witryny, 
- Alias
- Meta tagi 
- Przekierowania URL
- Autor 
- Data publikacji
- Data aktualizacji
- Opublikowane 
- Promowane na głównej
- Rewizje

### Pole nie migrowane
- Domain Access – wybór domen w których ma być wyświetlany wpis.


## Twórca (Nazwa systemowa: artist)
 Rodzaj zawartosći do przechowywania informacji o twóracach.

- Imię i nazwisko twórcy – title
- Język - wybór języka treśc
- Opis - długi tekst i podsumowanie. (Nazwa systemowa: body)
- Krótki opis twórcy – jednowierczowe pole tekstowe.
- Sylwetka Culture – Boolean
- Top photo - pole wyboru pliku zdjęcia.
- Okładki
    - Okładka dzieła (kwadratowa) pole wyboru pliku zdjęcia.
    - Okładka dzieła (prostokątna) pole wyboru pliku zdjęcia.
- Related artists – referencja do Artystów powiązanych.
- Lata życia – pole tekstowe - narodziny i śmierć
- Rodzaj treści - Referencja do słownika rodzajów treści, dla statystyk wiedzy. (ukryte)
- A-Z – Referencja do słownika A-Z
- Kolejność sortowania – pole tekstowe.
- Youku – zastepstwo filmów iframe z youtube i vimeo w Chinach.
- Kategoria – Referencja do słownika kategorii.
- Tagi - Referencja do słownika tagów.
- Treści dot. projektów IAM – statystyka wpisów dotyczących IAM
- Mapa XML witryny, 
- Alias
- Meta tagi 
- Przekierowania URL
- Autor 
- Data publikacji
- Data aktualizacji
- Opublikowane 
- Promowane na głównej
- Rewizje

### Pole nie migrowane
- Domain Access – wybór domen w których ma być wyświetlany wpis.



## Wideo (Nazwa systemowa: video)
 Film z zewnętrznego serwisu, takiego, jak Youtube i Vimeo.

- Tytuł – Pole tytuł (Nazwa systemowa: title)
- Język - wybór języka treści
- Opis filmu - długi tekst i podsumowanie. (Nazwa systemowa: body)
- Pole wideo
- Kod EMBED - Długi tekst i podsumowanie•
- Powiązane elementy – referencja do encji
- Stopklatka filmu – pole wyboru pliku zdjęcia.
- Odtwarzaj automatycznie – Boolean
- Wideo polecane – Boolean
- Multimedia
- Polecane na multimediach – Boolean
- Sekcja Specjalna – Boolean
- Ikona Youtube - pole wyboru pliku zdjęcia.
- Wideo polecane w stopce – Boolean
- Youku – zastepstwo filmów iframe z youtube i vimeo w Chinach
- Rodzaj treści - Referencja do słownika rodzajów treści, dla statystyk wiedzy. (ukryty)
- Kategoria – Referencja do słownika kategorii.
- Tagi - Referencja do słownika tagów.
- Treści dot. projektów IAM – statystyka wpisów dotyczących IAM
- Mapa XML witryny, 
- Alias
- Meta tagi 
- Przekierowania URL
- Autor 
- Data publikacji
- Data aktualizacji
- Opublikowane 
- Promowane na głównej
- Rewizje

### Pole nie migrowane
- Domain Access – wybór domen w których ma być wyświetlany wpis.
- Dodaj do menu – Boolean
- Top photo - pole wyboru pliku zdjęcia – ukryty


## Wydarzenie (Nazwa systemowa: event)

 Wydarzenie z datą opisem i powiązanym miejscem.
 
- Tytuł– Pole tytuł (Nazwa systemowa: title)
- Język - wybór języka treść.
- Miejsce – Referencja do miejsca.
- Baidu – pole z konfiguracją Baidu maps (China).
- Data wydarzenia – pole kalendarza – czas trwania od dnia do dnia
- Opis wydarzenia - długi tekst i podsumowanie. (Nazwa systemowa: body)
- Youku - zastepstwo filmów iframe z youtube i vimeo w Chinach.
- Okładki
    - Okładka dzieła (kwadratowa) pole wyboru pliku zdjęcia.
    - Okładka dzieła (prostokątna) pole wyboru pliku zdjęcia.
- Photo - pole wyboru pliku zdjęcia z crop.
- Galeria – Referencja do Galerii.
- Miasta – Referencja do terminu ze słownika Miasta.
- Kup bilet – Link do miejsca zakupu biletu na wydarzenie.
- Wydarzenie polecane – Boolean
- Odliczanie – Boolean
- Państwa Azja – Referencja do terminu ze słownika Państwa Azja
- Powiązane elementy – Referencja do encji zawartości.
- Rodzaj treści - Referencja do słownika rodzajów treści, dla statystyk wiedzy (ukryte).
- Kategoria – Referencja do słownika kategorii.•
- Tagi - Referencja do słownika tagów.
- Treści dot. projektów IAM – statystyka wpisów dotyczących IAM
- Mapa XML witryny, 
- Alias
- Meta tagi 
- Przekierowania URL
- Autor 
- Data publikacji
- Data aktualizacji
- Opublikowane 
- Promowane na głównej
- Rewizje

### Pole nie migrowane
- Domain Access – wybór domen w których ma być wyświetlany wpis.
- Liferay: LR UUID, LR Group Id


## Wydarzenie live (Nazwa systemowa: live_events)
 Rodzaj wydarzenia z transmisją live i widgetami Twitter/Instagram.

- Tytuł– Pole tytuł (Nazwa systemowa: title)
- Język - wybór języka treść.
- Miejsce – Referencja do miejsca.
- Data wydarzenia – pole kalendarza – czas trwania od dnia do dnia
- Opis wydarzenia - długi tekst i podsumowanie. (Nazwa systemowa: body)
- Baidu – pole z konfiguracją Baidu maps (China).
- Youku - zastepstwo filmów iframe z youtube i vimeo w Chinach.
- Okładki
    - Okładka dzieła (kwadratowa) pole wyboru pliku zdjęcia.
    - Okładka dzieła (prostokątna) pole wyboru pliku zdjęcia.
- Kod transmisji live – Długie pole testowe – embed
- Twitter ID – pole tekstowe
- Instagram hashtag – pole tekstowe
- Rodzaj treści - Referencja do słownika rodzajów treści, dla statystyk wiedzy (ukryte).
- Kategoria – Referencja do słownika kategorii.•
- Tagi - Referencja do słownika tagów.
- Treści dot. projektów IAM – statystyka wpisów dotyczących IAM
- Mapa XML witryny, 
- Alias
- Meta tagi 
- Przekierowania URL
- Autor 
- Data publikacji
- Data aktualizacji
- Opublikowane 
- Promowane na głównej
- Rewizje

### Pole nie migrowane
- Domain Access – wybór domen w których ma być wyświetlany wpis.
- Liferay: LR UUID, LR Group Id



## Box (Nazwa systemowa: box)
 Boxy wyświetlane w Top Menu. **Nie migrowany**
 - Tytuł – Pole tytuł  
 - Język - wybór języka treści  
 - URL boksu - Link do którego prowadzi box.  
 - Tło Boksu - pole do załadowania pliku obrazu tła.  
 - Typ Boxu – lista meu w których box może być umieszczony  
 - Rodzaj Boxu – rodzaj wyświetlania boxu  
 - Autor    
 - Data publikacji  
 - Data aktualizacji   
 - Opublikowane  
 - Promowane na głównej  
 - Rewizje  
 - Domain Access – wybór domen w których ma być wyświetlany wpis. (Potrzeba decyzji czy migrujemy to do jakiegoś osobnego słownika)
 - Treści dot. projektów IAM – statystyka wpisów dotyczących IAM


## FrontBox (Nazwa systemowa: frontbox) 
 
 Boks na stronie głównej. **Nie migrowany**
 
- Tytuł – Pole tytuł (Nazwa systemowa: title)
- Język - wybór języka treści
- Rodzaj boksu – lista z wyborem typu boxa.
- Zawartość boksu – Długi tekst i podsumowanie. (Nazwa systemowa: body)
- Tło boksu - pole wyboru pliku zdjęcia.
- Rozmiar boksu – wybór rozmiaru boxu.
- URL boksu - Link do którego prowadzi box.
- Lista odnośników – Lista linków wyświetlana w boksie.
- Kolor tła licznika - wybór koloru – wartość RGB hex.
- Data, do której odlicza licznik - pole z kalendarzem.
- Azja Kategorie - select list - powiązane kraje w Azja.
- Domain Access – wybór domen w których ma być wyświetlany wpis.
- Treści dot. projektów IAM – statystyka wpisów dotyczących IAM
- Mapa XML witryny, 
- Alias
- Meta tagi 
- Przekierowania URL
- Autor 
- Data publikacji
- Data aktualizacji
- Opublikowane 
- Promowane na głównej
- Rewizje

 
## FrontSlide (Nazwa systemowa: front_slide) 

Slajd w sliderze u góry strony głównej i strony kategorii. **Nie migrowany**
- Powiązany artykuł - Odnośnik do encji – Autouzupełnianie
- Tytuł slajdu – Pole tytuł
- Obraz – pole do załadowania zdjęcia z mechanizmem crop
- Język - wybór języka treści
- Where should be shown - radio button – powiązany projekt
- Azja Kategorie – select list - powiązane kraje w Azja
- Kolor tła – wybór koloru – wartość RGB hex
- URL – Link do którego prowadzi slide.• Opis slajdu – długi tekst
- Kategoria – Referencja do słownika kategorii, w których ma wyświetlać się slide.
- Tagi - Referencja do słownika tagów, w których ma wyświetlać się slide.

- Przesunięcie na stronie głównej – X i Y – ustawienie niestandardowej wysokości baneru
- Przesunięcie w kategorii – X i Y – ustawienie niestandardowej wysokości baneru
- Kampania Analytics - Włącz kampanię niestandardową, UTM Source, UTM Medium,
UTM Campaign
- Domain Access – wybór domen w których ma być wyświetlony slide
- Treści dot. projektów IAM – statystyka wpisów dotyczących IAM
- Mapa XML witryny, 
- Alias
- Meta tagi 
- Przekierowania URL
- Autor 
- Data publikacji
- Data aktualizacji
- Opublikowane 
- Promowane na głównej
- Rewizje
