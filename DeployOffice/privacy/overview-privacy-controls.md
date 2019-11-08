---
title: Pregled kontrola za zaštitu privatnosti za Office 365 ProPlus
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
audience: ITPro
ms.topic: conceptual
ms.service: o365-proplus-itpro
localization_priority: Priority
ms.collection:
- Ent_O365
- M365-modern-desktop
ms.custom:
- Ent_Office_ProPlus
- Ent_Office_Privacy
description: Administratorima sustava Office nudi pregled kontrola za zaštitu privatnosti za Office 365 ProPlus, uključujući dijagnostičke podatke i povezana iskustva.
hideEdit: true
ms.openlocfilehash: 784bbf08626e6dc8571c416a74511c9f5feeceec
ms.sourcegitcommit: acb22296532bbfdfcad4dc1e7162f812997fbdd1
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/08/2019
ms.locfileid: "38067328"
---
# <a name="overview-of-privacy-controls-for-office-365-proplus"></a>Pregled kontrola za zaštitu privatnosti za Office 365 ProPlus

Microsoft predano radi na tome da vam pruži informacije i kontrole potrebne da biste mogli odabrati načine prikupljanja i korištenja podataka o vama prilikom korištenja sustava Office 365 ProPlus.

Počevši od verzije 1904 sustava Office 365 ProPlus (objavljene u mjesečnom kanalu krajem 29. travnja 2019.), nudimo vam nove, ažurirane i poboljšane kontrole za zaštitu privatnosti u ovim područjima:
- ***Dijagnostički podaci*** o klijentskom softveru sustava Office koji se koristi na računalima sa sustavom Windows u vašoj tvrtki ili ustanovi, a koji se prikupljaju i šalju Microsoftu.
- ***Povezana iskustva*** koja koriste funkcije utemeljene na oblaku da bi vama i vašim korisnicima ponudila poboljšane značajke sustava Office.

U sklopu tih promjena pojavili su se novi i ažurirani elementi korisničkog sučelja (UI-ja) i postavke pravilnika.

> [!IMPORTANT]
> - Te se promjene odnose na Access, Excel, OneNote, Outlook, PowerPoint, Publisher i Word.
> - Te se promjene odnose i na sljedeće:
>   - Verziju 16.28 ili noviju verziju sljedećih aplikacija sustava Office za Mac: Excel, Outlook, OneNote, PowerPoint i Word.
>   - Verziju 1904 ili noviju verziju programa Project i Visio za računala koje se isporučuju s nekim pretplatničkim tarifama, kao što su Project Online Professional ili Visio Online Plan 2.
> - Ove kontrole za zaštitu privatnosti uključene su u verziju 1908. polugodišnjeg kanala (ciljano), koja je objavljena 10. rujna 2019. godine. Očekuje se da će biti dostupne u polugodišnjem kanalu u siječnju 2020. godine.
> - Te kontrole zaštite privatnosti dostupne su za verziju 2.30 i novije verzije programa Excel, OneNote, PowerPoint i Word te za verziju 1.17 i noviju verziju Preglednika za Visio za iOS.
> - Te kontrole zaštite privatnosti dostupne su za verziju 16.0.12226.10000 i novije verzije programa Excel, OneNote, PowerPoint i Word za Android, te za verziju 16.0.12228.20004 i novije verzije programa OneNote za Android.
> - Većina tih aplikacija Office za web mora početi koristiti novu kontrolu zaštite privatnosti za [neobvezna povezana iskustva](optional-connected-experiences.md).. To su sljedeće aplikacije: Excel za web, OneNote za web, PowerPoint za web, Visio za web i Word za web. Možete koristiti [Uslugu Office pravilnik o oblaku](../overview-office-cloud-policy-service.md) kako biste konfigurirali odgovarajuće [postavke pravilnika](manage-privacy-controls.md#policy-setting-for-optional-connected-experiences).
> - Te nove i poboljšane kontrole za zaštitu privatnosti proširit ćemo na dodatne klijente sustava Office, uključujući Teams i vlastite mobilne aplikacije. Dodatne informacije o tim promjenama objavit ćemo tijekom sljedećih mjeseci. Nastavit ćemo pažljivo slušati vaše povratne informacije i poboljšavati sve klijente i servise sustava Office 365.

## <a name="diagnostic-data-sent-from-office-365-proplus-to-microsoft"></a>Dijagnostički podaci koje Office 365 ProPlus šalje Microsoftu

Dijagnostički podaci koriste se da bi Office uvijek bio siguran i ažuran, kao i radi otkrivanja, dijagnosticiranja i otklanjanja problema te poboljšavanja proizvoda. Ti podaci ne sadrže korisnikovo ime ili adresu e-pošte, sadržaj korisnikovih datoteka ni informacije o aplikacijama koje nisu povezane sa sustavom Office.

To su dijagnostički podaci o klijentskom softveru sustava Office koji se koristi na računalima sa sustavom Windows u vašoj tvrtki ili ustanovi, a koji se prikupljaju i šalju Microsoftu.

Možete birati između tri razine dijagnostičkih podataka za klijentski softver sustava Office 365 ProPlus:

- **Obavezno**: minimalni podaci potrebni da bi Office bio siguran i ažuran te da bi na uređaju na kojem je instaliran funkcionirao na očekivan način.

- **Neobavezno**: dodatni podaci koji nam pomažu pri poboljšavanju proizvoda i pružaju poboljšane informacije koje nam pomažu pri otkrivanju, dijagnosticiranju i otklanjanju problema.

- **Nijedno**: ne prikupljaju se i ne šalju nikakvi dijagnostički podaci o klijentskom softveru sustava Office na korisnikovu uređaju. Ta mogućnost, međutim, znatno ograničava naše mogućnosti vezane uz otkrivanje, dijagnosticiranje i otklanjanje problema na koje vaši korisnici mogu naići koristeći Office.

Obavezni dijagnostički podaci mogu, primjerice, obuhvaćati informacije o verziji sustava Office instaliranog na uređaju ili informacije koje pokazuju da se aplikacije sustava Office ruše prilikom pokušaja otvaranja dokumenata. Neobavezni dijagnostički podaci mogu obuhvaćati informacije o vremenu potrebnom za spremanje dokumenta, što može ukazivati na problem specifičan za spremanje na vašem uređaju.

Ako odaberete slanje neobaveznih dijagnostičkih podataka, uz njih se prikupljaju i obavezni dijagnostički podaci.

Kao administrator za svoju tvrtku ili ustanovu moći ćete koristiti postavku pravilnika da biste odabrali koju ćete nam razinu dijagnostičkih podataka slati. Ako ne promijenite postavku, Microsoftu se šalju neobavezni dijagnostički podaci. Davanje neobaveznih dijagnostičkih podataka olakšava inženjerskom timu za Office u Microsoftu otkrivanje, dijagnosticiranje i ublažavanje problema s ciljem smanjenja njihovog utjecaja na vašu tvrtku ili ustanovu.

Vaši korisnici neće moći promijeniti razinu dijagnostičkih podataka za svoje uređaje ako su se prijavili u Office pomoću vjerodajnica svoje tvrtke ili ustanove, koje se ponekad nazivaju računom tvrtke ili obrazovne ustanove.

Ti dijagnostički podaci ne sadrže imena korisnika, njihove adrese e-pošte ni sadržaj njihovih datoteka sustava Office. Naš sustav stvara jedinstven ID koji povezuje s vašim dijagnostičkim podacima. Kada zaprimimo dijagnostičke podatke koji pokazuju da se jedna od naših aplikacija srušila 100 puta, taj jedinstveni ID omogućuje nam da utvrdimo je li se 100 puta srušila jednom korisniku ili se po jedanput srušila kod 100 različitih korisnika. Taj jedinstveni ID ne koristimo da bismo identificirali određenog korisnika.

Da biste vidjeli koji se dijagnostički podaci šalju Microsoftu, možete koristiti besplatni Preglednik dijagnostičkih podataka, koji možete preuzeti i instalirati iz trgovine Microsoft Store.

Dodatne informacije potražite u sljedećim člancima:

- [Obavezni dijagnostički podaci za Office](required-diagnostic-data.md)
- [Neobavezni dijagnostički podaci za Office](optional-diagnostic-data.md)
- [Korištenje postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Office 365 ProPlus](manage-privacy-controls.md)
- [Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office za Mac](mac-privacy-preferences.md)
- [Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office na iOS uređajima](ios-privacy-preferences.md)
- [Korištenje postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti na Android uređajima](android-privacy-controls.md)
- [Korištenje preglednika dijagnostičkih podataka sa sustavom Office](https://support.office.com/article/cf761ce9-d805-4c60-a339-4e07f3182855)

## <a name="connected-experiences-for-office-365-proplus"></a>Povezana iskustva za Office 365 ProPlus

Office 365 ProPlus sastoji se od klijentskih softverskih aplikacija i povezanih iskustava osmišljenih radi učinkovitijeg stvaranja, komunikacije i suradnje. Suradnja s drugim korisnicima na dokumentu pohranjenom na servisu OneDrive za tvrtke ili prevođenje sadržaja dokumenta programa Word na neki drugi jezik primjeri su povezanih iskustava.

Razumijemo da možda želite odabrati koje će vrste povezanih iskustava biti dostupne vašim korisnicima prilikom rada u aplikacijama sustava Office. Kao administrator svoje tvrtke ili ustanove na raspolaganju će vam biti postavka pravilnika koja omogućuje da odaberete želite li korisnicima ponuditi ove vrste povezanih iskustava:

- **Iskustva koja analiziraju vaš sadržaj**: to su iskustva koja koriste vaš sadržaj iz sustava Office da bi vam ponudila preporuke dizajna, prijedloge za uređivanje, uvide u podatke i slične značajke. Na primjer, PowerPoint Designer ili Redaktor u programu Word.

- **Iskustva koja preuzimaju internetski sadržaj**: to su iskustva koja omogućuju pretraživanje i preuzimanje internetskih sadržaja – uključujući predloške, slike, 3D modele, videozapise i referentne materijale – radi poboljšavanja vaših dokumenata. Na primjer, predlošci sustava Office ili alat za brz početak rada s programom PowerPoint.

Na primjer, možete odabrati da korisnicima ponudite povezana iskustva koja preuzimaju internetske sadržaje, ali ne i povezana iskustva koja analiziraju sadržaj. Ako ne konfigurirate te postavke pravilnika, sva će povezana iskustva biti dostupna vašim korisnicima.

Uz to, postoji i postavka pravilnika koja dopušta isključivanje svih tih povezanih sučelja, čime se isključuju i druga povezana sučelja, kao što su suautorstvo na dokumentima i mrežni prostor za pohranu datoteka. No čak i ako upotrijebite tu postavku pravilnika da biste isključili sva ta povezana iskustva, ostat će dostupne određene funkcije sustava Office, kao što su sinkroniziranje poštanskog sandučića u programu Outlook pomoću programa Teams ili Skype za tvrtke, kao i najvažniji servisi opisani u nastavku.

Ako odlučite korisnicima uskratiti određene vrste povezanih iskustava, naredbe tih povezanih iskustava na vrpci ili izborniku bit će zasivljene ili će korisnici dobiti poruku o pogrešci kada pokušaju koristiti ta povezana iskustva.

Vaši korisnici neće moći odabrati žele li uključiti ili isključiti ta povezana iskustva ako su se prijavili u Office pomoću vjerodajnica svoje tvrtke ili ustanove, koje se ponekad nazivaju računom tvrtke ili obrazovne ustanove.

Dodatne informacije potražite u sljedećim člancima:

- [Povezana iskustva u sustavu Office](connected-experiences.md)
- [Korištenje postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Office 365 ProPlus](manage-privacy-controls.md)
- [Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office za Mac](mac-privacy-preferences.md)
- [Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office na iOS uređajima](ios-privacy-preferences.md)
- [Korištenje postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti na Android uređajima](android-privacy-controls.md)

## <a name="optional-connected-experiences-for-office-365-proplus"></a>Neobavezna povezana iskustva za Office 365 ProPlus

Osim gore spomenutih povezanih iskustava obuhvaćenih sustavom Office 365 ProPlus, postoje i neobavezna povezana iskustva za koja korisnicima možete omogućiti da im pristupaju korištenjem računa tvrtke ili ustanove. Na primjer, značajke vezane uz LinkedIn u pomoćniku za životopis u programu Word ili značajka 3D karte u programu Excel, koja koristi Bing.

To su neobavezna povezana iskustva koja nisu obuhvaćena komercijalnim ugovorom vaše tvrtke ili ustanove s Microsoftom, već se reguliraju zasebnim uvjetima i odredbama. Neobavezna povezana iskustva koja Microsoft izravno nudi vašim korisnicima regulirana su [Microsoftovim ugovorom o pružanju usluga](https://www.microsoft.com/servicesagreement), a ne [Uvjetima korištenja internetskih servisa](https://www.microsoft.com/licensing/product-licensing/products).

Budući da su ta neobavezna povezana iskustva regulirana zasebnim uvjetima i odredbama, njima se upravlja odvojeno od gore spomenutih povezanih iskustava. Kao administrator za svoju tvrtku ili ustanovu moći ćete koristiti postavku pravilnika kojom odabirete želite li ta neobavezna povezana iskustva kao grupu staviti na raspolaganje korisnicima. Ako ne konfigurirate tu postavku pravilnika, ta su neobavezna povezana iskustva dostupna vašim korisnicima.

Čak i ako odlučite ta neobavezna povezana iskustva staviti na raspolaganje korisnicima, oni će imati mogućnost isključivanja neobaveznih povezanih iskustava kao grupe putem [dijaloškog okvira postavki zaštita privatnosti](https://support.office.com/article/3e7bc183-bf52-4fd0-8e6b-78978f7f121b). Korisnicima će se taj izbor pružati samo ako su se prijavili u Office s vjerodajnicama tvrtke ili ustanove (koje se ponekad nazivaju računom tvrtke ili obrazovne ustanove), a ne i ako su se prijavili s osobnom adresom e-pošte.

Dodatne informacije potražite u sljedećim člancima:

- [Pregled neobaveznih povezanih iskustava za Office](optional-connected-experiences.md)
- [Korištenje postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Office 365 ProPlus](manage-privacy-controls.md)
- [Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office za Mac](mac-privacy-preferences.md)
- [Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office na iOS uređajima](ios-privacy-preferences.md)
- [Korištenje postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti na Android uređajima](android-privacy-controls.md)

## <a name="required-service-data-for-connected-experiences"></a>Obavezni servisni podaci za povezana iskustva

Obavezni servisni podaci su podaci koji nam omogućuju primjenu povezanih iskustava utemeljenih na oblaku te pospješuju sigurnost i funkcioniranje tih iskustava na očekivan način. Obavezne servisne podatke čine tri vrste informacija.

- **Korisnički sadržaj**, tj. sadržaj koji stvarate koristeći Office, kao što je tekst upisan u dokument programa Word.
- **Funkcionalni podaci**, koji obuhvaćaju informacije koje su povezanom iskustvu potrebne za izvođenje njegovih zadataka, poput konfiguracijskih informacija o aplikaciji.
- **Servisni dijagnostički podaci**, tj. podaci nužni za zaštitu, ažurnost i funkcioniranje servisa na očekivan način. Budući da su ti podaci strogo vezani uz povezano iskustvo, odvojeni su od razina obaveznih ili neobaveznih dijagnostičkih podataka.

Da biste bolje razumjeli obavezne servisne podatke, u nastavku je naveden primjer scenarija upotrebe značajke PowerPoint Designer, povezanog iskustva koje možete koristiti prilikom stvaranja slajdova prezentacije. PowerPoint Designer potpomaže poboljšavanje slajdova automatskim generiranjem dizajnerskih ideja između kojih možete birati. Dok stavljate sadržaj na slajd, Designer u pozadini radi na podudaranju tog sadržaja s profesionalno dizajniranim izgledima.

Obavezni servisni podaci koji se šalju Microsoftu da bi vam se omogućilo to povezano iskustvo mogu obuhvaćati sljedeće:

- *Korisnički sadržaj*, poput teksta ili slika koje ste dodali na slajd.
- *Funkcionalne podatke*, poput slajda na kojem radite i njegovog izgleda.
- *Servisne dijagnostičke podatke*, poput događaja koji nam govore je li se dizajnerska ideja pravilno primijenila na vaš slajd i jesu li servisni pozivi pravilno funkcionirali.

Ako odlučite korisnicima uskratiti kategoriju povezanih iskustava koja obuhvaća PowerPoint Designer, ta će se značajka isključiti i neće nam slati ništa od tih obaveznih servisnih podataka.

Dodatne informacije potražite u članku [Obavezni servisni podaci za Office](required-service-data.md).

## <a name="essential-services-for-office-365-proplus"></a>Ključni servisi za Office 365 ProPlus

Postoji i skup servisa koji su ključni za funkcioniranje sustava Office 365 ProPlus te ih se ne može onemogućiti. Na primjer, servis za licenciranje, koji potvrđuje da imate ispravnu licencu za korištenje sustava Office 365 ProPlus. Obavezni servisni podaci o tim servisima prikupljaju se i šalju Microsoftu bez obzira na druge konfigurirane postavke pravilnika.

Dodatne informacije potražite u članku [Ključni servisi za Office](essential-services.md).

## <a name="related-topics"></a>Povezane teme
- [Zaštita privatnosti u tvrtki Microsoft](https://privacy.microsoft.com/)
- [Zaštita privatnosti u sustavu Windows](https://docs.microsoft.com/windows/privacy/)
