# Formaty HTML (profile CKEditor) 
Formaty tekstów pozwalają na stworzenie różnych konfiguracji CKEditora i dopuszczalnego formatowania HTML. Ustawienia te mogą być wykorzystane dla pól stworzonych w obrębie typów zawartości, kategorii czy paragrafów.  
Poniżej podane zostały przykłady użycia poszczególnych konfiguracji dla niektórych pól; dokładniejsza rozpiska wykorzystanych formatów znajduje się przy opisie typów zawartości, paragrafów i kategorii.  

## Header Title (simple_html) 
### Opis 
Format tekstu z ograniczonym, podstawowym formatowaniem dedykowany wyłącznie dla tytułów nagłówków (np.: tytuły w header). Podczas wystawiania pola do json api tagi <p> są zamieniane na <span> (tag <p> nie jest dopuszczalny w <h1>); sam tag <p> jest zapisywany normalne w bazie danych tak żeby możliwe było formatowanie tekstu z poziomu CKEditor.
### Przypadki użycia  
field_hero_header_header, field_work_subtitle
### CKEditor  
bold, italic, underline, left, center, right, justify, source
### Dopuszczalne tagi  
< em > < strong > < u > < i > < br > < p class="text-align-left text-align-center text-align-right text-align-justify" >
### Dodatkowa funkcjonalność
Zmiana znaczników <p> na <span> (tekst wykorzystywany wewnątrz nagłówków).

## Basic HTML (basic_html)
### Opis
Podstawowy format używany przez redakcję dla standardowej treści artykułów i innych wpisów, które wymagają możliwości formatowania tekstu i dodawania różnych elementów HTML dopuszczalnych przez markup i style guide (np.: obrazek, lista, tabela).
### Przypadki użycia
field_hero_header_header, field_work_subtitle
### CKEditor
bold, italic, underline, sup, sub, left, center, right, justify, source, link, unlink, ul, ol, table, quota, iframe, image, block formating, source
### Dopuszczalne tagi
< a href hreflang > < em > < strong > < cite > < blockquote cite > < code > < ul type > < ol start type > < li > < dl > < dt > < dd > < h2 id > < h3 id > < h4 id > < h5 id > < h6 id > < p class="text-align-left text-align-center text-align-right text-align-justify" > < br > < span > < img src alt height width data-entity-type data-entity-uuid data-align data-caption > < iframe align frameborder height longdesc name scrolling src title width > < pre >< table id class >< thead >< tbody >< tfoot >< tr id class >< td class >< th id class >< sub >< sup >

## Limited HTML text only (limited_editor)
### Opis
Format tekstu z ograniczonym, podstawowym formatowaniem treści stosowany tam gdzie używany jest średniej długości tekst bez dodatkowych elementów html jak np.: tabele, listy czy obrazki. 
### Przypadki użycia
field_hero_header_lead, field_introduction, field_video_description, field_gallery_description
### CKEditor
bold, italic, underline, left, center, right, justify,link, unlink, source
### Dopuszczalne tagi
< em > < strong > < u > < i > < br > < p class="text-align-left text-align-center text-align-right text-align-justify" > < a href hreflang > < span class >

## Restricted HTML (restricted_html)
### Opis
Formatowanie stosowane tam, gdzie nie dajemy możliwości formatowania tekstu - format jest z góry określony przez style guide, np.: summary na listingach.
### Przypadki użycia
field_hero_header_pic_signature, field_venue_map_text, field_venue_contact_details
### CKEditor
bold, italic, link, unlink, source
### Dopuszczalne tagi
< a href hreflang > < em > < br > < span > < strong > < i > < p >

## Plain text (plain_text)
### Opis
Format tekstu dostępny dla wszystkich użytkowników; najbardziej restrykcyjny; całkowicie usuwa tagi HTML oprócz znaków nowej linii, które sam generuje. Stosowany tam gdzie formatowanie i tagi html nie są potrzebne.
### Przypadki użycia
field_summary, field_venue_map_tooltip_name
C### KEditor
CKEditor nie jest podpięty.

## Full HTML (full_html) 
Format tekstu „Full HTML” nie jest używany, ale zostaje w systemie w standardowej formie.
