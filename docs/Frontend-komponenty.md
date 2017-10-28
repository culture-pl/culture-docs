# Komponenty frontendowe

## MAIN

src/**App.vue** - główny komponent który ładuje pozostałe


## COMMON (src/components/common)

#### Komponenty używane globalnie

**Main.vue** - komponent ładujący pozostałe elementy głównej zawartości  
**SidebarLeft.vue** -  komponent odpowiedzialny za lewy pasek boczny w głównym layoucie   
**SidebarRight.vue** -  komponent odpowiedzialny za prawy pasek boczny w głównym layoucie  
**Preloader.vue** - preloader pokazujący się podczas pobierania treści z API   
  
**Header.vue** - komponent ładujący pozostałe elementy górnej belki  
**HeaderText.vue** - teksty nagłówkowe (breadcrumb)  
**Search.vue** - komponent odpowiedzialny za wyszukiwarkę  
**ContrastSwitch.vue** - przełącznik wysokiego kontrastu   
**NavIcon.vue** - ikona sterująca wyświetlaniem głównego menu  
  
**Navigation.vue** - komponent ładujący pozostałe elementy głównej nawigacji  
**MainMenu.vue** - menu w główej nawigacji  
**Hashtags.vue** - hashtagi w głównej nawigacji  
**LangSwitch.vue** - przełącznik wersji językowych  
  
**Footer.vue** - stopka  
**FooterMenu.vue** - menu w stopce  
**ContactPopup.vue** - popup z formularzem kontaktowym; wywoływany po kliknięciu w element z klasą "contact-popup"  

#### Komponenty używane w konkretnych typach zawartości lub w określonych warunkach
  
**GalleryPicture.vue** - pojedyncze zdjęcie, składnik galerii wyświtlany w typie zawartości galeria (gallery)  
**GoogleMap.vue** - komponent wyświetlający mapę w postaci Google Maps używany w wydarzeniu (event) i miejscu (venue)  
**GoogleStreetView.vue** - komponent wyświetlający mapę w postaci Google Street View używany w miejscu (venue)  
**Member.vue** - osoba - wykorzystywany w ParagraphStructure    
**NewsletterBlock.vue** - newsletter w formie bloku (obudowuje Newsletter form)  
**NewsletterFooter.vue** - newsletter w stopce bloku (obudowuje Newsletter form)  
**NodeAuthor.vue** - blok z nazwą autora treści, jego miniatura, opisem oraz odnośnikami do profili na twitterze i facebooku  
**NodeAuthorPublished.vue** - nazwa autora treści i data jej publikacji   
**NodeAuthorSimple.vue** - nazwa autora treści  
**NodeRelatedArtist.vue** - powiązany artysta (artist) występuje w dziele (work) oraz wydarzeniu (event)  
**NodeSocialLinks.vue** - linki socialne do udostępniania treści  
**NodeTags.vue** -   lista tagów  
**NodeVideo.vue** - główny komponent odpowiedzialny za obsługę wszystkich rodzajów wideo  
**RelatedNodeGallery.vue** - powiązana galeria - używane w typie zawartości artysta (artist)  
**RelatedNodeVideo.vue** - powiązane wideo - używane w typie zawartości artysta (artist)     
**Timeline.vue** - komponent odpowiedzialny za oś czasu w typie zawartości artysta (artist) 
  
## FORMS (src/components/forms)
### komponenty tworzące formularze
  
**Contact.vue** - formularz kontaktowy  
**Newsletter.vue** - formularz newslettera  
  
**AutosizingTextarea.vue** - kontrolka textarea automatycznie dopasowująca swoją wysokość do ilości wpisanego tekstu

## MIXINS (src/components/mixins)
### Części wspólne reużywane przez kilka komponentów

**highContrast.js** - mixin zawierający metody do sprawdzania aktualnego kontrastu  
**imageMetaMixin.js** - mixin zawierający metody do pobierania metatagów zdjęć typu media image  
**menuMixin.js** - mixin zawierający części wspólne komponentów odpowiedzialnych za menu   
**nodeMixin.js** - mixin zawierający części wspólne komponentów odpowiedzialnych za typy zawartości  
**paragraphContentMixin.js** - mixin zawierający części wspólne komponentów odpowiedzialnych za paragrafy będące składnikami głównej treści   
**withoutTranslations.js** - mixin zawierający części wspólne komponentów odpowiedzialnych za wyświetlanie podstron, które nie są pobierane z backendu a co za tym idzie nie mają własnej logiki przełączania języków   

## CONTENT TYPES (src/components/pages/content-types)
### Komponenty odpowiadające za wyświetlanie podstron dla różnych typów zawartości

**Article.vue** - typ zawartości artykuł (article)  
**Artist.vue** - typ zawartości artysta (artist)  
**Event.vue** - typ zawartości wydarzenie (event)  
**Gallery.vue** - typ zawartości galeria (gallery)  
**StaticPage.vue** - typ zawartości strona statyczna (static_page)  
**Venue.vue** - typ zawartości miejsce (venue)  
**Video.vue** - typ zawartości wideo (video)  
**Work.vue** - typ zawartości dzieło (work)  

## ERRORS (src/components/pages/errors)
### Komponenty odpowiadające za wyświetlanie stron błędów
**404.vue** - strona błedu nieznalezienia strony  
**500.vue** - strona błedu komunikacji z API  

## PARAGRAPHS (src/components/paragraphs)
### Komponenty odpowiadające za wyświetlanie paragrafów.  
  
#### Składniki głównej treści
**ParagraphTextFormatted.vue** - sformatowany tekst  
**ParagraphPicture.vue** - pojedyncze zdjęcie z opisem  
**ParagraphQuotation.vue** - cytat  
**ParagraphEmbeddedArticle.vue** - referencja - zajawka artykułu  
**ParagraphEmbeddedGallery.vue** - referencja - galeria w formie karuzeli lub pojedynczego zdjęcia; referencja  
**ParagraphEmbeddedVideo.vue** - referencja - odtwarzacz wideo  
**ParagraphStructure.vue** - struktura działu, używany w treściach typu static_page (strona statyczna)
#### Nagłówki
**ParagraphHeroHeader.vue** - nagłowek typu HeroHeader  
**ParagraphHeroHeaderArtist.vue** - nagłowek typu HeroHeaderArtist  
      

## SIDEBAR (src/components/sidebar)
### Komponenty odpowiadające za wyświetlanie treści powiązanych z paragrafami (będącymi składnikami główej treści).

**RelatedNodeArticle.vue** - artykuł  
**RelatedNodeArtist.vue** - twórca  
**RelatedNodeEvent.vue** - wydarzenie  
**RelatedNodeGallery.vue** - galeria  
**RelatedNodeVenue.vue** - miejsce  
**RelatedNodeVideo.vue** - wideo  
**RelatedNodeWork.vue** - dzieło  