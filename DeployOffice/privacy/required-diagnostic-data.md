---
title: Obavezni dijagnostički podaci za Office
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
audience: ITPro
ms.topic: reference
ms.service: o365-proplus-itpro
localization_priority: Priority
ms.collection: Ent_O365
ms.custom:
- Ent_Office_ProPlus
- Ent_Office_Privacy
description: Administratorima sustava Office nudi informacije o obaveznim dijagnostičkim podacima u sustavu Office, a sadrži i popis događaja i podatkovnih polja.
hideEdit: true
ms.openlocfilehash: 6b099a73550f3a2c31147b9c7a5adb34dce6ff5f
ms.sourcegitcommit: 9f4afc7525d1d4cb6fbc0feef721a8eaffc09048
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/14/2021
ms.locfileid: "49867444"
---
# <a name="required-diagnostic-data-for-office"></a>Obavezni dijagnostički podaci za Office

> [!NOTE]
> Popis proizvoda sustava Office obuhvaćenih ovim informacijama o zaštiti privatnosti potražite u članku [kontrole zaštite privatnosti dostupne za proizvode sustava Office](products-versions-privacy-controls.md).

Dijagnostički podaci koriste se da bi Office uvijek bio siguran i ažuran, kao i radi otkrivanja, dijagnosticiranja i rješavanja problema te poboljšavanja proizvoda. Ti podaci ne obuhvaćaju korisnikovo ime i prezime ni adresu e-pošte, sadržaj korisnikovih datoteka ni informacije o aplikacijama koje nisu povezane sa sustavom Office.

Ovi dijagnostički podaci o klijentskom softveru sustava Office koji se pokreće na uređaju korisnika prikupljaju se i šalju Microsoftu. Neki su dijagnostički podaci obavezni, a neki nisu. Omogućujemo vam da odaberete hoćete li nam slati obavezne ili dijagnostičke podatke putem kontrola zaštite privatnosti, kao što su postavke pravila za tvrtke ili ustanove. Dijagnostičke podatke koji nam se šalju možete pogledati pomoću preglednika dijagnostičkih podataka.

***Obavezni dijagnostički podaci** _ minimalni su podaci potrebni da bi Office bio siguran i ažuran te da bi na uređaju na kojem je instaliran funkcionirao na očekivan način.

Obavezni dijagnostički podaci omogućuju da otkrijete probleme sa sustavom Office koji mogu biti povezani s konfiguracijom uređaja ili softvera. Na primjer, pomoću njih možete utvrditi ruši li se značajka sustava Office češće u određenoj verziji operacijskog sustava, zbog tek uvedenih značajki ili kada se onemoguće određene značajke sustava Office. Obavezni dijagnostički podaci omogućuju nam da otkrijemo, dijagnosticiramo i brže riješimo te probleme kako bi se smanjio utjecaj na korisnike ili tvrtke i ustanove.

Dodatne informacije o dijagnostičkim podacima potražite u ovim člancima:

- [Neobavezni dijagnostički podaci za Office](optional-diagnostic-data.md)
- [Korištenje preglednika dijagnostičkih podataka sa sustavom Office](https://support.microsoft.com/office/cf761ce9-d805-4c60-a339-4e07f3182855)

Ako ste administrator svoje organizacije,tvrtke ili ustanove možda će vas zanimati i sljedeći članci:

- [Pregled kontrola za zaštitu privatnosti za Microsoft 365 Apps za velike tvrtke](overview-privacy-controls.md)
- [Upotreba postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Microsoft 365 Apps za velike tvrtke](manage-privacy-controls.md)
- [Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office za Mac](mac-privacy-preferences.md)
- [Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office na iOS uređajima](ios-privacy-preferences.md)
- [Korištenje postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Office na Android uređajima](android-privacy-controls.md)

## <a name="categories-data-subtypes-events-and-data-fields-for-required-diagnostic-data"></a>Kategorije, podvrste podataka, događaji i podatkovna polja za obavezne dijagnostičke podatke

Obavezni dijagnostički podaci organizirani su u kategorije i podvrste podataka. U svakoj su podvrsti podataka događaji koji sadrže podatkovna polja specifična tom događaju.

U sljedećoj su tablici navedene kategorije za obavezne dijagnostičke podatke. Navedene su podvrste podataka u svakoj kategoriji i opis fokusa za tu podvrstu podataka. Postoje veze na odgovarajući odjeljak podvrsta podataka u kojem ćete pronaći sljedeće informacije:

- popis događaja u toj podvrsti podataka
- opis svakog događaja
- popis podatkovnih polja u svakom događaju
- opis svakog podatkovnog polja

| _ *Kategorija**       | **Podvrsta podataka**| **Opis**    |
| ---------- | ------------- | ---- |
| **Instalacija softvera i instalirani softver** | [Instalacija sustava Office i instalirani softver](#office-setup-and-inventory-subtype)   | Instalirani proizvod, njegova verzija i njegov status instalacije.  |
| | [Konfiguracija dodatka za Office](#office-add-in-configuration-subtype)  | Softverski dodaci i njihove postavke.     |
| | [Sigurnost](#security-subtype)  | Uvjeti za pogreške u dokumentima, značajkama i dodacima koji mogu ugroziti sigurnost, uključujući spremnost proizvoda za ažuriranje.  |
| **Korištenje proizvoda i usluga**    | [Uspjeh značajki aplikacije](#application-feature-success-subtype)   | Uspješno funkcioniranje aplikacije. Ograničeno na otvaranje i zatvaranje aplikacije i dokumenata, uređivanje datoteka i zajedničko korištenje dokumenata (suradnju). |
| | [Status i pokretanje aplikacije](#application-status-and-boot-subtype)    | Utvrđivanje je li došlo do određenih događaja povezanih sa značajkama, kao što je pokretanje ili zaustavljanje, te utvrđivanje je li značajka pokrenuta.   |
| | [Konfiguracija pristupačnosti za Office](#office-accessibility-configuration-subtype)  | Značajke pristupačnosti u sustavu Office       |
| | [Zaštita privatnosti](#privacy-subtype)| Postavke zaštite privatnosti u sustavu Office|
| **Performanse proizvoda i usluga**       | [Neočekivano zatvaranje aplikacije (rušenje)](#unexpected-application-exit-crash-subtype)  | Neočekivana zatvaranja aplikacija i stanje aplikacije kada se to dogodi.    |
|  | [Performanse značajki aplikacije ](#application-feature-performance-subtype)  | Loše vrijeme odziva ili performanse u situacijama kao što su pokretanje aplikacije ili otvaranje datoteke. |
|  | [Pogreška aktivnosti aplikacije](#application-activity-error-subtype)   | Pogreške u funkcioniranju značajke ili korisničkog okruženja.  |
| **Povezivost i konfiguracija uređaja** | [Povezivost i konfiguracija uređaja](#device-connectivity-and-configuration-subtype) | Stanje mrežne veze i postavke uređaja, kao što je memorija. |


> [!NOTE]
> - Kategorije su prikazane u pregledniku dijagnostičkih podataka, ali podvrste podataka nisu prikazane.
> - Podatkovno polje označeno kao *Zastarjelo* uklonjeno je ili će uskoro biti uklonjeno iz obaveznih dijagnostičkih podataka. Neka od tih podatkovnih polja su duplikati koji su nastali prilikom moderniziranja dijagnostičkih podataka i korišteni su da bi se spriječio prekid aktivnih izvješća dijagnostičkog nadzora.

## <a name="categories-and-data-fields-that-are-common-for-all-events"></a>Kategorije i podatkovna polja koja su zajednička svim događajima

Ovdje su i neke informacije koje se odnose na sve događaje, bez obzira na kategoriju ili podvrstu podataka. Te opće informacije, koje se ponekad nazivaju *podatkovni ugovori*, organizirane su po kategorijama. Svaka kategorija sadrži polja, a ta su polja metapodaci i svojstva pojedinog događaja. Te podatke možete pogledati pomoću preglednika dijagnostičkih podataka.

Kategorije podataka koji se prikupljaju o događajima mogu se podijeliti u dvije grupe:

  - [Informacije zajedničke svim događajima](#information-common-to-all-events)
  - [Informacije koje izričito podržavaju prikupljanje dijagnostičkih podataka](#information-that-specifically-supports-diagnostic-data-collection)

### <a name="information-common-to-all-events"></a>*Informacije zajedničke svim događajima*

U sljedeće kategorije prikupljaju se informacije zajedničke svim događajima.

#### <a name="app"></a>Aplikacija 

Informacije o aplikaciji. Sva su polja konstante za sve sesije određene verzije navedene aplikacije.

Ova kategorija sadrži sljedeća polja:

  - **Grana** ― grana iz koje dolazi navedena međuverzija. Omogućuje da utvrdimo iz koje vrste grane dolazi navedena međuverzija kako bismo ispravno usmjerili rješenja.
  - **InstallType** ― identifikator koji određuje način na koji je korisnik instalirao aplikaciju. Omogućuje da utvrdimo stvaraju li mehanizmi određene instalacije probleme kojih nema u mehanizmima drugih instalacija.
  - **Naziv** ― naziv aplikacije koja daje podatke. Omogućuje prepoznavanje aplikacije s kojom se pojavljuje problem kako bismo ga znali riješiti.
  - **Platforma** ― općenita klasifikacija platforme na kojoj je pokrenuta aplikacija. Omogućuje da odredimo na kojim se platformama problem pojavljuje kako bismo mogli ispravno odrediti njegov prioritet.
  - **Verzija** ― verzija aplikacije. Omogućuje prepoznavanje verzija proizvoda s kojima se pojavljuje problem kako bismo mogli ispravno odrediti njegov prioritet.

#### <a name="client"></a>Klijent 

Identifikator povezan s instancom sustava Office na uređaju. Konstanta za sve sesije svih aplikacija određene verzije instalacije za pakete s više aplikacija ili konstanta za sve sesije određene verzije aplikacije.

Ova kategorija sadrži sljedeća polja:

  - **ID** ― jedinstveni identifikator dodijeljen klijentu u trenutku instaliranja sustava Office. Omogućuje da utvrdimo zahvaćaju li problemi određeni skup instalacija i broj korisnika na koje utječu.

#### <a name="consent"></a>Pristanak

Informacije o pristanku korisnika za dijagnostičke podatke i povezana iskustva.

Ova kategorija sadrži sljedeća polja:

  - **ControllerConnectedServicesSourceLocation** – označava kako je napravljen korisnikov odabir za neobavezna povezana iskustva

  - **ControllerConnectedServicesState** – označava ima li korisnik pristup neobaveznim povezanim iskustvima

  - **ControllerConnectedServicesStateConsentTime** – označava kada je korisnik odabrao status za neobavezna povezana iskustva. Datum će se pojaviti ili kao datum koji ljudi mogu čitati ili kao strojno kodirani datum koji izgleda kao veliki broj.

  - **DiagnosticConsentConsentTime** – označava kada je korisnik dao pristanak za dijagnostičke podatke. Datum će se pojaviti ili kao datum koji ljudi mogu čitati ili kao strojno kodirani datum koji izgleda kao veliki broj.

  - **DiagnosticConsentLevel** – označava razinu pristanka za dijagnostičke podatke koju je korisnik dao

  - **DiagnosticConsentLevelSourceLocation** – označava način na koji je korisnik dao pristanak za dijagnostičke podatke

  - **DownloadContentSourceLocation** – označava kako je korisnik napravio odabir omogućivanja ili onemogućivanja povezanih iskustava koja preuzimaju internetski sadržaj

  - **DownloadContentState** – označava je li korisnik odlučio omogućiti ili onemogućiti povezana iskustva koja preuzimaju internetski sadržaj

  - **DownloadContentStateConsentTime** – označava kada je korisnik napravio odabir omogućivanja ili onemogućivanja povezanih iskustava koja preuzimaju internetski sadržaj. Datum će se pojaviti ili kao datum koji ljudi mogu čitati ili kao strojno kodirani datum koji izgleda kao veliki broj.

  - **ServiceConnectionState** – označava je li korisnik odlučio koristiti ili ne koristiti sva povezana iskustva

  - **ServiceConnectionStateConsentTime** – označava kada je korisnik odlučio želi li koristiti sva povezana iskustva. Datum će se pojaviti ili kao datum koji ljudi mogu čitati ili kao strojno kodirani datum koji izgleda kao veliki broj.

  - **ServiceConnectionStateSourceLocation** – označava način na koji je korisnik odlučio želi li koristiti sva povezana iskustva

  - **UserCategoryValue ―** određuje vrstu korisnika koji daje pristanak. Jedan MSAUser, AADUser ili LocalDeviceUser

  - **UserContentDependentSourceLocation** – označava kako je napravljen korisnikov odabir omogućivanja ili onemogućivanja povezanih iskustava koja analiziraju sadržaj

  - **UserContentDependentState** – označava je li korisnik odlučio omogućiti ili onemogućiti povezana iskustva koja analiziraju sadržaj

  - **UserContentDependentStateConsentTime** – označava kada je napravljen korisnikov odabir omogućivanja ili onemogućivanja povezanih iskustava koja analiziraju sadržaj. Datum će se pojaviti ili kao datum koji ljudi mogu čitati ili kao strojno kodirani datum koji izgleda kao veliki broj.

#### <a name="device"></a>Uređaj 

Informacije o operacijskom sustavu i međuverziji.

Ova kategorija sadrži sljedeća polja:

  - **OsBuild** – broj međuverzije operacijskog sustava instaliranog na uređaju. Omogućuje da utvrdimo utječu li problemi na pojedinačne servisne pakete ili verzije određenog operacijskog sustava drugačije od drugih kako bismo mogli odrediti prioritete problema.

  - **OsVersion** – glavna verzija operacijskog sustava instaliranog na uređaju. Omogućuje da utvrdimo utječu li problemi na određenu verziju operacijskog sustava više od drugih kako bismo mogli odrediti prioritete problema.

#### <a name="legacy"></a>Starije verzije 

Pruža ID aplikacije i verziju OS-a zbog kompatibilnosti s postojećim praksama prikupljanja za starije verzije.

Ova kategorija sadrži sljedeća polja:

  - **AppId** – vrijednost identifikatora koji označava aplikaciju koja šalje podatke. Omogućuje prepoznavanje aplikacije s kojom se pojavljuje problem kako bismo ga znali riješiti.

  - **OsEnv** – identifikator koji označava operacijski sustav na kojem je pokrenuta sesija. Omogućuje prepoznavanje operacijskog sustava na kojem se pojavljuje problem kako bismo mogli odrediti prioritete problema.

#### <a name="release"></a>Izdanje 

Podaci koji se odnose na kanal izdavanja. Sva su polja konstante za sve sesije svih aplikacija određene verzije instalacije. Određuje grupu uređaja u jednoj fazi ciklusa izdavanja proizvoda.

Ova kategorija sadrži sljedeća polja:

  - **Ciljna skupina** – označava segment određene grupe ciljnih skupina. Omogućuje da pratimo podskupove grupa ciljnih skupina za procjenu rasprostranjenosti i određivanja prioriteta problema.

  - **AudienceGroup** – označava krug iz kojeg potječu podaci. Omogućuje postupno uvođenje značajki i prepoznavanje potencijalnih problema prije nego što dođu do većine korisnika.

  - **Kanal** – kanal putem kojeg se izdaje proizvod. Omogućuje da odredimo utječe li problem na jedan od naših kanala za uvođenje drugačije od drugih.

  - **Međuverzija** – određuje međuverziju proizvoda. Omogućuje mehanizam za prikupljanje podataka u skupu brojeva međuverzija radi prepoznavanja problema povezanih s određenim izdanjem.

#### <a name="session"></a>Sesija 

Informacije o sesiji postupka. Sva su polja konstante za ovu sesiju.

Ova kategorija sadrži sljedeća polja:

  - **ABConfigs** – označava skup međuverzija koje se izvode u određenoj sesiji. Omogućuje prepoznavanje pojedinačnih međuverzija koje se izvode u sesiji kako bismo utvrdili je li međuverzija izvor problema koji utječe na korisnike.

  - **EcsETag** – pokazatelj iz sustava međuverzija koji predstavlja međuverzije poslane na računalo. Omogućuje prepoznavanje međuverzija koje utječu na određenu sesiju.

  - **Zastavice** – zastavice za praćenje bit-maske koje se odnose na cijelu sesiju, trenutno se uglavnom odnosi na uzorkovanje i mogućnosti dijagnostičkih podataka. Omogućuje kontrolu ponašanja određene sesije u odnosu prema dijagnostičkim podacima koje sesija generira.

  - **HostAppName** – označava naziv host aplikacije koja pokreće podaplikaciju. Aplikacije kao što je Office Mobile (Android) mogu pokrenuti podaplikacije Word, Excel i PowerPoint. Za takve pod-aplikacije glavna aplikacija je OfficeMobile

  - **Hostsessioid** – jedinstveno prepoznaje sesiju host aplikacije za podaplikaciju

  - **ID** – jedinstveno označava određenu sesiju podataka. Omogućuje utvrđivanje utjecaja problema procjenom broja zahvaćenih sesija te postoje li zajedničke značajke tih sesija.

  - **ImpressionId** – označava skup međuverzija koje se izvode u određenoj sesiji. Omogućuje prepoznavanje pojedinačnih međuverzija koje se izvode u sesiji kako bismo utvrdili je li međuverzija izvor problema koji utječe na korisnike.

  - **MeasuresEnabled** – zastavica koja označava jesu li podaci trenutne sesije uzorkovani. Omogućuje da utvrdimo kako statistički procijeniti podatke prikupljene iz određene sesije.

  - **SamplingClientIdValue** – ID klijenta kojim se utvrđuje je li dio uzorkovanja. Omogućuje da utvrdimo zašto je pojedinačna sesija uključena ili isključena iz uzorkovanja.
  
 - **SubAppName** – za aplikaciju Office za mobilne uređaje ovo polje predstavlja temeljnu aplikaciju koja se koristi za otvaranje dokumenta. Na primjer, ako otvorite dokument programa Word u aplikaciji Office, to polje će prijaviti vrijednost „Word“.

 - **VirtualizationType** – vrsta vizualizacije ako se Office izvodi u jednoj. Moguće vrijednosti su: 
    - 0 = Ništa
    - 1 = Windows Virtual Desktop
    - 2 = Microsoft Defender Application Guard
    - 3 = Windows Core OS

#### <a name="user"></a>Korisnik

Pruža informacije o klijentu za SKU-ove komercijalnog softvera.

Ova kategorija sadrži sljedeća polja:

  - **PrimaryIdentityHash** – identifikator u obliku pseudonima koji predstavlja trenutnog korisnika.

  - **PrimaryIdentitySpace** – vrsta identiteta sadržana u identifikatoru PrimaryIdentityHash. MASCID, OrgIdCID ili UserObjectId.

  - **TenantGroup** – vrsta klijenta kojem pripada pretplata. Omogućuje klasifikaciju problema i utvrđivanje je li problem rasprostranjen ili ograničen na skup korisnika.

  - **TenantId** – klijent s kojim je povezana pretplata korisnika. Omogućuje klasifikaciju problema i utvrđivanje je li problem rasprostranjen ili ograničen na skup korisnika ili određenog klijenta.

### <a name="information-that-specifically-supports-diagnostic-data-collection"></a>*Informacije koje izričito podržavaju prikupljanje dijagnostičkih podataka*

Informacije koje izričito podržavaju prikupljanje dijagnostičkih podataka prikupljaju se u sljedećim kategorijama.

#### <a name="activity"></a>Aktivnost

Informacije za shvaćanje uspješnosti samog događaja prikupljanja.

Ova kategorija sadrži sljedeća polja:

  - **AggMode** – govori sustavu kako prikupiti rezultate aktivnosti. Omogućuje nam smanjenje količine podataka prenesenih s korisnikova računala prikupljanjem rezultata aktivnosti u jedan događaj koji se šalje povremeno.

  - **Count** – broj izvršavanja aktivnosti ako je broj iz skupnog događaja. Omogućuje da odredimo koliko je često aktivnost uspjela na temelju načina prikupljanja aktivnosti.

  - **CV** – vrijednost koja određuje odnos između aktivnosti i segmenata aktivnosti. Omogućuje ponovno stvaranje odnosa između ugniježđenih aktivnosti.

  - **Trajanje** – vrijeme potrebno za izvršavanje aktivnosti. Omogućuje prepoznavanje problema s performansama koji negativno utječu na korisničko okruženje.

  - **Rezultat** – kôd koji je definirala aplikacija za prepoznavanje određenog rezultata. Omogućuje da utvrdimo specifične pojedinosti o određenoj pogrešci, primjerice kod pogreške koji može se koristiti za klasifikaciju i rješavanje problema.

  - **Result.Tag** – oznaka cijelog broja koja označava mjesto u kodu u kojem je generiran rezultat. Omogućuje jasno utvrđivanje mjesta u kodu na kojem je rezultat generiran što omogućuje klasifikaciju pogrešaka.

  - **Result.Type** – vrsta koda rezultata. Određuje vrstu poslanog koda rezultata kako bi se vrijednost ispravno tumačila.

  - **Uspjeh** – zastavica koja označava je li aktivnost uspjela. Omogućuje da utvrdimo uspijevaju li radnje koje korisnik izvršava u proizvodu. Time se omogućuje prepoznavanje problema koji utječu na korisnika.

#### <a name="application"></a>Aplikacija 

Informacije o instalaciji aplikacije iz koje se prikupljaju događaji.

Ova kategorija sadrži sljedeća polja:

  - **Arhitektura** – arhitektura aplikacije. Omogućuje nam da klasificiramo pogreške koje mogu biti specifične za arhitekturu aplikacije.

  - **Click2RunPackageVersion** – broj verzije paketa Klikom do cilja koji je instalirao aplikaciju. Omogućuje nam da identificiramo verziju programa za instalaciju koja je korištena za instalaciju sustava Office kako bismo mogli prepoznati probleme povezane s postavljanjem.

  - **DistributionChannel** – kanal u kojem je aplikacija implementirana. Omogućuje da podijelimo dolazne podatke kako bismo utvrdili utječu li problemi na ciljne skupine.

  - **InstallMethod** – određuje je li sustav nadograđen na trenutnu međuverziju sustava Office sa starije međuverzije, vraćen na nju ili je u pitanju nova instalacija.

  - **IsClickToRunInstall** – zastavica koja označava radi li se o instalaciji „klikom do cilja“. Omogućuje da prepoznamo probleme koji mogu biti specifični za mehanizam instalacije Klikom do cilja.

  - **IsDebug** – zastavica koja označava radi li se o međuverziji sustava Office za ispravljanje pogrešaka. Omogućuje nam da utvrdimo dolaze li problemi iz verzija za uklanjanje pogrešaka, koje se mogu ponašati drugačije.

  - **IsInstalledOnExternalStorage** – zastavica koja označava je li Office instaliran na vanjskom uređaju za pohranu. Omogućuje nam da odredimo mogu li se problemi povezati s mjestom za vanjsku pohranu.

  - **IsOEMInstalled** – zastavica koja označava je li Office instalirao proizvođač originalne opreme (OEM). Omogućuje nam da odredimo je li aplikaciju instalirao OEM, što nam može pomoći u klasificiranju i identificiranju problema.

  - **PreviousVersion** – verzija sustava Office koja je već instalirana na računalu. Omogućuje da se vratimo na prethodnu verziju ako postoji problem s trenutnom.

  - **ProcessFileName** – naziv datoteke aplikacije. Omogućuje prepoznavanje naziva izvršne datoteke koja generira podatke jer može postojati nekoliko različitih naziva datoteka procesa koji izvještavaju s istim nazivom aplikacije.

#### <a name="client"></a>Klijent

Informacije o klijentu sustava Office.

Ova kategorija sadrži sljedeća polja:

  - **FirstRunTime** – prvo pokretanje klijenta. Omogućuje da utvrdimo koliko je dugo sustav Office instaliran na klijentu.

#### <a name="device"></a>Uređaj

Informacije o konfiguraciji i mogućnostima uređaja.

Ova kategorija sadrži sljedeća polja:

  - **DigitizerInfo** – informacije o digitalizatoru koji računalo koristi. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **FormFactor** – utvrđuje format hardvera uređaja koji šalje podatke. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **FormFactorFamily** – utvrđuje format hardvera uređaja koji šalje podatke. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **HorizontalResolution** – vodoravna razlučivost zaslona uređaja. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **Id** – jedinstveni identifikator za uređaj. Omogućuje prepoznavanje distribucije problema u skupu uređaja.

  - **IsEDPPolicyEnabled** – zastavica koja označava je li na računalu omogućena napredna zaštita podataka. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **IsTerminalServer** – zastavica koja utvrđuje je li računalo terminalski poslužitelj. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **Proizvođač** – proizvođač uređaja. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **Model** – model uređaja. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **MotherboardUUIDHash** – hash oznaka jedinstvenog identifikatora za matičnu ploču. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **Naziv** – naziv uređaja. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.
  
  - **NetworkCost** – označava trošak ili vrstu mreže, primjerice s ograničenim prometom ili s ograničenom prometom s gornjom granicom.
  
  - **NetworkCountry** – pozivni broj države pošiljatelja na temelju nepročišćene IP adrese klijenta.

  - **NumProcPhysCores** – broj fizičkih jezgri na računalu. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **OsLocale** – regionalne postavke pokrenutog operacijskog sustava. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **ProcessorArchitecture** – arhitektura procesora. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **ProcessorCount** – broj procesora na računalu. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **ProcSpeedMHz** – brzina procesora. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **RamMB** – količina memorije uređaja. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **ScreenDepth** – omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **ScreenDPI** – vrijednost točaka po inču zaslona. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **SusClientId** – ID za Windows Update uređaja na kojem se Office pokreće.

  - **SystemVolumeFreeSpaceMB** – količina slobodnog prostora na sistemskom disku. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **SystemVolumeSizeMB** – veličina sistemskog diska na računalu. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **VerticalResolution** – okomita razlučivost zaslona uređaja. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **WindowErrorReportingMachineId** – jedinstveni identifikator računala kojeg daje izvješćivanje o pogreškama u sustavu Windows. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

  - **WindowSqmMachineId** – jedinstveni identifikator za računalo kojeg daje Windows SQM. Omogućuje da klasificiramo podatke na temelju središnjeg mehanizma uređaja.

#### <a name="event"></a>Događaj 

Informacije specifične za događaj, uključujući njegov jedinstveni identifikator u sesiji.

Ova kategorija sadrži sljedeća polja:

  - **Ugovor** – popis svih ugovora koje događaj implementira. Omogućuje da procijenimo koji su podaci dio pojedinačnog događaja kako bismo ih mogli učinkovito obraditi.

  - **CV** – vrijednost koja omogućuje prepoznavanje povezanih događaja. Koristi se za dijagnostiku kako bismo prepoznali uzorke povezanog ponašanja ili povezanih događaja.

  - **Zastavice** – informacije koje se koriste za promjenu načina na koji događaj odgovara. Koristi se za upravljanje načinom na koji se događaj tretira radi prijenosa podataka Microsoftu.

  - **Id** – jedinstveni identifikator za događaj. Omogućuje jedinstveno identificiranje primljenih događaja.

  - **Level** – označava vrstu događaja.

  - **Naziv** – naziv događaja. Omogućuje nam prepoznavanje događaja koji šalje klijent.

  - **Pravilo** – identifikator pravila koje je generiralo podatke ako ih je generiralo pravilo. Omogućuje prepoznavanje izvora dijela podataka tako da možemo provjeriti parametre tog događaja i njima upravljati

  - **RuleId** – identifikator pravila koje je generiralo podatke ako ih je generiralo pravilo. Omogućuje prepoznavanje izvora dijela podataka tako da možemo provjeriti parametre tog događaja i njima upravljati.

  - **RuleInterfaces** – sučelja koja određeno pravilo implementira. Omogućuje nam klasificiranje i uvoz podataka na temelju njihove strukture, što pojednostavljuje obradu podataka.

  - **RuleVersion** – identifikator pravila koje je generiralo podatke ako ih je generiralo pravilo. Omogućuje prepoznavanje izvora dijela podataka tako da možemo provjeriti parametre tog događaja i njima upravljati.

  - **SampleRate** – oznaka koliki postotak korisnika šalje ovaj dio podataka. Time se omogućuje statistička analiza podataka i veoma česte točke podataka ne zahtijevaju da to šalju svi korisnici.

  - **SchemaVersion** – verzija sheme koja se koristi za generiranje dijagnostičkih podataka. Obavezno za upravljanje podacima koje šalje klijent. Time se omogućuju promjene podataka koje šalje svaki klijent tijekom vremena.

  - **Slijed** – brojač koji navodi redoslijed kojim je događaj generiran na klijentu. Omogućuje numeriranje primljenih podataka kako bismo prepoznali korake koji su doveli do problema koji utječe na klijente.

  - **Izvor** – izvorni kanal upotrijebljen za prijenos podataka. Obavezno za praćenje svih kanala za prijenos radi ukupnog stanja i prepoznavanja problema s kanalom za prijenos. Time se omogućuje praćenje pojedinačnih kanala za prijenos kako bi bili usklađeni.

  - **Vrijeme** – vrijeme generiranja događaja na klijentu. Omogućuje sinkroniziranje i provjeru valjanosti redoslijeda događaja generiranih na klijentu i uspostavu parametara za mjerenje performansi za korisničke upute. 

#### <a name="host"></a>Glavno računalo

Informacije o aplikaciji koja hostira ugrađenu aplikaciju

Ova kategorija sadrži sljedeća polja:

  - **Id** – jedinstveni identifikator koji ugrađena aplikacija pripisuje glavnoj aplikaciji.

  - **SessionId** – globalno jedinstveni identifikator za sesiju glavnog računala.

  - **Version** – identifikator verzije primarne izvršne datoteke glavnog računala.

#### <a name="legacy"></a>Starije verzije

Informacije potrebne za kompatibilnost naslijeđenih sustava.

Ova kategorija sadrži sljedeća polja:

  - **OsBuild** – broj određene međuverzije operacijskog sustava. Omogućuje da utvrdimo iz koje verzije operacijskog sustava potječu dijagnostički podaci kako bismo odredili prioritete problema.

  - **OsBuildRevision** – broj revizije međuverzije operacijskog sustava. Omogućuje da utvrdimo iz koje verzije operacijskog sustava potječu dijagnostički podaci kako bismo odredili prioritete problema.

  - **OsMinorVersion** – sporedna verzija operacijskog sustava. Omogućuje da utvrdimo iz koje verzije operacijskog sustava potječu dijagnostički podaci kako bismo odredili prioritete problema.

  - **OsVersionString** – sjedinjeni niz koji predstavlja broj međuverzije operacijskog sustava. Omogućuje da utvrdimo iz koje verzije operacijskog sustava potječu dijagnostički podaci kako bismo odredili prioritete problema.

#### <a name="session"></a>Sesija

Informacije o sesiji postupka.

Ova kategorija sadrži sljedeća polja:

  - **ABConfigsDelta** – prati razliku između aktualnih podataka ABConfigs i prethodne vrijednosti. Omogućuje praćenje novih međuverzija na računalu da bismo lakše otkrili je li nova međuverzija odgovorna za problem.

  - **CollectibleClassification** – klase informacija koje sesija može prikupiti. Omogućuje filtriranje sesija na temelju podataka koje imaju.

  - **DisableTelemetry** – zastavica koja označava je li ključ DisableTelemetry postavljen. Omogućuje da utvrdimo je li sesija izvješćivala dijagnostičke podatke koji nisu EssentialServiceMetadata.

  - **SamplingClientIdValue** – vrijednost ključa za određivanje uzorkovanja. Omogućuje da utvrdimo zašto je sesija uzorkovana.

  - **SamplingDeviceIdValue** – vrijednost ključa za određivanje uzorkovanja. Omogućuje da utvrdimo zašto je sesija uzorkovana.

  - **SamplingKey** – ključ koji određuje je li sesija uzorkovana. Omogućuje da utvrdimo kako pojedine sesije odlučuju hoće li biti uzorkovane.

  - **SamplingMethod** – metoda koja se koristi za utvrđivanje pravila uzorkovanja. Omogućuje da utvrdimo koji podaci dolaze iz sesije.

  - **SamplingSessionKValue** – napredni metapodaci uzorkovanja. Koristi se za procjenu statističkog značenja primljenih podataka.

  - **SamplingSessionNValue** – napredni metapodaci uzorkovanja. Koristi se za procjenu statističkog značenja primljenih podataka.

  - **Slijed** – jedinstveni numerički identifikator za sesiju. Omogućuje određivanje redoslijeda sesija za analizu problema koji su se pojavili.

  - **Pokretanje** – vrijeme pokretanja sesije postupka. Omogućuje da utvrdimo kada je sesija pokrenuta.

  - **TelemetryPermissionLevel** – vrijednost koja označava razinu dijagnostičkih podataka koje je korisnik odabrao. Omogućuje da utvrdimo razinu dijagnostičkih podataka koja se može očekivati od sesije.

  - **TimeZoneBiasInMinutes** – razlika u minutama između UTC-a i lokalnog vremena. Omogućuje normalizaciju UTC-a na lokalno vrijeme.

## <a name="data-fields-that-are-common-for-onenote-events"></a>Polja podataka koja su uobičajena za događaje aplikacije OneNote

Sljedeća polja podataka uobičajena su za sve događaje za aplikaciju OneNote na sustavima Mac, iOS i Android.

> [!NOTE]
> Kada koristite preglednik dijagnostičkih podataka, događaji za aplikaciju OneNote na sustavima Mac, iOS i Android prikazivat će se kao da imaju naziv Aktivnost, Podaci o izvješću ili Neočekivano. Da biste pronašli stvarni naziv događaja, odaberite događaj, a zatim pogledajte polje EventName.

- **Activity_ActivityType** – označava vrstu događaja u ovoj aktivnosti. Aktivnost može biti normalna aktivnost ili aktivnost visoke vrijednosti.

- **Activity_AggMode** – govori sustavu kako prikupiti rezultate aktivnosti. Omogućuje nam smanjenje količine podataka prenesenih s korisnikova računala prikupljanjem rezultata aktivnosti u jedan događaj koji se šalje povremeno.

- **Activity_Count** – broj izvršavanja aktivnosti ako je broj iz skupnog događaja. Omogućuje da odredimo koliko je često aktivnost uspjela na temelju načina prikupljanja aktivnosti.

- **Activity_CV** – vrijednost koja određuje iznos između aktivnosti i segmenata aktivnosti. Omogućuje ponovno stvaranje odnosa između ugniježđenih aktivnosti.

- **Activity_DetachedDurationInMicroseconds** – vrijeme tijekom kojeg je aktivnost neaktivna te ne obavlja nikakav stvaran rad, no to se vrijeme i dalje uračunava u ukupno vrijeme aktivnosti.

- **Activity_DurationInMicroseconds** – vrijeme potrebno za izvršavanje aktivnosti. Omogućuje prepoznavanje problema s performansama koji negativno utječu na korisničko okruženje.

- **Activity_Expiration** – datum u brojčanom obliku označava kada će se ovaj događaj prestati slati putem korisnika

- **Activity_FailCount** – koliko je puta ova aktivnost bila neuspješna

- **Activity_Name** – kratki naziv događaja. Omogućuje nam prepoznavanje događaja koji šalje klijent.

- **Activity_Namespace** – prostor naziva događaja. Omogućuje nam grupiranje događaja u grupe.

- **Activity_Reason** – niz koji označava razlog koji uzrokuje završavanje aktivnosti s određenim rezultatom.

- **Activity_Result** – zastavica koja označava je li aktivnost uspjela, nije uspjela ili neočekivano nije uspjela. Omogućuje da utvrdimo uspijevaju li radnje koje korisnik izvršava u proizvodu. Time se omogućuje prepoznavanje problema koji utječu na korisnika.

- **Activity_State** – zastavica označava je li događaj početak aktivnosti korisnika ili završetak aktivnosti korisnika.

- **Activity_SucceedCount** – koliko je puta ova aktivnost bila uspješna.

- **ErrorCode** – označava šifru pogreške ako je dostupna.

- **ErrorCode2** – označava drugu šifru pogreške ako je dostupna.

- **ErrorCode3** – označava treću šifru pogreške ako je dostupna.

- **ErrorTag** – označava oznaku povezanu s kodom pogreške ako je dostupna.

- **ErrorType** – označava vrstu pogreške ako je dostupna.

- **EventName** – jedinstven naziv događaja aplikacije OneNote. Događaji u aplikaciji OneNote koriste ovo prilagođeno polje kako bi odredili jedinstven naziv zbog inženjerskog ograničenja u prošlosti.

- **ExpFeatures** – označava je li korisnik uključio prekidač za pokusnu značajku u aplikaciji OneNote ili nije.

- **ExpirationDate** – datum u brojčanom obliku označava kada će se ovaj događaj prestati slati putem korisnika

- **IsConsumer** – označava je li korisnik potrošač ili nije

- **IsEdu** – označava je li korisnik ujedno korisnik u obrazovnoj ustanovi ili nije

- **IsIW** – označava je li korisnik ujedno korisnik iz velike tvrtke ili nije

- **IsMsftInternal** – označava je li korisnik Microsoftov zaposlenik ili nije

- **IsPremiumUser** – označava ima li korisnik licencu za Premium ili nema

- **Namespace** – prostor naziva događaja. Omogućuje nam grupiranje događaja u grupe.

- **Release_AppStore** – zastavica označava dolazi li međuverzija iz trgovine aplikacija ili ne.

- **Release_Audience** – označava segment određene grupe ciljnih skupina. Omogućuje da pratimo podskupove grupa ciljnih skupina za procjenu rasprostranjenosti i određivanja prioriteta problema.

- **Release_AudienceGroup** – označava krug iz kojeg potječu podaci. Omogućuje postupno uvođenje značajki i prepoznavanje potencijalnih problema prije nego što dođu do većine korisnika.

- **Release_Channel** – kanal putem kojeg se izdaje proizvod. Omogućuje da odredimo utječe li problem na jedan od naših kanala za uvođenje drugačije od drugih.

- **RunningMode** – označava kako je aplikacija pokrenuta bilo putem korisnika ili procesa sustava.

- **SchemaVersion** – označava trenutnu verziju telemetrijske sheme u telemetrijskom cjevovodu aplikacije OneNote.

- **Session_EcsETag** – pokazatelj iz sustava međuverzija koji predstavlja međuverzije poslane na računalo. Omogućuje prepoznavanje međuverzija koje utječu na određenu sesiju.

- **Session_ImpressionId** – označava skup međuverzija koje se izvode u određenoj sesiji. Omogućuje prepoznavanje pojedinačnih međuverzija koje se izvode u sesiji kako bismo utvrdili je li međuverzija izvor problema koji utječe na korisnike.

- **SessionCorrelationId** – globalno jedinstveni identifikator za sesiju glavnog računala.

- **SH_ErrorCode** – označava šifru pogreške ako je dostupna tijekom neuspješne aktivnosti.

- **Tag** – oznaka cijelog broja koja označava mjesto u kodu u kojem je generiran telemetrijski događaj.

- **UserInfo_IdType** – niz označava vrstu korisnikova računa

- **UserInfo_OMSTenantId** – klijent s kojim je povezana pretplata korisnika. Omogućuje klasifikaciju problema i utvrđivanje je li problem rasprostranjen ili ograničen na skup korisnika ili određenog klijenta.

- **UserInfo_OtherId** – popis identifikatora u obliku pseudonima koji nisu primarni predstavlja korisnikove račune.

- **UserInfo_OtherIdType** – popis vrsta računa koji nisu primarni.

## <a name="data-fields-that-are-common-for-outlook-mobile-events"></a>Polja podataka koja su uobičajena za događaje aplikacije Outlook

Outlook Mobile prikuplja uobičajena polja za svaki naš događaj da bismo mogli osigurati da je aplikacija ažurna, sigurna i funkcionalna kao što se očekuje. 

Sljedeća polja podataka uobičajena su za sve događaje za aplikaciju Outlook na sustavima iOS i Android.

- **aad_tenant_id** – ID klijenta korisnika ako je dostupan

- **account_cid** – identifikator u obliku pseudonima koji predstavlja trenutačnog korisnika

- **account_domain** – naziv domene računa

- **account_puid** – globalno jedinstveni identifikator korisnika za Microsoftov potrošački račun

- **account_type** – prati vrstu računa kao što je Office 365, Google Cloud Cache, Outlook.com itd.

- **action** – naziv radnje događaja (kao što je arhiva, brisanje itd.) tako da možemo otkriti poteškoće sa specifičnim radnjama koje su poduzete

- **ad_id** – jedinstveni identifikator oglašavanja

- **app_version** – trenutačna instalirana verzija aplikacije koja nam pomaže otkriti probleme koji utječu na određenu verziju aplikacije

- **AppInfo.ETag** – jedinstven identifikator za upravljanje izdanjima naših značajki kako bismo lakše prepoznali probleme koji utječu na određene značajke koje se objavljuju

- **AppInfo.Language** – trenutačna jezična postavka uređaja koja nam omogućuje otkrivanje problema koji utječu na određene jezike

- **AppInfo.Version** – trenutačna verzija instalirane verzije s pomoću koje otkrivamo probleme koji utječu na određene verzije aplikacija

- **ci** – identifikator u obliku pseudonima koji predstavlja identifikatora specifičnog za uređaj

- **cid_type** – označava koja je vrsta računa, npr. poslovni račun ili račun za Outlook.com.

- **cloud** – mjesto gdje se poštanski sandučić nalazi za račun na ovom uređaju kako bi se lakše prepoznali problemi specifični za oblak specifičnog poštanskog sandučića, poput sustava Office 365 ili GCC.

- **customer_type** – označava vrstu korisnika (potrošač, komercijalni korisnik, treća strane itd.) kako bismo lakše prepoznali probleme koji utječu na određene vrste korisnika

- **device_category** – označava vrstu uređaja (telefon, tablet itd.) kako bismo lakše prepoznali specifične probleme kategorije uređaja

- **DeviceInfo.Id** – jedinstven identifikator uređaja s pomoću kojeg lakše otkrivamo specifične probleme uređaja

- **DeviceInfo.Make** – marka uređaja (tj. Apple, Samsung itd.) kako bismo lakše prepoznali probleme specifične za marku

- **DeviceInfo.Model** – model uređaja (npr. iPhone 6s) kako bismo lakše prepoznali probleme specifične za model

- **DeviceInfo.NetworkType** – trenutačna mreža uređaja koja se upotrebljava (Wi-Fi, mobilna itd.) kako bismo lakše prepoznali probleme specifične za mrežu

- **DeviceInfo.OsBuild** – trenutačna međuverzija OS-a uređaja kako bismo lakše prepoznali probleme koji utječu na određene međuverzije OS-a

- **DeviceInfo.OsName** – naziv OS-a (npr. iOS) kako bismo lakše prepoznali probleme koji utječu na određene platforme

- **DeviceInfo.OsVersion** – trenutačna verzija OS-a uređaja kako bismo lakše prepoznali probleme koji utječu na određene verzije OS-a

- **DeviceInfo.SDKUid** – jedinstveni identifikator uređaja (sličan identifikatoru DeviceInfo.Id)

- **EventInfo.InitId** – ID koji se upotrebljava u okviru postavljanja rasporeda događaja preko našeg kanala za telemetriju kako bismo lakše prepoznali uzrok problema u kanalu

- **EventInfo.SdkVersion** – SDK verzija koju upotrebljavamo za slanje naše telemetrije kako bismo lakše prepoznali uzrok problema u kanalu

- **EventInfo.Sequence** – slijed je za raspored događaja kroz naš kanal za telemetriju kako bismo lakše prepoznali uzrok problema u kanalu

- **EventInfo.Source** – govori nam koji je dio kôda poslao događaj kako bi nam pomogao prepoznati uzrok problema

- **EventInfo.Time** – vrijeme i datum emitiranja događaja s uređaja tako da naši sustavi mogu uspješno upravljati događajima koji stižu

- **eventpriority** – prioritet telemetrijskog događaja koji se odnosi na druge događaje tako da naši sustavi mogu uspješno upravljati događajima koji stižu

- **first_launch_date** – prvi put kada je aplikacija pokrenuta da bismo lakše shvatili kada je problem nastao

- **hashed_email** – identifikator u obliku pseudonima koji predstavlja poruku e-pošte trenutačnog korisnika

- **is_first_session** – prati ako je ovo prva sesija aplikacija radi rješavanja pogrešaka

- **origin** – izvor radnje. Na primjer, označavanje poruke pročitanom može doći s popisa poruka ili iz obavijesti o novoj pošti, a to nam pomaže otkriti probleme na temelju izvora radnje

- **PipelineInfo.AccountId** – identifikator u obliku pseudonima koji predstavlja trenutačnog korisnika

- **PipelineInfo.ClientCountry** – trenutačna zemlja uređaja kako bi se prepoznali specifični problemi i nedostupnost u vezi zemlje ili regije

- **PipelineInfo.ClientIp** – IP adresa na kojoj je uređaj spojen radi rješavanja problema s povezivanjem

- **PipelineInfo.IngestionTime** – vremenska oznaka telemetrijskog prihvaćanja za ovaj događaj

- **Session.Id** – jedinstven identifikator za sesiju aplikacije za lakše otkrivanje problema u vezi sa sesijom

- **Session.ImpressionId** – jedinstven identifikator za upravljanje izdanjima naših značajki da bi se značajke uspješno objavile svim korisnicima i u svim uređajima

- **ui_mode** – je korisnik u svijetlom ili tamnom načinu rada, pomaže nam razvrstati pogreške u korisničkom sučelju

- **UserInfo.Language** – korisnikov jezik koji pomaže rješavati pogreške u vezi s tekstom prijevoda

- **UserInfo.TimeZone** – vremenska zona korisnika koja pomaže rješavati pogreške u vezi s kalendarom


Osim toga, sljedeća su polja podataka uobičajena za sve događaje za aplikaciju Outlook za iOS.

- **DeviceInfo.NetworkProvider** – davatelj mreže uređaja (npr. Verizon)

- **gcc_restrictions_enabled** – upućuje na to jesu li na aplikaciju primijenjena ograničenja GCC-a tako da možemo osigurati da korisnici GCC-a sigurno upotrebljavaju našu aplikaciju
 
- **multi_window_mode** – govori nam upotrebljava li korisnik na iPadu više prozora da bi nam pomogao otkriti probleme u vezi s upotrebom više prozora.

- **office_session_id** – jedinstveni identifikator koji prati sesiju za spojene usluge sustava Office kako bi se lakše prepoznali problemi specifični za integraciju usluge sustava Office u aplikaciju Outlook, poput aplikacije Word

- **state** – je li aplikacija bila aktivna kada je ovaj događaj poslan kako bi se lakše prepoznali problemi specifični za aktivna i neaktivna stanja aplikacija


Osim toga, sljedeća su polja podataka uobičajena za sve događaje za aplikaciju Outlook za Android.

- **aad_id** – identifikator u obliku pseudonima za Azure Active Directory

- **DeviceInfo.NetworkCost** – pokazatelj trenutačnog mrežnog troška uređaja koji odražava status mreže Wi-Fi/mobilne mreže/roaminga kako bi se lakše prepoznali problemi specifični za mrežu uređaja

- **is_app_in_duo_split_view_mode** – javit će nam da je aplikacija bila u načinu dijeljenja zaslona na uređaju Duo.  To je svojstvo podešeno samo za uređaje Duo (samo Android).

- **is_dex_mode_enabled** – je li omogućen Samsungov način rada DeX kako bi se lakše prepoznali problemi specifični za način rada DeX kod Samsungovih uređaja

- **is_sliding_drawer_enabled** – je li sučelje klizne ladice omogućeno kako bi se lakše prepoznali problemi koje uzroku naše sučelje klizne ladice

- **orientation** – fizičko usmjerenje zaslona (okomito/vodoravno) kako bi se lakše prepoznali specifični problemi u vezi s usmjerenjem zaslona

- **os_arch** – arhitektura operacijskog sustava za uređaj kako bi se lakše prepoznali problemi specifični za operacijske sustave uređaja

- **process_bitness** – broj bitova postupka (32 ili 64 bitova) za aplikaciju kako bi se lakše prepoznali problemi specifični za broj bitova uređaja

- **webview_kernel_version**: verzija jezgre sustava Chromium web-prikaza na uređaju koja nam pomaže prepoznati probleme s kompatibilnošću povezane s verzijom web-prikaza.

- **webview_package_name**: naziv paketa web-prikaza na uređaju koji nam pomaže prepoznati probleme s kompatibilnošću povezane s verzijom web-prikaza.

- **webview_package_version**: verzija paketa web-prikaza na uređaju koji nam pomaže prepoznati probleme s kompatibilnošću povezane s verzijom web-prikaza.


## <a name="software-setup-and-inventory-data-events"></a>Događaji koji se odnose na instalaciju softvera i podatke o instaliranom softveru

Ovo su podvrste podataka u toj kategoriji:
- [Instalacija sustava Office i instalirani softver](#office-setup-and-inventory-subtype)
- [Konfiguracija dodatka za Office](#office-add-in-configuration-subtype)
- [Sigurnost](#security-subtype)  

### <a name="office-setup-and-inventory-subtype"></a>*Instalacija sustava Office i podvrsta instaliranog softvera*

Instalirani proizvod, njegova verzija i njegov status instalacije.

#### <a name="addssoaccount"></a>add.sso.account

Time će se Microsoft izvijestiti o uspjehu ili neuspjehu korisnika s dodavanjem računa putem jedinstvene prijave (SSO).

Prikupljaju se sljedeća polja: 

- **account_type** – vrsta računa dodanog upotrebom SSO-a.

- **action_origin** – odakle je taj događaj generiran. (for example, values: sso_drawer, sso_add_account, sso_add_account_prompt, sso_settings, sso_oobe).

- **provider** – identifikator pružatelja softverskog paketa za SSO.

- **state** – trenutačno stanje računa (npr. vrijednost: NIJE USPJELO, NA ČEKANJU, Dodano itd.)


#### <a name="installreferral"></a>install.referral

Ovaj se događaj aktivira pri početnoj instalaciji aplikacije i bilježi odakle je korisnik upućen (ako je dostupan).

Prikupljaju se sljedeća polja:

- **install_referrer** – proizvod ili iskustvo s kojeg je korisnik upućen

 
#### <a name="officeclicktorunupdatestatus"></a>Office.ClickToRun.UpdateStatus

Odnosi se na sve aplikacije win32. Omogućuje nam da utvrdimo status postupka ažuriranja paketa sustava Office (uspjeh ili neuspjeh s detaljima o pogrešci)

Prikupljaju se sljedeća polja:

- **međuverzija** – trenutno instalirana verzija sustava Office

- **kanal** – kanal putem kojeg je Office distribuiran

- **errorCode** – kod pogreške koji označava pogrešku

- **errorMessage** – dodatne informacije o pogrešci

- **status** – trenutni status ažuriranja

- **targetBuild** – verzija na koju se ažurira Office

#### <a name="officecompliancefileformatballotdisplayedonfirstboot"></a>Office.Compliance.FileFormatBallotDisplayedOnFirstBoot

Označava je li dijaloški okvir izbora oblika datoteke sustava Office prikazan korisniku tijekom prvog/drugog pokretanja programa Word, Excel ili PowerPoint na sustavu Win32.  Prati prikazuje li se dijaloški okvir FileFormat Ballot – događaj se šalje pri prvom / drugom pokretanju programa Word, Excel ili PPT Win32.

Prikupljaju se sljedeća polja.

- **CountryRegion** – korisnikove postavke za državu i regiju u sustavu Windows

- **FileFormatBallotBoxAppIDBootedOnce** – u kojoj je aplikaciji (Word, Excel, PPT) obrađena logika prikazivanja oblika formata Ballot.

- **FileFormatBallotBoxDisplayedOnFirstBoot** – koji je rezultat prikazivanja za oblik formata Ballot (prikazan/nije prikazan kao neočekivano / nije prikazan zbog licence / nije prikazan zbog lokacije).

#### <a name="officecompliancefileformatballotoption"></a>Office.Compliance.FileFormatBallotOption

Prati prikazuje li se dijaloški okvir FileFormat Ballot – događaj se šalje pri prvom / drugom pokretanju programa Word, Excel ili PPT Win32.  Označava prikazuje li se dijaloški okvir izbora oblike datoteke sustava Office tijekom prvog ili drugog pokretanja programa Word, Excel ili PowerPoint na sustavu Win32.

Prikupljaju se sljedeća polja:

- **FileFormatBallotSelectedOption** – prepoznaje mogućnost oblika formata (OOXML/ODF) koji je korisnik odabrao putem dijaloškog okvira oblika formata Ballot.


#### <a name="officecorrelationmetadatautccorrelationmetadata"></a>Office.CorrelationMetadata.UTCCorrelationMetadata

Prikuplja metapodatke sustava Office putem UTC-a radi usporedbe s odgovarajućim podacima prikupljenim kroz kanal za telemetriju radi provjere ispravnosti i potpunosti podataka.

Prikupljaju se sljedeća polja:

- **abConfigs** – popis ID-ova značajki radi utvrđivanja koje su značajke na klijentu omogućene ili prazna vrijednost kada se ti podaci ne prikupljaju.

- **abFlights** – „NoNL:NoFlights“ kada izdvojene međuverzije nisu postavljene. U suprotnom „holdoutinfo = Nepoznato“.

- **AppSessionGuid** – identifikator određene sesije aplikacije koja počinje od vremena postupka stvaranja i traje do završetka postupka. Oblikovan je kao standardni 128-bitni GUID, ali se sastoji od četiri dijela. Ta su četiri dijela redom: (1) 32-bitni ID procesa (2) 16-bitni ID sesije (3) 16-bitni ID pokretanja (4) 64-bitno UTC vrijeme stvaranja procesa, izraženo u koracima od 100 ns

- **appVersionBuild** – broj međuverzije aplikacije.

- **appVersionMajor** – broj glavne verzije aplikacije.

- **appVersionMinor** – broj sporedne verzije aplikacije.

- **appVersionRevision** – broj verzije revizije aplikacije.

- **audienceGroup** – naziv grupe ciljne skupine za izdanje

- **audienceId** – naziv ciljne skupine za izdanje

- **kanal** – kanal putem kojeg je Office distribuiran

- **deviceClass** – format hardvera uređaja iz operacijskog sustava

- **ecsETag** – identifikator eksperimenta za postupak

- **impressionId** – guid koji označava trenutni skup značajki.

- **languageTag** – oznaka jezika IETF-a trenutnog korisničkog sučelja sustava Office

- **officeUserID** – nasumično generirani guid za ovu instalaciju sustava Office

- **osArchitecture** – arhitektura operacijskog sustava

- **osEnvironment** – cijeli broj koji označava operacijski sustav (Windows, Android, iOS, Mac itd).

- **osVersionString** – verzija operacijskog sustava

- **sessionID** – nasumično generirani guid za prepoznavanje sesije aplikacije

- **UTCReplace_AppSessionGuid** – konstantna Booleova vrijednost. Uvijek istinito.

#### <a name="officeonenoteandroidapponenotelaunchednonactivated"></a>Office.OneNote.Android.App.OneNoteLaunchedNonActivated

*[Ovaj je događaj prethodno imenovan OneNote.App.OneNoteLaunchedNonActivated.]*

Bilježi podatke o stanju aktivacije aplikacije.  Podaci se prate da bi se osiguralo identificiranje porasta u problemima sa aktivacijom. Također analiziramo podatke kako bismo pronašli područja poboljšanja.

Prikupljaju se sljedeća polja: 

- **INSTALL_LOCATION** – upućuje na to je li aplikacija unaprijed instalirana ili je preuzeta iz trgovine

#### <a name="officeonenoteandroidresetstatus"></a>Office.OneNote.Android.ResetStatus

*[This event was previously named OneNote.ResetStatus.]*

Signal koji se koristi za bilježenje problema koji se pojave kada korisnik pokušava ponovno postaviti aplikaciju.  Telemetrija se koristi za nadgledanje, otkrivanje i ispravljanje problema uzrokovanih tijekom ponovnog postavljanja. 

Prikupljaju se sljedeća polja: 

- **Poslovni subjekti** – označava vrste ako se računi koriste za prijavu u aplikaciju

- **Generic String Type** – vraća se ako su kompletno ponovno postavljene notes_light_data

- **LaunchPoint** – točka u kojoj se pokreće ponovno postavljanje. Moguće vrijednosti: gumb za odjavljivanje, pogreška prilikom odjave, pokretanje servisa Intune

- **Pass** – označava je li ponovno pokretanje bilo uspješno

#### <a name="officeonenoteandroidsigninsignincompleted"></a>Office.OneNote.Android.SignIn.SignInCompleted

*[Ovaj je događaj prethodno imenovan OneNote.SignIn.SignInCompleted.]*

Ključni signal kojim se osigurava uspješna prijava ili ne. Telemetrija se prikuplja za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge.

Prikupljaju se sljedeća polja: 

- **CompletionState** – završno stanje prijave – uspješno ili neuspješno. I slučajevi neuspjeha

- **EntryPoint** – označava odakle je pokrenuta prijava

- **Hresult** – kôd pogreške

- **Provider Package ID** – u slučaju automatske prijave

- **Result** – uspjela, nije uspjela, nepoznato, otkazana

- **ServerType** – vraća vrstu poslužitelja koji nudi uslugu 

- **SignInMode** – prijava ili registracija ili ubrzana automatska prijava ili registracija

#### <a name="officeonenoteandroidsigninsigninstarted"></a>Office.OneNote.Android.SignIn.SignInStarted

*[Ovaj je događaj prethodno imenovan OneNote.SignIn.SignInStarted.]*

Signal koji se koristi za označavanje bilo kakvih problema tijekom korištenja trake s porukama.  Telemetrija se koristi za nadgledanje, otkrivanje i ispravljanje problema nastalih tijekom interakcije s trakom s porukama

Prikupljaju se sljedeća polja: 

- **EntryPoint** – označava odakle je pokrenuta prijava

- **Result** – rezultat tijeka prijave

- **ServerType** – vraća vrstu poslužitelja koji nudi uslugu 

- **SignInMode** – prijava ili registracija ili ubrzana automatska prijava ili registracija


#### <a name="officeonenotefirstrunfirstrun"></a>Office.OneNote.FirstRun.FirstRun

Ključni signal korišten za osiguravanje da novi korisnici uspješno mogu prvi put pokrenuti aplikaciju OneNote.  Telemetrija se prikuplja za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. Ako korisnici ne mogu prvi put pokrenuti aplikaciju, time bi se izazvao incident visoke ozbiljnosti.

- **AfterOneDriveFrozenAccountError** – označava pogrešku aplikacije OneDrive kada je račun zamrznut.

- **Attempt** – broj puta koji se iskustvo prvog pokretanja treba ponovno pokušati.

- **IsDefaultNotebookCreated** – označava je li aplikacija OneNote stvorila zadanu bilježnicu korisnika ili nije.

- **IsDelayedSignIn** – označava provodi li se prvo pokretanje u odgođenom načinu prijave u kojem se korisnik ne treba prijaviti.

- **IsMSA** – označava je li račun Microsoftov račun ili nije.

#### <a name="officeonenotefirstrunfirstrunformsa"></a>Office.OneNote.FirstRun.FirstRunForMSA

Ključni signal korišten za osiguravanje da novi privatni korisnici (Microsoftov račun) uspješno mogu prvi put koristiti aplikaciju OneNote.

Telemetrija korištena za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. Ako korisnici ne mogu prvi put pokrenuti aplikaciju, time bi se izazvao incident visoke ozbiljnosti.

Prikupljaju se sljedeća polja:

- **Attempt** – broj puta koji se iskustvo prvog pokretanja treba ponovno pokušati.

- **Error A** – objekt pogreške aplikacije OneNote označava pogrešku tijekom prvog pokretanja ako ona postoji.

- **FAllowAddingGuide** – označava hoće li OneNote dopustiti stvaranje bilježnice vodiča ili ne.

- **FrozenOneDriveAccount** – označava je li račun aplikacije OneNote zamrznut ili nije.

- **IsDefaultNotebookCreated** – označava je li aplikacija OneNote stvorila zadanu bilježnicu korisnika ili nije.

- **NoInternetConnection** – označava slučaj kada uređaj nema internetsku vezu.

- **ProvisioningFailure** – objekt pogreške aplikacije OneNote koji označava pogrešku dodjele resursa ako ona postoji.

- **ProvisioningFinishedTime** – označava vrijeme završetka kada OneNote završava dodjelu resursa bilježnici tijekom iskustva prvog pokretanja.

- **ProvisioningStartedTime** – označava vrijeme početka kada OneNote započinje dodjelu resursa bilježnici tijekom iskustva prvog pokretanja.

- **ShowSuggestedNotebooks** – označava hoće li OneNote prikazati predloženu značajku bilježnice ili ne.

#### <a name="officeonenotefirstrunfirstrunfororgid"></a>Office.OneNote.FirstRun.FirstRunForOrgId

Ključni signal korišten za osiguravanje da novi korisnici iz velike tvrtke (AAD/OrgID) uspješno mogu prvi put pokrenuti aplikaciju OneNote.  Telemetrija korištena za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. Ako korisnici ne mogu prvi put pokrenuti aplikaciju, time bi se izazvao incident visoke ozbiljnosti.

- **Attempt** – broj puta koji se iskustvo prvog pokretanja treba ponovno pokušati.

- **Error** – objekt pogreške aplikacije OneNote označava pogrešku tijekom prvog pokretanja ako ona postoji.

- **FAllowAddingGuide** – označava hoće li OneNote dopustiti stvaranje bilježnice vodiča ili ne.

- **IsDefaultNotebookCreated** – označava je li aplikacija OneNote stvorila zadanu bilježnicu korisnika ili nije.

- **ProvisioningFailure** – objekt pogreške aplikacije OneNote koji označava pogrešku dodjele resursa ako ona postoji.

- **ProvisioningFinishedTime** – označava vrijeme završetka kada OneNote završava dodjelu resursa bilježnici tijekom iskustva prvog pokretanja.

- **ProvisioningStartedTime** – označava vrijeme početka kada OneNote započinje dodjelu resursa bilježnici tijekom iskustva prvog pokretanja.

#### <a name="officeonenotefirstrunmrureadernotebookentries"></a>Office.OneNote.FirstRun.MruReaderNoteBookEntries 

Signal koji se koristi za bilježenje problema koji su se pojavili pri učitavanju bilježnica tijekom prvog pokretanja.  Telemetrija se koristi za nadgledanje, otkrivanje i ispravljanje problema pri prvom pokretanju.

Prikupljaju se sljedeća polja: 

- **OnPremNBCount** – Broj bilježnica na lokalnom poslužitelju

- **TotalNBCount** – Ukupan broj bilježnica povezanih s korisničkim računom

#### <a name="officetargetedmessagingensurecached"></a>Office.TargetedMessaging.EnsureCached 

Prati je li preuzet paket za dinamičko radno područje. Smatra se softverskom konfiguracijom jer se paket mora uspješno preuzeti da bi klijent mogao omogućiti pravo iskustvo. Osobito je važno u korisničkim pretplatama u kojima obavještavamo korisnika putem radnog područja da je licenca istekla. Koristi se za praćenje metapodataka paketa dinamičnog sadržaja kojeg je preuzeo i predmemorirao proizvod, i rezultate radnji izvršenih na paketu: neuspjela preuzimanja, neuspjela raspakiranja, pogreške provjere dosljednosti, pronalaženje objekata u predmemoriji, načini korištenja paketa, izvori preuzimanja.

Prikupljaju se sljedeća polja:

  - **Data\_CacheFolderNotCreated –** Booleova zastavica koja označava je li uspjelo stvaranje mape predmemorije

  - **Data\_CdnPath – izvorna adresa paketa-**

  - **Data\_EnsureCached –** Booleova zastavica koja označava je li paket sadržaja predmemoriran

  - **Data\_ExistsAlready –** Booleova zastavica koja označava da je paket već preuzet i da je došlo do drugog pokušaja

  - **Data\_GetFileStreamFailed –** izvorni paket nije dostupan u izvoru

  - **Data\_GetFileStreamFailedToCreateLocalFolder –** problemi s lokalnim diskom uzrokuju pogreške tijekom stvaranja direktorija

  - **Data\_GetFileStreamFromPackageFailed –** zastavica koja označava je li paket preuzet, ali ga klijent ne može čitati

  - **Data\_GetFileStreamFromPackageSuccess –** uspješni pokušaji čitanja paketa

  - **Data\_GetFileStreamSuccess –** nema problema s diskom ni problema s konfiguracijom koji ne dopuštaju čitanje tijeka podataka

  - **Data\_GetRelativePathsFailed –** relativni put ne upućuje na dostupno mjesto

  - **Data\_HashActualValue –** vrijednost raspršivanja izdvojena iz naziva datoteke kada je paket korišten

  - **Data\_HashCalculationFailed –** pogreška s izračunom raspršivanja

  - **Data\_HashMatchFailed –** nepodudarnost raspršivanja između naziva paketa i predmemorirane vrijednosti registra

  - **Data\_HashMatchSuccess –** provjera uspjeha dosljednosti raspršivanja

  - **Data\_PackageDownloadRequestFailed –** nije moguće preuzeti paket

  - **Data\_PackageDownloadRequestNoData –** preuzeti paket ne sadrži podatke

  - **Data\_PackageDownloadRequestSuccess –** uspješno preuzimanje paketa

  - **Data\_PackageExplodedSuccess –** statusi pokušaja raspakiranja

  - **Data\_PackageOpenFailed –** neuspjeli pokušaji otvaranja datoteke paketa

  - **Data\_PackageOpenSuccess –** uspješni pokušaji otvaranja datoteke paketa

  - **Data\_SuccessHashValue –** vrijednost raspršivanja izdvojena iz naziva datoteke kada je paket preuzet

  - **Data\_SuccessSource –** površina za koju je paket preuzet

#### <a name="officevisiovisiosku"></a>Office.Visio.VisioSKU

Bilježi standardni ili profesionalni SKU programa Visio. Bitno za kategoriziranje problema na temelju SKU-a.

Prikupljaju se sljedeća polja:

  - **Data\_VisioSKU**:**integer** – 0 za standardni SKU i 1 za profesionalni SKU

### <a name="office-add-in-configuration-subtype"></a>*Podvrsta konfiguracije dodatka za Office*

Softverski dodaci i njihove postavke.

#### <a name="exceladdindefinedfunctioncustomfunctionsallinone"></a>Excel.AddinDefinedFunction.CustomFunctionsAllInOne

Prikuplja informacije o ponašanju izvođenja prilagođenih funkcija dodataka. Održava brojače pokušaja provedbe, uspješnih provedbi, infrastrukturnih pogrešaka i pogrešaka korisničkog koda. To se upotrebljava za prepoznavanje problema s pouzdanošću u proizvodu i uklanjanje problema koji utječu na korisnika.
 
Prikupljaju se sljedeća polja:

- **AsyncBegin** – broj asinkronih funkcija koje započinju

- **AsyncEndAddinError** – broj asinkronih funkcija koje završavaju pogreškom

- **AsyncEndInfraFailure** – broj asinkronih funkcija koje završavaju infrastrukturnim kvarom

- **AsyncEndSuccess** – broj asinkronih funkcija koje završavaju uspješno

- **AsyncRemoveCancel** – broj asinkronih funkcija koje su otkazane 

- **AsyncRemoveRecycle** – broj asinkronih funkcija koje su uklonjene zbog recikliranja 

- **StreamingCycles1** – brojač ciklusa strujanja

#### <a name="officeextensibilityappcommandsappcmdprojectionstatus"></a>Office.Extensibility.AppCommands.AppCmdProjectionStatus

Prikuplja informacije radi praćenja koje su instalacije dodatka za Office uspješno ažurirale vrpcu, a koje nisu.

Koristi se za rješavanje uobičajenih problema s registracijom kada dodaci nisu pravilno instalirani i nikad se ne prikazuju, zbog čega su neupotrebljivi.

Prikupljaju se sljedeća polja:

  - Nijedno

#### <a name="officeextensibilityappcommandsaddsolution"></a>Office.Extensibility.AppCommands.AddSolution

Prikuplja informacije o instalaciji za dodatke sustava Office koje prilagođavaju vrpcu.  Koristi se za otkrivanje problema s načinom na koji prilagođeni dodaci izmjenjuju vrpcu sustava Office.
 
Prikupljaju se sljedeća polja:

- **AppVersion** – verzija aplikacije

- **SolutionId** – ID rješenja

- **StoreType** – označava porijeklo aplikacije


#### <a name="officeextensibilitycatalogexchangegetentitlements"></a>Office.Extensibility.Catalog.ExchangeGetEntitlements

Podaci o uspjehu ili neuspjehu dohvaćanja podataka o pravima dodataka za administratore klijenta za Office 365. Koristi se za metriku stanja, grafikone i analizu korisničkih problema.

Prikupljaju se sljedeća polja:

  - **CachingResult –** rezultat pokušaja spremanja povratne vrijednosti servisnog poziva

  - **ClientParameter –** identifikator klijenta poslan u servisnom pozivu

  - **EntitlementsCount –** broj prava očekivanih u odgovoru na poziv

  - **EntitlementsParsed –** broj raščlanjenih prava iz odgovora

  - **IsAllEntitlementsParsed –** odgovara li broj očekivanih prava broju raščlanjenih prava

  - **ServiceCallHResult –** rezultat koji vraća API servisnog poziva

  - **TelemetryId –** GUID koji predstavlja jedinstvenog korisnika

  - **UsedCache –** je li korišten predmemorirani odgovor umjesto upućivanja servisnog poziva

  - **VersionParameter –** broj verzije sustava Office poslan u servisnom pozivu

#### <a name="officeextensibilitycatalogexchangegetlastupdate"></a>Office.Extensibility.Catalog.ExchangeGetLastUpdate

Podaci o uspjehu ili neuspjehu dohvaćanja potrebnih ažuriranih podataka dodataka za administratore klijenta za Office 365. Koristi se za metriku stanja, grafikone i analizu korisničkih problema. ExchangeGetLastUpdate uvijek se pokreće pri pokretanju u sklopu koda glavnog računala i utvrđuje jesu li se promijenili zadaci dodatka za korisnika.   Ako je tako, osf.DLL će se učitati pa možemo pozvati ExchangeGetEntitlements radi dobivanja određenih zadataka (pozvat će se i ExchangeGetManifests radi dohvaćanja novih potrebnih manifesta).   ExchangeGetEntitlements (i ExchangeGetManifests) mogu se također pozvati na zahtjev kada je glavna aplikacija pokrenuta.   Svrha je toga da se ne učita veliki DLL ako nije potreban.   Bez tog događaja u atributu Obavezno ne bismo mogli znati jesu li pokušaji korisnika da dobiju dodijeljene dodatke neuspješni ako prvi servisni poziv ne uspije.   To je i glavni signal za probleme s provjerom autentičnosti s kojima smo suočeni pri razgovaranju sa servisom.

Prikupljaju se sljedeća polja:

  - **Abort –** je li glavno računalo isključeno tijekom servisnog poziva

  - **AllowPrompt –** je li dopušten upit za provjeru autentičnosti

  - **AuthScheme –** shema provjere autentičnosti koju zahtijeva sustav Exchange

  - **BackEndHttpStatus –** http kod prijavljen tijekom razgovora s pozadinskim poslužiteljem sustava Exchange

  - **BackupUrl –** sekundarni URL sustava Exchange za poziv

  - **BEServer –** naziv pozadinskog poslužitelja sustava Exchange

  - **CalculatedBETarget –** puni naziv pozadinskog računala sustava Exchange

  - **Call(n)\_TokenAuthError –** pogreška provjere autentičnosti n-tog pokušaja servisnog poziva

  - **Call(n)\_TokenIsValid –** je li token provjere autentičnosti na n-tom pokušaju servisa valjan

  - **CallMethod –** niz koji označava put koda

  - **ConfigSvcReady –** je li pokrenut servis za konfiguraciju

  - **Date –** vrijednost koju vraća poslužitelj sustava Exchange

  - **DiagInfo –** informacije koje vraća poslužitelj sustava Exchange

  - **End\_TicketAuthError –** pogreške u dobivanju potvrde za provjeru autentičnosti nakon servisnog poziva

  - **End\_TokenIsValid –** je li potvrda za provjeru autentičnosti valjana nakon servisnog poziva

  - **EndingIdentityState –** prijavljeno stanje objekata identiteta nakon servisnih poziva

  - **EwsHandler –** vraćena vrijednost iz sustava Exchange

  - **FEServer –** prednji poslužitelj sustava Exchange koji obrađuje zahtjev

  - **HResult –** kod rezultata

  - **HttpStatus –** Http kod stanja koji vraća sustav Exchange

  - **IsSupportedAuthResponse –** možemo li koristiti vrstu autentičnosti

  - **LastUpdateValueRegistry –** vrijednost raspršivanja dohvaćena iz registra

  - **LastUpdateValueRetrieved –** vrijednost raspršivanja koju vraća servisni poziv

  - **MSDiagnostics –** vraćena vrijednost iz sustava Exchange

  - **MsoHttpResult –** vrijednost identifikatora koju vraća http API

  - **NeedRefresh –** ovo polje sadrži vrijednost Točno ili Netočno te označava jesu li podaci dodatka zastarjeli i jesmo li ih ažurirali.

  - **PrimaryUrl –** glavni URL kojem je upućen servisni poziv

  - **RequestId –** vraćena vrijednost iz sustava Exchange

  - **RequestTryCount –** broj pokušaja upućivanja servisnog poziva

  - **RequestTryCount –** broj pokušaja obraćanja sustavu Exchange

  - **ResultChain –** niz koda rezultata iz svakog pokušaja servisnog poziva

  - **StartingIdentityState –** prijavljeno stanje objekata identiteta nakon servisnih poziva

  - **TelemetryId –** GUID koji predstavlja jedinstvenog korisnika i označava jesu li potrebni drugi servisni pozivi

#### <a name="officeextensibilitycatalogexchangegetmanifests"></a>Office.Extensibility.Catalog.ExchangeGetManifests

Podaci o uspjehu ili neuspjehu dohvaćanja podataka manifesta dodataka za administratore klijenta za Office 365. Koristi se za metriku stanja, grafikone i analizu korisničkih problema.

Prikupljaju se sljedeća polja:

  - **CachedManifestsParsed** – broj manifesta pronađenih u predmemoriji

  - **IsAllReturnedManifestsParsed** – mogu li se svi vraćeni manifesti raščlaniti

  - **ManifestsRequested** – broj potrebnih manifesta

  - **ManifestsReturned** – broj manifesta vraćenih s poslužitelja

  - **ManifestsToRetrieve** – broj manifesta koje treba dobiti od poslužitelja

  - **ReturnedManifestsParsed** – broj manifesta vraćenih s poslužitelja koji su uspješno raščlanjeni

  - **TelemetryId** – GUID koji predstavlja jedinstvenog korisnika

#### <a name="officeextensibilityuxfensureloadosfdll"></a>Office.Extensibility.UX.FEnsureLoadOsfDLL 

Prati neuspješno učitavanje datoteke Osf.DLL. Otkrij neuspjeh učitavanja DLL-a koji sprječava pokretanje značajke.

Prikupljaju se sljedeća polja:

  - Ne koristi

#### <a name="officeextensibilityuxfensureloadosfuidll"></a>Office.Extensibility.UX.FEnsureLoadOsfUIDLL 

Prati neuspješno učitavanje datoteke OsfUI.DLL. Otkrij neuspjeh učitavanja DLL-a koji sprječava pokretanje značajke.

Prikupljaju se sljedeća polja:

  - Ne koristi

#### <a name="officeextensibilityuxfensureosfshareddllload"></a>Office.Extensibility.UX.FEnsureOsfSharedDLLLoad 

Prati neuspješno učitavanje datoteke OsfShared.DLL. Otkrij neuspjeh učitavanja DLL-a koji sprječava pokretanje značajke.

Prikupljaju se sljedeća polja:

  - Ne koristi

#### <a name="officeextensibilityvbatelemetrycomobjectinstantiated"></a>Office.Extensibility.VBATelemetryComObjectInstantiated

Prikuplja informacije o pozivanju poslužitelja za automatizaciju ili klijenta u rješenjima VBA. Koristi se za razumijevanje interakcije između objekata VBA i COM.

Prikupljaju se sljedeća polja:

  - **ComObjectInstantiatedCount** – broj instanci objekta COM

  - **HashComObjectInstantiatedClsid** – identifikator klase raspršivanja objekta COM

  - **HashProjectName** – raspršivanje naziva VBA projekta

  - **TagId** – jedinstvena oznaka

#### <a name="officeextensibilityvbatelemetrydeclare"></a>Office.Extensibility.VBATelemetryDeclare 

Prikuplja informacije o pozivanju API-jeva Win32 u rješenjima VBA. Koristi se za razumijevanje interakcije između VBA rješenja i upotrebe i dopunjavanje istraživanja sigurnosti.

Prikupljaju se sljedeća polja:

  - **DeclareCount** – broj deklaracija

  - **HashDeclare** – raspršivanje naziva DLL-a

  - **HashEntryPoint** – raspršivanje naziva API-ja

  - **HashProjectName** – raspršivanje naziva VBA projekta

  - **IsPtrSafe** – je li naredba deklariranja kompatibilna za različite arhitekture

  - **TagId** – jedinstvena oznaka

#### <a name="officeoutlookdesktopadd-insadd-inloaded"></a>Office.Outlook.Desktop.Add-ins.Add-inLoaded

Prikuplja uspjeh i neuspjeh učitavanja dodatka u Outlook. Ti se podaci aktivno nadziru da bi se osigurao pravilan rad programa Outlook s dodacima korisnika Ti se podaci koriste za otkrivanje i istraživanje problema.

Prikupljaju se sljedeća polja:

  - **Standardna HVA aktivnost** bez prilagođenog opterećenja

#### <a name="officeoutlookmacaddinapiusage"></a>Office.Outlook.Mac.AddinAPIUsage

Prikuplja uspješne i neuspješne provedbe dodataka u programu Outlook. Ti se podaci aktivno nadziru da bi se osigurao pravilan rad programa Outlook s dodacima. Ti se podaci koriste za otkrivanje i istraživanje problema.

Prikupljaju se sljedeća polja:

- **AccountType** – vrsta računa koji je povezan s dodatkom 

- **Cookie** – kolačić koji dodatak koristi

- **DispId** – identifikator isporuke 

- **EndTime** – vrijeme kada je dodatak završio 

- **ExecutionTime** – vrijeme proteklo tijekom provedbe dodatka 

- **Result** – rezultat korištenja dodatka u programu Outlook 

- **StartTime** – vrijeme početka dodatka


#### <a name="officeoutlookmacaddineventapisusage"></a>Office.Outlook.Mac.AddinEventAPIsUsage

Prikuplja uspješne ili neuspješne provedbe dodataka u programu Outlook. Ti se podaci aktivno nadziru da bi se osigurao pravilan rad programa Outlook s dodacima. Ti se podaci koriste za otkrivanje i istraživanje problema.

Prikupljaju se sljedeća polja:

- **AddinType** – vrsta dodatka 

- **EventAction** – radnja koju izvršava dodatak 

- **EventDispid** – identifikator isporuke

- **EventResult** – rezultat radnje koju je proveo dodatak 

#### <a name="officeoutlookmacaddininstallationfrominclientstore"></a>Office.Outlook.Mac.AddInInstallationFromInClientStore

Prikuplja uspješne ili neuspješne instalacije dodataka u programu Outlook. Ti se podaci aktivno nadziru da bi se osigurao pravilan rad programa Outlook s dodacima. Ti se podaci koriste za otkrivanje i istraživanje problema.

Prikupljaju se sljedeća polja:

- **AccountType** – vrsta računa koji je povezan s dodatkom 

- **FailureReason** – razlog zbog kojeg instalacija dodatka nije bila uspješna 

- **MarketplaceAssetId** – identifikator dodataka trgovine 

- **Status** – status instalacije dodatka


#### <a name="officeprogrammabilityaddinsinternalsetconnectenterprise"></a>Office.Programmability.Addins.InternalSetConnectEnterprise

Događaj koji se stvara kada je COM dodatak učitan na uređaju sa sustavom Enterprise. Koristi se za utvrđivanje problema s usvajanjem, izvedbom i pouzdanošću dodataka za Office. 

Prikupljaju se sljedeća polja:

  - **Activity Result** – Stanje uspjeha veze *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

  - **AddinConnectFlag** – predstavlja ponašanje učitavanja 

  - **Add-inDescriptionV2** – opis dodatka

  - **Add-inFileNameV2** – naziv datoteke dodatka, bez puta datoteke

  - **AddinFriendlyNameV2** – neslužbeni naziv dodatka

  - **Add-inId** – the add-in Class ID *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **AddinIdV2** – ID klase dodatka

  - **AddinProgIdV2** – programski ID dodatka

 - **Add-inProviderV2** – davatelj dodatka

  - **Add-inTimeDateStamp** – Vremenska oznaka dodatka iz DLL metapodataka *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

  - **AddinTimeDateStampV2** – vremenska oznaka dodatka iz metapodataka DLL-a

  - **AddinVersionV2** – verzija dodatka

  - **Isbootinprogress** – bez obzira na to je li aplikacija sustava Office u postupku dizanja
 
  - **LoadDuration** – trajanje učitavanja dodatka
  
  - **LoadResult** – uspjeh opterećenja


#### <a name="officevisiovisioaddonload"></a>Office.Visio.Visio.AddonLoad

Bilježi pogreške neuspješnog učitavanja rješenja. Bitno za ispravljanje pogrešaka učitavanja dodatka u programu Visio.

Prikupljaju se sljedeća polja:

  - **Data\_Load1Error:integer** – vrijednost pogreške tijekom učitavanja dodatka za Visio

#### <a name="officevisiovisioaddonusage"></a>Office.Visio.Visio.AddonUsage

Bilježi pogreške kada postoji pogreška u funkciji rješenja. Bitno za ispravljanje pogrešaka dodatka u dodacima.

Prikupljaju se sljedeća polja:

  - **Data\_DocumentSessionLogID:string** – identifikator sesije dokumenta

  - **Data\_IsEnabled**:**bool** – istinito ako je rješenje omogućeno

  - **Data\_TemplateID:string** – GUID predloška u kojem je rješenje učitano. Zapisano kao 0 za prilagođeno rješenje

  - **Data\_AddOnID**:**string** – GUID za prepoznavanje učitanog dodatka

  - **Data\_Error**:**integer** – ID pogreške

### <a name="security-subtype"></a>*Podvrsta sigurnosti*

Uvjeti za pogreške u dokumentima, značajkama i dodacima koji mogu ugroziti sigurnost, uključujući spremnost proizvoda za ažuriranje.

#### <a name="officeappguardcreatecontainer"></a>Office.AppGuard.CreateContainer

Prikupljamo kodove pogrešaka te informacije o tome je li spremnik već postojao ili nije. Prikupljamo i kodove pogrešaka za ponovno postavljanje u slučaju da ne uspijemo stvoriti spremnik pri prvom pokušaju. Podaci će se upotrebljavati za identifikaciju postotka sesija za koje uspješno stvorimo spremnik za pokretanje aplikacija Office Application Guard. Također, podaci će Microsoftu omogućiti identifikaciju i rješavanje kodova pogrešaka u vezi sa stvaranjem spremnika.

Prikupljaju se sljedeća polja:

- **ErrorCode1** – vrsta koda pogreške za postavljanje spremnika.  

- **ErrorCode2** – kôd pogreške iz provedbe stvaranja. 

- **ErrorCode3** – dodatni kôd pogreške. 

- **Id** – jedinstveni identifikator (GUID) za stvaranje spremnika.

- **ResetError** – kôd pogreške iz pokušaja ponovnog postavljanja spremnika nakon neuspješna pokušaja.

- **ResetErrorCode1** – vrsta koda pogreške postavljanja spremnika nakon naredbe za ponovno postavljanje. 

- **ResetErrorCode2** – kôd pogreške iz provedbe stvaranja nakon naredbe za ponovno postavljanje.

- **ResetErrorCode3** – dodatni kôd pogreške nakon naredbe za ponovno postavljanje.

- **ResetErrorType** – vrsta pogreške tijekom ponovnog postavljanja: Stvaranje, Priprema datoteke ili Pokretanje.

- **WarmBoot** – prepoznaje je li spremnik već bio stvoren ili nije.

#### <a name="officeappguardlaunchfile"></a>Office.AppGuard.LaunchFile

Ovaj događaj označava rezultat izvođenja datoteke za pokretanje alata Application Guard. Moći ćemo odrediti postotak sesija u kojima je uspješno pokrenuta datoteka programa Word, Excel ili PowerPoint te šifre pogrešaka za neuspjele pokušaje.

Prikupljaju se sljedeća polja:

- **AppId** – identificira aplikaciju koja se pokreće.

- **DetachedDuration** – označava ukupno trajanje spojene aktivnosti. 

- **ErrorCode1** – vrsta koda pogreške pri postavljanju spremnika.  

- **ErrorCode2** – kôd pogreške pri provedbi stvaranja. 

- **ErrorCode3** – dodatni kôd pogreške. 

- **FileId** – jedinstveni identifikator (GUID) koji je Windows API vratio nakon pokretanja datoteke.

- **ID** – jedinstveni identifikator (GUID) za pokretanje i stvaranje datoteke. Taj se identifikator koristi za korelaciju događaja iz sustava Office i Windows.

- **ResetError** – kôd pogreške iz pokušaja ponovnog postavljanja spremnika nakon neuspješnog pokušaja.

- **ResetErrorCode1** – vrsta koda pogreške postavljanja spremnika nakon naredbe za ponovno postavljanje. 

- **ResetErrorCode2** – kôd pogreške iz provedbe stvaranja nakon naredbe za ponovno postavljanje.

- **ResetErrorCode3** – dodatni kôd pogreške nakon naredbe za ponovno postavljanje.  

- **ResetErrorType** – vrsta pogreške: Stvaranje, PrepFile ili Pokretanje.



#### <a name="officesecurityactivationfilterclsidactivated"></a>Office.Security.ActivationFilter.CLSIDActivated

Prati kada je u sustavu Office aktiviran identifikator određene klase (Flash, Silverlight itd). Koristi se za praćenje učinka blokiranja kontrola za Flash, Silverlight i Shockwave na krajnje korisnike.

Prikupljaju se sljedeća polja:

  - **ActivationType** – vrsta aktivacije za kontrolu

  - **Blokirano** – je li kontrolu blokirao sustav Office

  - **CLSID** – identifikator klase kontrole

  - **Count** – koliko je puta kontrola aktivirana

#### <a name="officesecurityactivationfilterfailedtoregister"></a>Office.Security.ActivationFilter.FailedToRegister

Prati uvjet pogreške u rješavanju sigurnosti koji blokira aktivaciju opasnih kontrola u sustavu Office.

Koristi se za dijagnosticiranje uvjeta pogreške u rješavanju sigurnosti koji bi mogli utjecati na sigurnost krajnjih korisnika.

Prikupljaju se sljedeća polja:

  - Ne koristi

#### <a name="officesecuritycomsecurityfileextensionlistfromservice"></a>Office.Security.ComSecurity.FileExtensionListFromService

Prati jesu li proširenja blokiranja programa za pakiranje čitana iz servisa za konfiguraciju ili smo koristili zadani popis klijenta. Koristi se da bi se osigurala učinkovitost rješavanja sigurnosti koja štiti krajnje korisnike sustava Office.

Prikupljaju se sljedeća polja:

  - **RetrievedFromServiceStatus** – jesmo li uspjeli dohvatiti popis datotečnih nastavaka za blokiranje, a ako ne, koji je razlog pogreške

#### <a name="officesecuritycomsecurityload"></a>Office.Security.ComSecurity.Load

Prati kada je OLE objekt učitan u dokumentu. Koristi se da bi se osigurala učinkovitost rješavanja sigurnosti koja štiti krajnje korisnike sustava Office.

Prikupljaju se sljedeća polja:

  - **Clsid** – identifikator klase OLE kontrole

  - **Count** – koliko je puta OLE kontrola učitana

  - **DocUrlHash** – raspršivanje koje jedinstveno označava dokument. (Napomena – iz toga nije moguće saznati stvarne pojedinosti o dokumentu. To je samo jedinstvena oznaka dokumenta.)

  - **IsCategorized** – je li OLE kontrola kategorizirana za učitavanje u sustavu Office

  - **IsInsertable** – može li se OLE kontrola umetnuti

#### <a name="officesecuritycomsecurityobjdetected"></a>Office.Security.ComSecurity.ObjDetected

Prati kada je OLE objekt otkriven u dokumentu. Koristi se da bi se osigurala učinkovitost rješavanja sigurnosti koja štiti krajnje korisnike sustava Office.

Prikupljaju se sljedeća polja:

  - **Clsid** – identifikator klase OLE kontrole

  - **Count** – koliko je puta otkriven ovaj OLE objekt

  - **DocUrlHash** – raspršivanje koje jedinstveno označava dokument. (Napomena – iz toga nije moguće saznati stvarne pojedinosti o dokumentu. To je samo jedinstvena oznaka dokumenta.)

  - **IsCategorized** – je li OLE kontrola kategorizirana za učitavanje u sustavu Office

  - **IsInsertable** – može li se OLE kontrola umetnuti

#### <a name="officesecuritycomsecuritypackageractivation"></a>Office.Security.ComSecurity.PackagerActivation

Prati ishod rješavanja sigurnosti koje blokira opasna proširenja ugrađena u dokumentima sustava Office. Koristi se da bi se osigurala učinkovitost rješavanja sigurnosti koja štiti krajnje korisnike sustava Office.

Prikupljaju se sljedeća polja:

  - **FromInternet** – je dokument s interneta

  - **PackagerSetting** – je trenutna postavka programa za pakiranje

  - **TrustedDocument** – je li dokument pouzdan

#### <a name="officesecuritycomsecuritypackageractivationerrors"></a>Office.Security.ComSecurity.PackagerActivationErrors

Prati stanja pogreške u rješavanju sigurnosti koje blokira opasna proširenja ugrađena u dokumentima sustava Office. Koristi se da bi se osigurala učinkovitost rješavanja sigurnosti koja štiti krajnje korisnike sustava Office.

Prikupljaju se sljedeća polja:

  - **Pogreška** – kod pogreške

  - **Nastavak** – je datotečni nastavak

  - **FromInternet** – je dokument s interneta

  - **LinkedDocument** – je li dokument povezan

  - **PackagerSetting** – je trenutna postavka programa za pakiranje

  - **TrustedDocument** – je li dokument pouzdan


#### <a name="officesecuritymacrointernetvbablockenabled"></a>Office.Security.Macro.InternetVBABlockEnabled

Prati je li postavka Blokiraj makronaredbu s interneta omogućena u klijentu. Procjena rješavanja sigurnosti radi zaštite od zlonamjernih makronaredbi.

Prikupljaju se sljedeća polja:

  - Ne koristi

#### <a name="officesecuritymacropolicydigsigtrustedpublishers"></a>Office.Security.Macro.PolicyDigSigTrustedPublishers

Prati je li provjereno da je makronaredba od pouzdanog izdavača. Koristi se da bi se osigurala učinkovitost rješavanja sigurnosti koja štiti krajnje korisnike sustava Office.

Prikupljaju se sljedeća polja:

  - **Policy** – je pravilnik koji je postavljen, nije postavljen ili nije dostupan

#### <a name="officesecuritymacroprompted"></a>Office.Security.Macro.Prompted

Prati kada se od korisnika traži da omogući VBA makronaredbe. Koristi se za procjenu rasprostranjenosti VBA makronaredbi i poboljšanje budućeg rješavanja sigurnosti koje ograničava izvođenje makronaredbe kao odgovor na sigurnosne incidente.

Prikupljaju se sljedeća polja:

  - **PromptType** – vrsta prikazanog upita

  - **VBAMacroAntiVirusHash** – antivirusno raspršivanje makronaredbe

  - **VBAMacroAntiVirusHRESULT** – rezultat antivirusne procjene

#### <a name="officesecuritymacrovbasecureruntimesessionenablestate"></a>Office.Security.Macro.VBASecureRuntimeSessionEnableState

Prati svaku provjeru AMSI izvođenja kada se izvršava makronaredba. Prati učinkovitost provjere AMSI izvođenja makronaredbe te prepoznaje pogreške koje bi mogle utjecati na sigurnost krajnjih korisnika.

Prikupljaju se sljedeća polja:

  - **IsRegistry** – je li administrator postavio neko nadjačavanje u registru

  - **Stanje** – koje je stanje za sigurno izvođenje

#### <a name="officesecuritymacroxl4prompted"></a>Office.Security.Macro.XL4Prompted

Prati kada se od korisnika traži da omogući XL4 makronaredbe. Koristi se za procjenu rasprostranjenosti XL4 makronaredbi u programu Excel radi poboljšanja budućeg rješavanja sigurnosti koje po zadanom blokira XL4 kao odgovor na sigurnosne incidente koji obuhvaćaju zlouporabu XL4 makronaredbi.

Prikupljaju se sljedeća polja:

  - **PromptType** – vrsta prikazanog upita


#### <a name="officesecurityocxufiprompt"></a>Office.Security.OCX.UFIPrompt

Prati kada se sigurnosni upit prikazuje korisniku prilikom učitavanja ActiveX kontrole koja je označena kao nepouzdana za inicijalizaciju. Koristi se za praćenje rasprostranjenosti UFI ActiveX kontrola u dokumentima sustava Office za poboljšanje rješavanja (na primjer, kontrole značajke killbit) kao odgovor na sigurnosne incidente.

Prikupljaju se sljedeća polja:

  - **IsFromInternet** – je dokument otvoren s interneta

  - **IsSecureReaderMode** – je dokument otvoren u sigurnom čitaču

  - **OcxTrustCenterSettings** – koja je trenutna postavka za ActiveX


#### <a name="officesecuritysecurereaderhostopeninosr"></a>Office.Security.SecureReaderHost.OpenInOSR

Prati postupak otvaranja u zaštićenom prikazu. Koristi se za dijagnosticiranje stanja koja vode do pogrešaka prilikom otvaranja datoteka u zaštićenom prikazu koje utječu na sigurnost i produktivnost korisnika.

Prikupljaju se sljedeća polja:

  - Ne koristi

## <a name="product-and-service-usage-data-events"></a>Podatkovni događaji koji se odnose na korištenje proizvoda i usluga

Ovo su podvrste podataka u toj kategoriji:

- [Uspjeh značajki aplikacije](#application-feature-success-subtype)
- [Status i pokretanje aplikacije](#application-status-and-boot-subtype)
- [Konfiguracija pristupačnosti za Office](#office-accessibility-configuration-subtype)
- [Zaštita privatnosti](#privacy-subtype)


### <a name="application-feature-success-subtype"></a>*Podvrsta uspjeha značajke aplikacije*

Uspješno funkcioniranje aplikacije. Ograničeno na otvaranje i zatvaranje aplikacije i dokumenata, uređivanje datoteka i zajedničko korištenje dokumenata (suradnju).

#### <a name="accountaction"></a>account.action

Potrebno za osiguranje da konfiguracija računa uspješno radi i koristi za nadzor stanja kreiranja računa, mogućnost dodavanja novih računa e-pošte i nadzor softverskog vraćanja izvornih postavki računa 

Prikupljaju se sljedeća polja: 

- **account_calendar_count** – broj kalendara koji račun ima
 
- **action** – vrsta provedene radnje, npr. create_account, delete_account.
 
- **duration_seconds** – trajanje radnje
 
- **entry_point** – ulazna točka radnje, kako je korisnik pokrenuo radnju
 
- **has_hx** – ima li uređaj račun koji koristi našu novu uslugu sinkronizacije e-pošte, ne nužno račun na kojem je radnja provedena
 
- **is_hx** – koristi li račun našu novu uslugu sinkronizacije e-pošte
 
- **is_shared_mailbox** – odnosi li se radnja na zajednički poštanski sandučić
 
- **number_of_accounts** – ukupan broj računa na kojima se radnja provodi
 
- **result** – rezultat radnje, npr. uspjeh, neuspjeh.
   
- **server_type** – vrsta poslužitelja za račun, slično kao account_type
 
- **shared_type** – vrsta zajedničkog računa (ako se račun zajednički koristi)
 
- **scope** – opseg radnje; za brisanje računa, this_device ili all_devices
 
- **total_calendar_accounts** – broj računa za kalendar u aplikaciji u trenutku radnje
 
- **total_email_accounts** – broj računa e-pošte u aplikaciji u trenutku radnje
 
- **total_file_accounts** – broj računa datoteka u aplikaciji u trenutku radnje

#### <a name="accountlifecycle"></a>account.lifecycle

Ovaj se događaj prikuplja za osiguranje da konfiguracija računa uspješno radi i koristi za nadzor stanja kreiranja računa, mogućnost dodavanja novih računa e-pošte i nadzor softverskog vraćanja izvornih postavki računa.

Prikupljaju se sljedeća polja: 

- **account_creation_source** – neobavezno svojstvo koje se upotrebljava za pronalazak i dijagnozu svih problema koji se pojavljuju tijekom stvaranja računa kada se doda vrsta radnje.  Ono može imati vrijednosti kao što su jedinstvena prijava (SS0), create_new_account, manual, itd.

- **action** – vrsta radnje provedene na računu, npr. dodavanje, brisanje ili ponovno postavljanje.

#### <a name="addnewaccountstep"></a>add.new.account.step

Ovaj nam događaj omogućuje prepoznati koji je napredak korisnika u stvaranju obrasca za novi račun.  To označava kada je korisnik prešao na drugi korisnik ili je odustao od rada.  Te su nam informacije potrebne da bismo prepoznali postoje li neispravni koraci te da bismo osigurali da je stvaranje korisničkog računa bilo uspješno. 

Prikuplja se sljedeće polje: 

- **OTAddAccountCurrentStep** – to može imati sljedeće vrijednosti: profile_form, redirect_mobile_check, mobile_check_success

#### <a name="apperror"></a>app.error

Prati kritične pogreške korištene aplikacije da bismo mogli spriječiti probleme koji mogu prouzročiti rušenje aplikacije ili vam onemogućiti čitanje e-pošte.

Prikupljaju se sljedeća polja: 

- **clientName** – naziv klijenta za datoteku u oblaku u kojoj je pogreška nastupila, ako je primjenjivo.

- **cloudfile_error_type** – vrsta pogreške koja je nastupila za datoteku u oblaku, ako je primjenjivo.

- **cloudfile_response_name** – naziv odgovora za pogrešku koja je nastupila za datoteku u oblaku, ako je primjenjivo.

- **component_name** – naziv komponente aplikacije u kojoj je pogreška nastupila, primjerice pošta ili kalendar.

- **debug_info** – informacije o pogrešci koja je nastupila za datoteku u oblaku kako bi se moglo utvrditi zašto je pogreška nastupila.

- **error_origin_identifier** – porijeklo pogreške koja je nastupila na skici na kojoj je pogreška nastupila, ako je primjenjivo.

- **error_type** – vrsta pogreške koja je nastupila. Neki primjeri obuhvaćaju spremanje skice, slanje skice i pogrešku datoteke u oblaku.

- **exdate** – datum proširenog pravila (odnosi se samo na pogreške ponavljanja obveze) *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

- **exrule** – vrijednost proširenog pravila (odnosi se samo na pogreške ponavljanja obveze) *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

- **has_attachments** – označava ima li skica na kojoj je pogreška nastupila privitke, ako je primjenjivo.

- **is_IRM_protected** – označava je li skica na kojoj je pogreška nastupila zaštićena upravljanjem pravima na informacije, ako je primjenjivo.

- **is_legitimate** – označava potječe li pogreška iz pogreške u programiranju ili ne. Pogreške u programiranju ne smatraju se valjanima.

- **is_local** – označava je li se skica na kojoj je pogreška nastupila sinkronizirala s poslužiteljem, ako je primjenjivo.

- **is_recoverable** – označava je li kod pogreške riječ o pogrešci koja se može otkloniti ili o fatalnoj pogrešci.

- **rdate** – datum pravila ponavljanja (odnosi se samo na pogreške ponavljanja obveza) *[To je polje uklonjeno iz trenutačnih međuverzija sustava Office, no i dalje se može pojavljivati u starijim međuverzijama.]*

- **rrule** – samo pravilo ponavljanja (odnosi se samo na pogreške ponavljanja obveza) *[To je polje uklonjeno iz trenutačnih međuverzija sustava Office, no i dalje se može pojavljivati u starijim međuverzijama.]*

- **rrule_error_message** – poruka o pogrešci s raščlanjivanjem pravila ponavljanja (odnosi se samo na pogreške ponavljanja obveze) *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

- **rrule_error_type** – vrsta pogreške s raščlanjivanjem pravila ponavljanja (odnosi se samo na pogreške ponavljanja obveze) *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

- **status_code** – kod stanja pogreške koja je nastupila. To nam pomaže razumjeti uzrok pogreške.

Svi su znakovi također moguća svojstva. To nam pomaže razumjeti znakove u tijelu skice poruke kada je pogreška nastupila. Primjerice, „a”, „b” i „c” su moguća svojstva.

#### <a name="applaunchreport"></a>app.launch.report

Ovaj nam događaj omogućava prepoznavanje i popravljanje problema kada se Outlook pokreće sporo ili nepotpuno, zbog čega korisnici imaju probleme s korištenjem naše aplikacije. To uključuje informacije o konkretnim značajkama koje su bile omogućene i koliko su dugo dijelovi pokretanja trajali.

Prikupljaju se sljedeća polja: 

- **is_agenda_widget_active** – govori nam je li widget za dnevni red aktivan.

- **is_alert_available** – govori nam je li aplikacija bila konfigurirana za dopuštanje upozorenja u obavijestima.

- **is_background_refresh_available** – govori nam je li aplikacija bila konfigurirana za osvježavanje u pozadini.

- **is_badge_available** – govori nam je li aplikacija bila konfigurirana za dopuštanje znački u obavijestima.

- **is_intune_managed** – govori nam upravlja li Intune aplikacijom.

- **is_registered_for_remote_notifications** – govori nam je li aplikacija bila registrirana za udaljene obavijesti.

- **is_sound_available** – govori nam je li aplikacija bila konfigurirana za dopuštanje zvukova u obavijestima.

- **is_watch_app_installed** – govori nam je li aplikacija sata za Outlook bila instalirana.

- **is_watch_paired** – govori nam je li aplikacija sata za Outlook uparena s glavnom aplikacijom Outlook.

- **launch_to_db_ready_ms** – govori nam o količini vremena koje je aplikaciji Outlook bilo potrebno od pokretanja do spremnosti baze podataka.

- **num_calendar_accounts** – govori nam broj računa za kalendar u aplikaciji.

- **num_cloud_file_accounts** – govori nam broj računa za pohranu u aplikaciji.

- **num_hx_calendar_accounts** – govori nam broj računa za kalendar u aplikaciji koji se povezuju s našom novom uslugom sinkronizacije pošte.

- **num_hx_mail_accounts** – govori nam broj računa pošte u aplikaciji koji se povezuju s našom novom uslugom sinkronizacije pošte.

- **num_mail_accounts** – govori nam broj računa pošte u aplikaciji.

#### <a name="calendaraction"></a>calendar.action

Koristi se za nadzor svih mogućih negativnih utjecaja na vašu mogućnost provedbe osnovnih radnji kalendara kao što su kreiranje ili uređivanje događaja.  Događaj također može uključivati niz naziva svojstava te jesu li se ona promijenila ili nisu. Primjerice, „title_changed”, „online_meeting_changed” i „description_changed” nazivi su svojstava koja su uključena kako bi nam pomogla razumjeti postoje li problemi s uređivanjem određenih svojstava.

Prikupljaju se sljedeća polja: 

- **account_sfb_enabled** – pomaže nam osigurati da je Skype za tvrtke ispravno konfiguriran. 

- **action** – vrsta radnje koja je provedena na kalendaru. Ovo uključuje stavke kao što su otvaranje, uređivanje, dodavanje prečaca, odgađanje itd. Pomaže nam osigurati da naš kalendar funkcionira u skladu s očekivanjima i da ne postoje oštećenja 

- **action_result** – rezultat radnje provedene na komponentama kalendara. To može uključivati vrijednosti kao što su uspjeh, neuspjeh, nepoznato i vremensko ograničenje. Koristi se za praćenje stope uspješnosti radnji i utvrđivanje postoji li rasprostranjen problem s radnjama kalendara. 

- **attendee_busy_status** – status slobodno/zauzeto sudionika s kojim je radnja povezana. Ova vrijednost može biti slobodno, zauzeto ili uvjetno. Pomaže nam razumjeti postoji li problem s radnjama povezanim s određenim statusom zauzetosti. 

- **availability** – vrijednost dostupnosti ako se vrijednost slobodno/zauzeto promijenila tijekom sastanka. Pomaže nam razumjeti postoje li problemi s postavljanjem određene vrijednosti dostupnosti. 

- **calendar_onlinemeeting_default_provider** – sadrži zadanog davatelja usluge za mrežni sastanak za upotrebu sa stvaranjem mrežnih sastanaka s podrškom poslužitelja. To uključuje vrste programa Skype, Skype za tvrtke, Hangout i Teams za tvrtke. Pomaže nam dijagnosticirati potencijalne probleme s kreiranjem mrežnih sastanaka na određenim davateljima usluga. 

- **calendar_onlinemeeting_enabled** – vrijednost true ako kalendar podržava stvaranje mrežnih sastanaka s podrškom poslužitelja na temelju zadanog davatelja usluga mrežnih sastanaka. Pomaže nam razumjeti postoje li problemi s kalendarima s omogućenim mrežnim sastancima. 

- **calendar_type** – vrsta kalendara na kojem se događaj nalazi nakon što je korisnik uredio sastanak. Moguće vrijednosti uključuju primarno, sekundarno, dijeljeno i grupno. Pomaže nam razumjeti postoje li problemi s određenom vrstom kalendara. 

- **delete_action_origin** – porijeklo provedene radnje brisanja. Ovo uključuje vrijednosti kao što su alatna traka navigacijske trake i alatna traka kapsule.  Pomaže nam razumjeti postoje li problemi s brisanjem sastanka iz određene lokacije. 

- **distribution_list_count** – broj sudionika koji se nalaze na popisima za raspodjelu. Pomaže nam pratiti postoje li problemi sa sudionicima koji se nalaze na popisima za raspodjelu. 

- **guest_count** – broj gostiju u sastanku.  Pomaže nam osigurati da se gosti ispravno dodaju. 

- **is_all_day** – koristi se zajedno s „meeting_duration” za određivanje je li riječ o cjelodnevnom sastanku. Pomaže nam razumjeti postoje li problemi s radnjama provedenim u okviru cjelodnevnih sastanaka. 

- **is_location_permission_granted** – je li korisnik dodijelio dozvolu mjesta sustava aplikaciji. Ako je dodijeljena dozvola mjesta, aplikacija može prikazati dodatne korisne informacije u korisničkom sučelju. Ako znamo da je dozvola lokacije dodijeljena, moći ćemo znati koliko se često dodatne korisne informacije prikazuju korisnicima.

- **is_organizer** – pomaže nam razumjeti može li organizator pravilno uređivati i kreirati sastanke. 

- **is_recurring** – pomaže nam razumjeti postoji li problem koji specifično utječe na ponavljajuće sastanke. 

- **launch_point** – točka pokretanja radnje. Može biti vrijednosti kao što su zaglavlje widgeta, podnožje widgeta, cjelodnevni widget i prečac kalendara. Pomaže nam razumjeti kontekst iz koje je radnja pokrenuta. 

- **location_count** – broj lokacija koje se postavljaju tijekom kreiranja i uređivanja događaja. Pomaže nam razumjeti postoje li problemi s kreiranjem ili uređivanjem događaja s određenim brojem lokacija. 

- **location_selection_source_type** – vrsta izvora za odabir lokacije. Ovo može uključivati vrijednosti kao što su prijedlog lokacije, prilagođeno i postojeće. Pomaže nam dijagnosticirati sve probleme s odabirom lokacije iz određenog izvora. 

- **location_session_id** – ID sesije za odabir lokacije sastanka. Pomaže nam dijagnosticirati sve probleme s odabirom lokacije koja se treba dodati sastanku. 

- **location_type** – vrsta odabrane lokacije.  Sadrži vrste kao što su prilagođena lokacija, konferencijska prostorija i Bing. Pomaže nam razumjeti probleme s dodavanjem određenih vrsta lokacija u sastanak. 

- **meeting_duration** – trajanje sastanka.  Pomaže nam osigurati da se sastanci konfiguriraju s točnim vremenima. 

- **meeting_insights_type** – vrsta uvida u sastanak u pojedinostima o događaju.  Ovo uključuje datoteku i poruku. Pomaže nam razumjeti broj uvida u sastanak koji se prikazuju. 

- **meeting_type** – vrsta mrežnog sastanka povezanog s radnjom.  To uključuje vrste programa Skype, Skype za tvrtke, Hangout i Teams za tvrtke. Pomaže nam razumjeti jesu li mrežni sastanci pravilno konfigurirani. 

- **origin** – porijeklo radnje kalendara. Ovo uključuje vrste kao što su dnevni red, kalendar, dnevni red widgeta itd. Pomaže nam u boljem osiguravanju da interakcija s komponentama kalendara pravilno funkcionira 

- **recurrence_scope** – vrsta ponavljanja sastanka, bilo pojava ili niz.  Pomaže nam razumjeti postoje li problemi s uređivanjem različitih vrsta ponavljanja sastanka. 

- **reminder_time** – vrijeme podsjetnika sastanka ako se ono promijenilo.  Koristi se za osiguravanje da je vrijeme sastanka pravilno spremljeno. 

- **reminders_count** – broj podsjetnika za događaj ako su se podsjetnici promijenili. Pomaže nam dijagnosticirati sve probleme s višestrukim podsjetnicima za događaj. 

- **sensitivity** – osjetljivost sastanka. To uključuje vrste normalno, osobno, privatno i povjerljivo. Pomaže nam razumjeti je li osjetljivost sastanka pravilno konfigurirana. 

- **session_duration** – trajanje sesije u milisekundama. Pomaže nam razumjeti postoje li problemi koji povećavaju količinu vremena potrebnog za provedbu radnje kalendara. 

- **shared_calendar_result** – rezultat radnje provedene na dijeljenom kalendaru. Moguće vrijednosti obuhvaćaju u redu, nema dozvole, nepoznato, lokalni vlasnik i vlasnik je grupa. Pomaže nam razumjeti pouzdanost radnji provedenih na dijeljenim kalendarima. 

- **time_picker_origin** – podrijetlo birača vremena za radnju spremanja. Uključuje vrijednosti kao što su više mogućnosti i manje mogućnosti. Pomaže nam razumjeti kako je korisnik usmjeravao tijek za spremanje sastanka i osigurati da ispravno funkcionira 

- **title** – automatski predloženi naslov iz vrijednosti koje je definirala aplikacija. To uključuje vrijednosti kao što su „Poziv”, „Ručak” i „Skype”. Pomaže nam razumjeti je li automatsko predlaganje naslova pravilno konfigurirano. 

- **txp** – vrsta rezervacije na događaju, ako postoji. Ovo uključuje vrste kao što su rezervacija događaja, rezervacija leta, rezervacija najma automobila itd. Pomaže nam razumjeti funkcioniraju li kartice za rezervaciju pravilno. 

- **upcoming_event_count** – broj predstojećih događaja prikazan u prikazu predstojećih događaja. Pomaže nam razumjeti postoje li problemi s prikazom predstojećih događaja. 

- **upcoming_event_seconds_until_event** – broj sekundi do početka sljedećeg predstojećeg događaja. Pomaže nam razumjeti tipične događaje koji se prikazuju u prikazu predstojećih događaja. 

- **value** – pojedinost specifična za radnju kao što je trajanje odgađanja upozorenja ili kategorija ponavljanja do. Pomaže nam razumjeti kontekst u kojem je radnja provedena. 

#### <a name="combinedsearchuse"></a>combined.search.use

Koristi se za nadzor mogućeg negativnog utjecaja na vašu sposobnost provedbe ključnih funkcija pretraživanja kao što su traženje pošte, kontakata ili događaja.

Sljedeća se polja prikupljaju na svim uređajima iOS i Android: 

- **account_switcher_action_type** – ova vrsta radnje prati je li korisnik koristio preglednik računa bilo u jednostavnom otkrivanju ili se odlučio za promjenu računa

- **action_type** – vrsta radnje koja je provedena za pretraživanje. Ovo prepoznaje je li pretraživanje pokrenuto, provodi li se ili je dovršeno te koje su se radnje provodile tijekom pretraživanja, na primjer, je li korišten mikrofon. Ovo je ključno za osiguravanje točnih i korisnih pretraživanja. 

- **conversation_id** – jedinstveni ID za svaku sesiju pretraživanja (tj. svaki put kada korisnik otvori okvir za pretraživanje)

- **entrance_type** – ovo određuje kako je korisnik pokrenuo upit za pretraživanje, iz kartice Pretraživanje, nulto pretraživanje, zaglavlje pretraživanja ili rezultat pretraživanja. 

- **has_contact_results** – jednostavna informacija o tome prikazuju li se rezultati kontakata u upitu za pretraživanje ili ne

- **include_deleted** – prikazuje li pretraživanje izbrisane mogućnosti među rezultatima pretraživanja 

- **is_ics_external_data** – bilježi je li dodani događaj interni (tj. dodan u program Outlook u kalendar programa Outlook) ili vanjski (tj. dodan iz druge aplikacije za e-poštu kao što je Gmail u kalendar programa Outlook).

- **is_network_fully_connected** – ovo služi tome da dobijete naznaku razloga za izvanmrežno pretraživanje. Ako je mreža povezana, a pretraživanje je izvan mreže, razlog je vjerojatno vremensko ograničenje poslužitelja

- **is_offline_search** – je li sesija pretraživanja ujedno pretraživanje izvan mreže na temelju rezultata pretraživanja koje vrati hx

- **re_enter_search_tab** – Booleova vrijednost za označavanje je li korisnik promijenio kartice prije odabira rezultata pretraživanja

- **result_selected_type** – s kojom vrstom podataka koji su bili prikazani korisnik komunicira, na primjer, prikaži sve kontakte, razgovore, događaje itd. 

- **search_conversation_result_data** – ovo sadrži podatke o označenom razgovoru iz rezultata pretraživanja uključujući vrstu računa (hx, ac itd.), drži li poruku servis u oblaku te je li prikazani pomak stranice jednaka stranica kao u prvoj poruci. 

- **search_origin** – podrijetlo pretraživanja, npr. glasovni pomoćnik, Cortana, unos tipkovnicom itd. 

- **search_scope** – niz koji označava u kojoj je vrsti računa korisnik provodio pretraživanje (na primjer, Exchange, Gmail itd.) ili je bila riječ o stavci Svi računi. 

- **search_suggestion_type** – označava što se nalazi iza prijedloga za pretraživanje, na primjer, je li riječ o ispravku pravopisa? Temelji li se na povijesti? Je li došlo do samodovršetka?

- **search_request_reason** – označava razlog zašto je zahtjev za pretraživanje poslan iz aplikacije, čime označava komponentu ili radnju korisnika koja je pokrenula pretraživanje.

- **search_result_filter_type** – označava koja je vrsta fltra primijenjena na pretraživanje, prikaži sve ili samo privitke

Sljedeća se polja prikupljaju na svim aplikacijama za iOS programa Outlook Mobile: 

- **action** – vrsta radnje koja je provedena za pretraživanje. Ovo prepoznaje je li pretraživanje pokrenuto, provodi li se ili je dovršeno te koje su se radnje provodile tijekom pretraživanja, na primjer, je li korišten mikrofon. Ovo je ključno za osiguravanje točnih i korisnih pretraživanja.

- **answer_result_selected_count** – prati koliko je puta pretraživanje bilo „uspješno”, na primjer, je li korisnik pronašao ono što je želio? Je li sastavljena e-pošta? Je li poruka označena knjižnom oznakom? 

- **contact_result_in_full_list_selected_count** – prati koliko je puta korisnik odabrao da se „prikažu svi kontakti” u punom popisu tijekom kombinirane sesije pretraživanja

- **contact_result_selected_count** – prati koliko je rezultata kontakata odabrano tijekom kombinirane sesije pretraživanja

- **conversation_result_selected_count** – prati koliko je razgovora označeno tijekom kombinirane sesije pretraživanja

- **mail_paging_gesture_count** – prati koliko je gesti listanja stranica za pretraživanje pošte izvršeno unutar kombinirane sesije pretraživanja

- **mail_requests_count** – prati koliko je zahtjeva za pretraživanje pošte poslano unutar kombinirane sesije pretraživanja

- **people_filter_selected_contacts_count** – prati koliko je kontakata odabrano u filtru za osobe

- **search_session_ended_type** – označava gdje je upit za pretraživanje završio jer je bio otkazan ili je upit bio ažuriran

- **search_suggestion_type** – označava što se nalazi iza prijedloga za pretraživanje, na primjer, je li riječ o ispravku pravopisa? Temelji li se na povijesti? Je li došlo do samodovršetka?

- **see_all_contacts_selected_count** – prati koliko je puta „prikaži sve kontakte” bilo odabrano tijekom kombinirane sesije pretraživanja

- **subtab_type** – prati gdje je korisnik odabrao rezultat i iz koje kartice rezultata

- **top_mail_result_selected_count** – prati koliko puta korisnik odabire glavne rezultate koji mu se pruže.

- **ui_reload_result_count** – bilježi vremena ponovnog učitavanja korisničkog sučelja zbog ažuriranja skupa rezultata (tijekom određenog upita)

- **ui_reload_result_time** – bilježi ukupno vrijeme utrošeno na ponovno učitavanje korisničkog sučelja zbog ažuriranja skupa rezultata (tijekom određenog upita)

- **ui_reload_status_count** – bilježi vremena ponovnog učitavanja korisničkog sučelja zbog ažuriranja statusa (tijekom određenog upita)

- **ui_reload_status_time** – bilježi ukupno vrijeme utrošeno na ponovno učitavanje korisničkog sučelja zbog ažuriranja statusa (tijekom određenog upita)

#### <a name="composemailaccessory"></a>compose.mail.accessory

Ovaj događaj omogućava nam prepoznavanje i popravljanje problema s ključnim radnjama sastavljanja poruka kako ne biste imali problema s prilaganjem datoteke, snimanjem fotografije kao privitka ili slanjem svoje raspoloživosti.

Prikupljaju se sljedeća polja: 

- **action** – govori nam radnju koja se pokušala provesti tijekom evidencije radnje. Neki primjeri uključuju prilaganje datoteke i prikaz većeg broja mogućnosti.

- **icon_name** – govori nam naziv ikone koja se prikazuje tijekom evidencije radnje.
 
- **origin** – otkriva nam porijeklo akcije. Moguće su vrijednosti quick_reply i full_screen.

- **toolbar_type** – Obavijestite nas o vrsti alatne trake koja se prikazuje na stranici za sastavljanje. Moguće su vrijednosti compose_actions i formatting.


#### <a name="conversationviewaction"></a>conversation.view.action

Koristi se za nadzor mogućeg negativnog utjecaja na vašu mogućnost prikaza i odgovaranja na poruke e-pošte

Prikupljaju se sljedeća polja:

- **contains_mention** – govori nam je li razgovor imao primijenjeno spominjanje @ kako bi nam pomogao prepoznati probleme sa spominjanjem u e-pošti

- **conversation_type** – govori nam koja je vrsta prikaza poruke e-pošte renderirana, primjerice prikaz jedne poruke ili prikazi većeg broja poruka. Pomaže nam prepoznati probleme povezane s određenim tipom poruke u našem prikazu razgovora e-pošte.

- **hx_error_type** – govori nam koja je pogreška dogodila uslugu koja je zabranila dovršavanje uklanjanja, ažuriranja ili dodavanja reakcije na poruku.

- **hx_string_tag** – govori nam oznaku pogreške u kodnoj bazi servisa.

- **reaction_origin** – govori nam izvor iz kojeg je korisnik reagirao 

- **reaction_type** – govori nam vrstu reakcije korisnika

- **suggested_reply_char_count** – govori nam koliko znakova predloženi odgovori koje nudimo (ako postoje) imaju kako bi nam pomogao prepoznati neobičnosti i probleme u vezi s našim prijedlozima

- **suggested_reply_click_pos** – govori nam na koji je položaj predloženi odgovor (ako postoji) prikazan kako bismo mogli prepoznati probleme s određenim prijedlogom

- **suggested_reply_type** – označava vrstu predloženog odgovora za tu akciju. Moguće su vrijednosti text, send_avail i create_meeting.

- **use_default_quick_reply_mode** – govori nam koji je zadani način za brzi odgovor korišten kako bi nam pomogao prepoznati probleme u vezi s doživljajem brzih odgovora za e-poštu

#### <a name="draftaction"></a>draft.action

Koristi se za nadzor mogućeg negativnog utjecaja na vašu mogućnost kreiranja i spremanja skica pošte.

Prikupljaju se sljedeća polja: 

- **action** – vrsta radnje, npr. spremi, odbaci.
 
- **draft_message_id** – ID poruke za skicu

- **is_groups** – šalje li se skica u/iz grupne mape
 
- **origin** – gdje je skica pokrenuta, npr. pojedinosti o poruci, sastavljanje.

- **smart_compose_model_version** – prati koja se verzija modela pametnog sastavljanja upotrebljava

- **suggestions_requested** – označava koliko ste modela pametnog sastavljanja tražili

- **suggestions_results** – rezultat prijedloga pametnog sastavljanja, tj. prihvaćeno, odbijeno

- **suggestions_returned** – označava koliko je prijedloga pametnog sastavljanja vraćeno s poslužitelja

- **suggestions_shown** – označava koliko je prijedloga pametnog sastavljanja prikazano korisniku
 
- **thread_id** – ID niti razgovora s kojim je skica povezana

#### <a name="draganddrop"></a>drag.and.drop

Ovaj nam događaj omogućuje prepoznavanje je li radnja povlačenja i ispuštanja bila uspješna ili ne.  To se koristi za osiguravanje da iskustva povlačenja i ispuštanja pravilno funkcioniraju u svim aplikacijama, kako kao događaj povlačenja u Outlook tako i kao događaj povlačenja koji izlazi izvan okvira programa Outlook.  Pomoću ovih podataka možemo osigurati da cjelovito iskustvo s drugim aplikacijama radi kako se očekivalo.

Prikupljaju se sljedeća polja: 

- **action** – radnja će biti povlačenje ili ispuštanje

- **location** – u slučaju radnje povlačenja, to će nam javiti s koje je lokacije korisnik započeo povlačenje.  U slučaju radnje ispuštanja, to će nam javiti gdje je korisnik ispustio datoteku koja se povlačila. 

- **source** – u slučaju radnje ispuštanja, to će nam javiti s koje je lokacije korisnik započeo povlačenje. To nam pomaže da bolje otkrijemo poteškoće s određenim izvorom kao što su OneDrive ili Datoteke u određeno mjesto za ispuštanje, kao što je nova poruka e-pošte.

#### <a name="drawerevent"></a>drawer.event

Koristi se za nadzor mogućeg negativnog utjecaja na vašu mogućnost pristupanja mapama u vašoj ulaznoj pošti

Prikupljaju se sljedeća polja:

- **add_calendar_option** – označava vrstu kalendara koji se dodaje iz ladice, odnosno, zanimljivi kalendar, kalendar pošte, dijeljeni kalendar, kako bi nam pomogao prepoznati probleme u vezi s određenim vrstama kalendara

- **calendar_accounts_count** – označava broj računa kalendara kako bi nam pomogao prepoznati probleme u vezi s brojem računa koji imate

- **calendar_apps_count** – označava broj aplikacija kalendara predstavljenih na uređaju korisnika kako bi nam pomogao prepoznati probleme u vezi s aplikacijama kalendara

- **drawer_type** – označava vrstu ladice: kalendar, pošta ili nulto pretraživanje kako bi nam pomogao prepoznati probleme u vezi s vrstom ladice

- **from_favorites** – označava je li radnja preuzeta iz favorita kako bi nam pomogao prepoznati probleme u vezi s favoritima

- **group_calendar_count** – Označava broj kalendara za račun koji će nam pomoći u otkrivanju problema povezanih s grupnim kalendarima

- **inbox_unread_count** – označava broj nepročitanih poruka u ulaznoj pošti kako bi nam pomogao prepoznati probleme s prikazivanjem količine nepročitanih poruka u ulaznoj pošti.

- **interesting_calendar_accounts_count** – označava broj računa koji ispunjavaju uvjete za zanimljive kalendare na uređaju kao bi nam pomogao prepoznati probleme u vezi sa zanimljivim kalendarima

- **is_group_calendar** – označava je li kalendar grupni kalendar kako bi nam pomogao prepoznati probleme u vezi s grupnim kalendarima

- **mail_folder_type** – označava vrstu mape pošte, npr. ulazna pošta, skice itd., kako bi nam pomogao prepoznati probleme u vezi s vrstama mapa.

- **mail_accounts_count** – označava broj računa pošte kako bi nam pomogao prepoznati probleme u vezi s računima pošte.

- **selected_group_calendar_count** – označava broj grupnih kalendara koji su odabrani i aktivni u korisničkom sučelju

- **visibility_toggle** – označava uključuje li korisnik ili isključuje određeni kalendar kako bi nam pomogao prepoznati probleme u vezi s prikazivanjem ili skrivanjem kalendara

#### <a name="ipccreaterepublishinglicense"></a>IpcCreateRepublishingLicense

Prikuplja se kada korisnik pokuša otvoriti dokument zaštićen IRM-om ili primijeniti zaštite IRM-a. Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada se stvori IpcCreateRepublishingLicense poziv API-ja.

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere

- **AppInfo.Name** – naziv aplikacije

- **AppInfo.Version** – verzija aplikacije

- **iKey** – identifikacijski broj poslužitelja pružatelja usluge zapisivanja

- **RMS.Duration** – ukupno vrijeme potrebno za dovršavanje poziva API-ja

- **RMS.DurationWithoutExternalOps** – ukupno vrijeme umanjeno za potrošene vanjske operacije poput latencije mreže.

- **RMS.ErrorCode** – kod pogreške koji, ako postoji, vraća poziv API-ja

- **RMS.HttpCall** – označava postoji li operacija HTTP-a

- **RMS.Result** – uspjeh ili neuspjeh poziva API-ja

- **RMS.ScenarioId** – identifikacijski broj scenarija definiran API-jem

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

- **RMS.StatusCode** – kod statusa vraćenog rezultata

#### <a name="ipcgetlicenseproperty"></a>IpcGetLicenseProperty

Prikuplja se kada korisnik pokuša otvoriti dokument zaštićen IRM-om ili primijeniti zaštite IRM-a. Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada se stvori IpcGetLicenseProperty poziv API-ja.

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere

- **AppInfo.Name** – naziv aplikacije.

- **AppInfo.Version** – verzija aplikacije

- **iKey** – identifikacijski broj poslužitelja pružatelja usluge zapisivanja

- **RMS.Duration** – ukupno vrijeme potrebno za dovršavanje poziva API-ja

- **RMS.DurationWithoutExternalOps** – ukupno vrijeme umanjeno za potrošene vanjske operacije poput latencije mreže.

- **RMS.ErrorCode** – kod pogreške koji, ako postoji, vraća poziv API-ja

- **RMS.HttpCall** – označava postoji li operacija HTTP-a

- **RMS.LicensePropertyType** – vrsta svojstva licence

- **RMS.Result** – uspjeh ili neuspjeh poziva API-ja

- **RMS.ScenarioId** – identifikacijski broj scenarija definiran API-jem

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

- **RMS.StatusCode** – kod statusa vraćenog rezultata

#### <a name="ipcgetserializedlicenseproperty"></a>IpcGetSerializedLicenseProperty

Prikuplja se kada korisnik pokuša otvoriti dokument zaštićen IRM-om ili primijeniti zaštite IRM-a. Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada se stvori IpcGetSerializedLicenseProperty poziv API-ja.

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere

- **AppInfo.Name** – naziv aplikacije.

- **AppInfo.Version** – verzija aplikacije

- **iKey** – identifikacijski broj poslužitelja pružatelja usluge zapisivanja

- **RMS.Duration** – ukupno vrijeme potrebno za dovršavanje poziva API-ja

- **RMS.DurationWithoutExternalOps** – ukupno vrijeme umanjeno za potrošene vanjske operacije poput latencije mreže.

- **RMS.ErrorCode** – kod pogreške koji, ako postoji, vraća poziv API-ja

- **RMS.HttpCall** – označava postoji li operacija HTTP-a

- **RMS.LicensePropertyType** – vrsta svojstva licence

- **RMS.Result** – uspjeh ili neuspjeh poziva API-ja

- **RMS.ScenarioId** – identifikacijski broj scenarija definiran API-jem

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

- **RMS.StatusCode** – kod statusa vraćenog rezultata

#### <a name="ipcgettemplateissuerlist"></a>IpcGetTemplateIssuerList

Prikuplja se kada korisnik pokuša otvoriti dokument zaštićen IRM-om ili primijeniti zaštite IRM-a. Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada se stvori IpcGetTemplateIssuerList poziv API-ja.

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere

- **AppInfo.Name** – naziv aplikacije.

- **AppInfo.Version** – verzija aplikacije

- **iKey** – identifikacijski broj poslužitelja pružatelja usluge zapisivanja

- **RMS.AuthCallbackProvided** – označava pruža li se povratni poziv za provjeru autentičnosti kao unos poziva API-ja ili ne

- **RMS.ConnectionInfo.ExtranetUrl** – URL ekstraneta za informacije o vezi

- **RMS.ConnectionInfo.IntranetUrl** – URL intraneta za informacije o vezi

- **RMS.ConnectionMode** – način povezivanja između klijenta usluge upravljanja pravima i poslužitelja: na mreži ili izvan mreže

- **RMS.Duration** – ukupno vrijeme potrebno za dovršavanje poziva API-ja

- **RMS.DurationWithoutExternalOps** – ukupno vrijeme umanjeno za potrošene vanjske operacije poput latencije mreže.

- **RMS.ErrorCode** – kod pogreške koji, ako postoji, vraća poziv API-ja

- **RMS.GuestTenant** – identifikacijski broj klijenta gosta za korisnika

- **RMS.HomeTenant** – identifikacijski broj početnog klijenta za korisnika

- **RMS.HttpCall** – označava postoji li operacija HTTP-a

- **RMS.Identity.ExtranetUrl** – URL ekstraneta poslužitelja usluge upravljanja pravima za korisnika koji se prikuplja tijekom dobivanja novog certifikata za račun prava s poslužitelja
 
- **RMS.Identity.IntranetUrl** – URL intraneta poslužitelja usluge upravljanja pravima za korisnika koji se prikuplja tijekom dobivanja novog certifikata za račun prava s poslužitelja

- **RMS.Identity.Status** – prvi put dobivanja certifikata za račun prava s poslužitelja ili obnavljanja certifikata za račun prava 

- **RMS.Identity.Type** – vrsta korisničkog računa kao što je račun za Windows ili račun za Live

- **RMS.Identity.UserProvided** – označava je li adresa e-pošte korisnika pružena ili nije tijekom dobivanja novog certifikata za račun prava s poslužitelja

- **RMS.IssuerId** – identifikacijski broj poslužitelja usluge upravljanja pravima koji izdaje certifikat za račun prava 

- **RMS.LicenseFormat** – format licence: Xrml ili Json

- **RMS.RACType** – vrsta certifikata za račun prava

- **RMS.Result** – uspjeh ili neuspjeh poziva API-ja

- **RMS.ScenarioId** – identifikacijski broj scenarija definiran API-jem

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

- **RMS.ServerType** – vrsta poslužitelja usluge upravljanja pravima

- **RMS.StatusCode** – kod statusa vraćenog rezultata

- **UserInfo.UserObjectId** – identifikacijski broj objekta korisnika

#### <a name="ipcgettemplatelist"></a>IpcGetTemplateList

Prikuplja se kada korisnik pokuša otvoriti dokument zaštićen IRM-om ili primijeniti zaštite IRM-a. Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada se stvori IpcGetTemplateList poziv API-ja.

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere

- **AppInfo.Name** – naziv aplikacije.

- **AppInfo.Version** – verzija aplikacije

- **iKey** – identifikacijski broj poslužitelja pružatelja usluge zapisivanja

- **RMS.AuthCallbackProvided** – označava pruža li se povratni poziv za provjeru autentičnosti kao unos poziva API-ja ili ne

- **RMS.ConnectionInfo.ExtranetUrl** – URL ekstraneta za informacije o vezi

- **RMS.ConnectionInfo.IntranetUrl** – URL intraneta za informacije o vezi

- **RMS.ConnectionMode** – način povezivanja između klijenta usluge upravljanja pravima i poslužitelja: na mreži ili izvan mreže

- **RMS.Duration** – ukupno vrijeme potrebno za dovršavanje poziva API-ja

- **RMS.DurationWithoutExternalOps** – ukupno vrijeme umanjeno za potrošene vanjske operacije poput latencije mreže.

- **RMS.ErrorCode** – kod pogreške koji, ako postoji, vraća poziv API-ja

- **RMS.GuestTenant** – identifikacijski broj klijenta gosta za korisnika

- **RMS.HomeTenant** – identifikacijski broj početnog klijenta za korisnika

- **RMS.HttpCall** – označava postoji li operacija HTTP-a

- **RMS.Identity.ExtranetUrl** – URL ekstraneta poslužitelja usluge upravljanja pravima za korisnika koji se prikuplja tijekom dobivanja novog certifikata za račun prava s poslužitelja
 
- **RMS.Identity.IntranetUrl** – URL intraneta poslužitelja usluge upravljanja pravima za korisnika koji se prikuplja tijekom dobivanja novog certifikata za račun prava s poslužitelja

- **RMS.Identity.Status** – prvi put dobivanja certifikata za račun prava s poslužitelja ili obnavljanja certifikata za račun prava 

- **RMS.Identity.Type** – vrsta korisničkog računa kao što je račun za Windows ili račun za Live

- **RMS.Identity.UserProvided** – označava je li adresa e-pošte korisnika pružena ili nije tijekom dobivanja novog certifikata za račun prava s poslužitelja

- **RMS.IssuerId** – identifikacijski broj poslužitelja usluge upravljanja pravima koji izdaje certifikat za račun prava 

- **RMS.LicenseFormat** – format licence: Xrml ili Json

- **RMS.RACType** – vrsta certifikata za račun prava

- **RMS.Result** – uspjeh ili neuspjeh poziva API-ja

- **RMS.ScenarioId** – identifikacijski broj scenarija definiran API-jem

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

- **RMS.ServerType** – vrsta poslužitelja usluge upravljanja pravima

- **RMS.StatusCode** – kod statusa vraćenog rezultata

- **RMS.TemplatesCount** – broj predložaka

- **UserInfo.UserObjectId** – identifikacijski broj objekta korisnika

#### <a name="ipcpcreatelicensefromscratch"></a>IpcpCreateLicenseFromScratch

Prikuplja se kada korisnik pokuša otvoriti dokument zaštićen IRM-om ili primijeniti zaštite IRM-a. Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada se stvori IpcpCreateLicenseFromScratch poziv API-ja.

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere

- **AppInfo.Name** – naziv aplikacije.

- **AppInfo.Version** – verzija aplikacije

- **iKey** – identifikacijski broj poslužitelja pružatelja usluge zapisivanja

- **RMS.Duration** – ukupno vrijeme potrebno za dovršavanje poziva API-ja

- **RMS.DurationWithoutExternalOps** – ukupno vrijeme umanjeno za potrošene vanjske operacije poput latencije mreže.

- **RMS.ErrorCode** – kod pogreške koji, ako postoji, vraća poziv API-ja

- **RMS.GuestTenant** – identifikacijski broj klijenta gosta za korisnika

- **RMS.HomeTenant** – identifikacijski broj početnog klijenta za korisnika

- **RMS.HttpCall** – označava postoji li operacija HTTP-a

- **RMS.Identity.ExtranetUrl** – URL ekstraneta poslužitelja usluge upravljanja pravima za korisnika koji se prikuplja tijekom dobivanja novog certifikata za račun prava s poslužitelja

- **RMS.Identity.IntranetUrl** – URL intraneta poslužitelja usluge upravljanja pravima za korisnika koji se prikuplja tijekom dobivanja novog certifikata za račun prava s poslužitelja

- **RMS.Identity.UserProvided** – označava je li adresa e-pošte korisnika pružena ili nije tijekom dobivanja novog certifikata za račun prava s poslužitelja

- **RMS.IssuerId** – identifikacijski broj poslužitelja usluge upravljanja pravima koji izdaje certifikat za račun prava 

- **RMS.LicenseFormat** – format licence: Xrml ili Json

- **RMS.RACType** – vrsta certifikata za račun prava

- **RMS.Result** – uspjeh ili neuspjeh poziva API-ja

- **RMS.ScenarioId** – identifikacijski broj scenarija definiran API-jem

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

- **RMS.ServerType** – vrsta poslužitelja usluge upravljanja pravima

- **RMS.StatusCode** – kod statusa vraćenog rezultata

- **RMS.TokenProvided** – označava je li token pružen kao unos poziva API-ja ili ne 

- **RMS.UserProvided** – označava je li korisnik pružen kao unos poziva API-ja ili ne 

- **UserInfo.UserObjectId** – identifikacijski broj objekta korisnika 

#### <a name="ipcpcreatelicensefromtemplate"></a>IpcpCreateLicenseFromTemplate

Prikuplja se kada korisnik pokuša otvoriti dokument zaštićen IRM-om ili primijeniti zaštite IRM-a. Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada se stvori IpcpCreateLicenseFromTemplate poziv API-ja. 

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere

- **AppInfo.Name** – naziv aplikacije.

- **AppInfo.Version** – verzija aplikacije

- **iKey** – identifikacijski broj poslužitelja pružatelja usluge zapisivanja

- **RMS.AuthCallbackProvided** – označava pruža li se povratni poziv za provjeru autentičnosti kao unos poziva API-ja ili ne

- **RMS.ConnectionMode** – način povezivanja između klijenta usluge upravljanja pravima i poslužitelja: na mreži ili izvan mreže

- **RMS.Duration** – ukupno vrijeme potrebno za dovršavanje poziva API-ja

- **RMS.DurationWithoutExternalOps** – ukupno vrijeme umanjeno za potrošene vanjske operacije poput latencije mreže.

- **RMS.ErrorCode** – kod pogreške koji, ako postoji, vraća poziv API-ja

- **RMS.HttpCall** – označava postoji li operacija HTTP-a

- **RMS.Result** – uspjeh ili neuspjeh poziva API-ja

- **RMS.ScenarioId** – identifikacijski broj scenarija definiran API-jem

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

- **RMS.StatusCode** – kod statusa vraćenog rezultata

- **RMS.TokenProvided** – označava je li token pružen kao unos poziva API-ja ili ne 

- **RMS.UserProvided** – označava je li korisnik pružen kao unos poziva API-ja ili ne 

#### <a name="ipcpgettemplatelistforuser"></a>IpcpGetTemplateListForUser

Prikuplja se kada korisnik pokuša otvoriti dokument zaštićen IRM-om ili primijeniti zaštite IRM-a. Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada se stvori IpcpGetTemplateListForUser poziv API-ja. 

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere

- **AppInfo.Name** – naziv aplikacije.

- **AppInfo.Version** – verzija aplikacije

- **iKey** – identifikacijski broj poslužitelja pružatelja usluge zapisivanja

- **RMS.ApplicationScenarioId** – identifikacijski broj scenarija koji pruža aplikacija

- **RMS.AuthCallbackProvided** – označava pruža li se povratni poziv za provjeru autentičnosti kao unos poziva API-ja ili ne

- **RMS.ConnectionInfo.ExtranetUrl** – URL ekstraneta za informacije o vezi

- **RMS.ConnectionInfo.IntranetUrl** – URL intraneta za informacije o vezi

- **RMS.ConnectionMode** – način povezivanja između klijenta usluge upravljanja pravima i poslužitelja: na mreži ili izvan mreže

- **RMS.Duration** – ukupno vrijeme potrebno za dovršavanje poziva API-ja

- **RMS.DurationWithoutExternalOps** – ukupno vrijeme umanjeno za potrošene vanjske operacije poput latencije mreže.

- **RMS.ErrorCode** – kod pogreške koji, ako postoji, vraća poziv API-ja

- **RMS.GuestTenant** – identifikacijski broj klijenta gosta za korisnika

- **RMS.HomeTenant** – identifikacijski broj početnog klijenta za korisnika

- **RMS.HttpCall** – označava postoji li operacija HTTP-a

- **RMS.Identity.ExtranetUrl** – URL ekstraneta poslužitelja usluge upravljanja pravima za korisnika koji se prikuplja tijekom dobivanja novog certifikata za račun prava s poslužitelja

- **RMS.Identity.IntranetUrl** – URL intraneta poslužitelja usluge upravljanja pravima za korisnika koji se prikuplja tijekom dobivanja novog certifikata za račun prava s poslužitelja

- **RMS.Identity.Status** – prvi put dobivanja certifikata za račun prava s poslužitelja ili obnavljanja certifikata za račun prava 

- **RMS.Identity.Type** – vrsta korisničkog računa kao što je račun za Windows ili račun za Live

- **RMS.Identity.UserProvided** – označava je li adresa e-pošte korisnika pružena ili nije tijekom dobivanja novog certifikata za račun prava s poslužitelja

- **RMS.IssuerId** – identifikacijski broj poslužitelja usluge upravljanja pravima koji izdaje certifikat za račun prava 

- **RMS.LicenseFormat** – format licence: Xrml ili Json

- **RMS.RACType** – vrsta certifikata za račun prava

- **RMS.Result** – uspjeh ili neuspjeh poziva API-ja

- **RMS.ScenarioId** – identifikacijski broj scenarija definiran API-jem

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

- **RMS.ServerType** – vrsta poslužitelja usluge upravljanja pravima

- **RMS.StatusCode** – kod statusa vraćenog rezultata

- **RMS.TemplatesCount** – broj predložaka

- **RMS.TokenProvided** – označava je li token pružen kao unos poziva API-ja ili ne 
    
- **RMS.UserProvided** – označava je li korisnik pružen kao unos poziva API-ja ili ne 

- **UserInfo.UserObjectId** – identifikacijski broj objekta korisnika 

#### <a name="ipcpserializelicense"></a>IpcpSerializeLicense

Prikuplja se kada korisnik pokuša primijeniti zaštite IRM-a na dokument. Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada se stvori IpcpSerializeLicense poziv API-ja.

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere

- **AppInfo.Name** – naziv aplikacije.

- **AppInfo.Version** – verzija aplikacije

- **iKey** – identifikacijski broj poslužitelja pružatelja usluge zapisivanja

- **RMS.ApplicationScenarioId** – identifikacijski broj scenarija koji pruža aplikacija

- **RMS.AuthCallbackProvided** – označava pruža li se povratni poziv za provjeru autentičnosti kao unos poziva API-ja ili ne

- **RMS.ConnectionMode** – način povezivanja između klijenta usluge upravljanja pravima i poslužitelja: na mreži ili izvan mreže

- **RMS.ContentId** – identifikacijski broj sadržaja dokumenta

- **RMS.Duration** – ukupno vrijeme potrebno za dovršavanje poziva API-ja

- **RMS.DurationWithoutExternalOps** – ukupno vrijeme umanjeno za potrošene vanjske operacije poput latencije mreže.

- **RMS.ErrorCode** – kod pogreške koji, ako postoji, vraća poziv API-ja

- **RMS.GuestTenant** – identifikacijski broj klijenta gosta za korisnika

- **RMS.HomeTenant** – identifikacijski broj početnog klijenta za korisnika

- **RMS.HttpCall** – označava postoji li operacija HTTP-a

- **RMS.Identity.ExtranetUrl** – URL ekstraneta poslužitelja usluge upravljanja pravima za korisnika koji se prikuplja tijekom dobivanja novog certifikata za račun prava s poslužitelja

- **RMS.Identity.IntranetUrl** – URL intraneta poslužitelja usluge upravljanja pravima za korisnika koji se prikuplja tijekom dobivanja novog certifikata za račun prava s poslužitelja

- **RMS.Identity.Status** – prvi put dobivanja certifikata za račun prava s poslužitelja ili obnavljanja certifikata za račun prava 

- **RMS.Identity.Type** – vrsta korisničkog računa kao što je račun za Windows ili račun za Live

- **RMS.Identity.UserProvided** – označava je li adresa e-pošte korisnika pružena ili nije tijekom dobivanja novog certifikata za račun prava s poslužitelja

- **RMS.IssuerId** – identifikacijski broj poslužitelja usluge upravljanja pravima koji izdaje certifikat za račun prava 

- **RMS.KeyHandle** – adresa memorije ručice ključa

- **RMS.LicenseFormat** – format licence: Xrml ili Json

- **RMS.PL.KeyType** – vrijednosti „jedno” ili „dvostruko”. Označava je li PL bio zaštićen zaštitom s jednim ključem ili zaštitom s dvostrukim ključevima.

- **RMS.RACType** – vrsta certifikata za račun prava

- **RMS.Result** – uspjeh ili neuspjeh poziva API-ja

- **RMS.ScenarioId** – identifikacijski broj scenarija definiran API-jem

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

- **RMS.ServerType** – vrsta poslužitelja usluge upravljanja pravima

- **RMS.StatusCode** – kod statusa vraćenog rezultata

- **RMS.TokenProvided** – označava je li token pružen kao unos poziva API-ja ili ne 

- **RMS.UserProvided** – označava je li korisnik pružen kao unos poziva API-ja ili ne 

- **UserInfo.UserObjectId** – identifikacijski broj objekta korisnika 

#### <a name="ipcsetlicenseproperty"></a>IpcSetLicenseProperty

Prikuplja se kada korisnik pokuša otvoriti dokument zaštićen IRM-om ili primijeniti zaštite IRM-a. Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada se stvori IpcSetLicenseProperty poziv API-ja. 

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere

- **AppInfo.Name** – naziv aplikacije.

- **AppInfo.Version** – verzija aplikacije

- **iKey** – identifikacijski broj poslužitelja pružatelja usluge zapisivanja

- **RMS.Duration** – ukupno vrijeme potrebno za dovršavanje poziva API-ja

- **RMS.DurationWithoutExternalOps** – ukupno vrijeme umanjeno za potrošene vanjske operacije poput latencije mreže.

- **RMS.ErrorCode** – kod pogreške koji, ako postoji, vraća poziv API-ja 

- **RMS.HttpCall** – označava postoji li operacija HTTP-a

- **RMS.LicensePropertyType** – vrsta svojstva licence

- **RMS.Result** – uspjeh ili neuspjeh poziva API-ja

- **RMS.ScenarioId** – identifikacijski broj scenarija definiran API-jem

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

- **RMS.StatusCode** – ID scenarija koji je definirao API


#### <a name="linkclickedaction"></a>link.clicked.action

Taj se događaj upotrebljava za praćenje uspjeha korisnika prilikom pregledavanja URL-a u web-prikazu preglednika Edge i dovršavanja standardnih web scenarija u tom web-prikazu, bez suočavanja s pogreškama

Prikupljaju se sljedeća polja:

- **account_type** – ako je web-prikaz pokrenut iz poruke e-pošte ili događaja u programu Outlook, vrsta računa odakle je URL došao

- **action** – radnja koju provodi korisnik u programu Outlook od trenutka kada dodirnu URL do trenutka kada izađu iz tog tijeka (otvorili su vezu u web-prikazu preglednika Edge, neuspjelo učitavanje stranice u web-prikazu, provedeno pretraživanje u web-prikazu, izlaz iz web-prikaza preglednika Edge radi otvaranja veze u aplikaciji web-preglednika itd.)

- **duration** – trajanje sesije korisnika

- **launch_type** – ako je web-prikaz pokrenut u pregledniku Edge, je li pokrenut iz programa Outlook, iz widgeta ili iz komponente OS-a

- **origin** – ako je korisnik izveo radnju u web-prikazu preglednika Edge, izvor te radnje

- **referrer** – mjesto URL-a koje je korisnik dodirnuo (e-pošta, događaj u kalendaru, TXP kartica itd.)

- **search_scope** – ako je korisnik pretraživao u web-prikazu preglednika Edge, opseg tog pretraživanja (Sve, Slike, Videozapisi itd.)

- **search_subtype** – ako je korisnik pretražio u web-prikazu preglednika Edge, je li to bili izvorno pretraživanje ili suženo pretraživanje.

- **session_summary_page_loaded_count** – broj stranica koje je korisnik učitao tijekom sesije u web-prikazu preglednika Edge

- **session_summary_page_loaded_count** – broj Bing pretraživanja koje je korisnik proveo tijekom sesije u web-prikazu preglednika Edge

- **session_summary_session_id** – identifikator trenutačne sesije korisnika u web-prikazu preglednika Edge

- **txp** – ako je web-prikaz preglednika Edge pokrenut iz TXP kartice, vrste događaja za tu karticu (blagovanje, let itd.)

- **txp_component** – ako je web-prikaz preglednika Edge pokrenut s TXP kartice, vrsta komponente korisničkog sučelja za tu karticu


#### <a name="mailaction"></a>mail.action

Koristi se za nadzor mogućeg negativnog utjecaja na vašu mogućnost provedbe ključnih radnji za poštu (poput pokretanja načina poruka u obliku niti, osiguravanja funkcije razvrstavanja pošte) kako bi se osiguralo da naša propisno funkcionira za poštu.

Prikupljaju se sljedeća polja:

- **account** – račun u okviru kojeg se provela radnja *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

- **action** – prati vrstu radnje koja se provela, tj. arhiviranje, brisanje, označavanje kao pročitano itd. 

- **attachment_content_type** – vrsta sadržaja preuzetog privitka 

- **attachment_content_type_with_count** – prati broj privitaka u poruci e-pošte

- **attachment_download_result** – rezultat (tj. uspjeh/neuspjeh) za radnju preuzimanja privitka

- **attachment_download_time** – trajanje radnje preuzimanja privitka

- **attachment_extn** – datotečni nastavak preuzetog privitka *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

- **attachment_id** – identifikator sustava za preuzeti privitak 

- **attachment_size** – veličina preuzetog privitka

- **domain** – domena dokumenta koji se otvara

- **duration** – prati koliko je radnja trajala kao čovjeku razumljivi niz na engleskom jeziku (npr. 1s, 4h)

- **error** – poruka o pogrešci povezanoj s radnjom 

- **event_mode** – u kojem je načinu događaja radnja bila, grupama ili ostalo. 

- **Extension** – četiri znaka proširenja datoteke veze ili privitka povezanih s tom akcijom  *[Ovo je polje uklonjeno iz aktualnih međuverzija sustava Office, ali i dalje će se prikazivati u starijim međuverzijama.]*

- **internet_message_id** – ID poruke o praćenju

- **is_group_escalation** – označava je li poruka ili radnja provedena u ili je poslana na korisnikov poštanski sandučić zbog eskalacije (pretplata na grupu)

- **is_rule** – označava vraća li provedena radnja za poštu fokusiranu/drugu klasifikaciju na izvorne postavke

- **is_threaded_mode** – označava je li poruka bila u obliku niti ili nije, tj. kako su poruke grupirane

- **is_unread** – označava je li poruka o tome da je radnja provedena nepročitana

- **left_swipe_setting** – označava koja je radnja postavljena kao radnja pokrenuta prelaskom prstom ulijevo

- **message_id** – ID poruke poslužitelja s ciljem za radnju ili popis odvojen zarezom ako je radnja provedena s više stavki od jedne.

- **message_type** – označava na kojoj je vrsti poruke radnja provedena** – grupne ili druge

- **number_selected** – broj stavki koje je korisnik odabrao na popisu poruka i poduzeo radnju tijekom višestrukog odabira.

- **origin** – izvor radnje, tj. prelazak prstom na mobilnom telefonu, nulti upit, dubinska veza, prikaz e-pošte, popis e-pošte itd.

- **origin_view** – izvorišni prikaz akcija, na primjer, razgovor, poruka itd.

- **reported_to_msft** – nakon slanja e-pošte u bezvrijednu poštu (neželjenu poštu) ili smeće (krađa identiteta) može se odabrati prijavljivanje radnje Microsoftu.

- **retry** – je li se radnja pokušala ponovno provesti

- **right_swipe_setting** – označava koja je radnja postavljena kao radnja pokrenuta prelaskom prstom udesno 

- **shortcut** – označava je li korišten prečac te koji je prečac korišten za zakazivanje poruke, odnosno, kasnije, sutra, odabir vremena itd.

- **size** – veličina veze ili privitka povezanog s ovom radnjom

- **source_folder** – prati vrstu izvorišne mape kada radnja upućuje na premještanje iz jedne mape u drugu, tj. u ulaznu poštu, smeće itd. 

- **source_inbox** – označava u kojoj se ulaznoj pošti radnja za poštu provodi (odnosno fokusirana, drugo itd.) state – stanje radnje, odnosno, točka uspjeha ili neuspjeha

- **state** – stanje radnje, tj. točka uspjeha ili točka neuspjeha

- **target_folder** – označava vrstu odredišne mape tijekom premještanja poruka e-pošte iz jedne mape u drugu

- **thread_id** – ID niti razgovora ciljanog za akciju ili popisa odvojenog zarezom ako je ciljano više od jedne stavke

- **time_taken_to_fetch_access_token** – vrijeme potrebno za dohvaćanje tokena za pristup sustavu koji se koristi za otvaranje veze

- **time_taken_to_fetch_drive_item** – vrijeme potrebno za dohvaćanje resursa servisa OneDrive kada se klikne

- **time_taken_to_fetch_embed_viewer_resource** – vrijeme potrebno za pokretanje ugrađenog preglednika tijekom otvaranja veza

- **time_taken_to_load_embed_viewer** – vrijeme potrebno za pokretanje ugrađenog preglednika tijekom otvaranja veza

- **time_taken_to_load_link** – vrijeme potrebno za dovršavanje radnje učitavanja veze

- **time_taken_to_tap_attachment** – vrijeme između otvaranja poruke i klika na privitak

- **time_taken_to_tap_link** – vrijeme koje je korisniku bilo potrebno između pregleda poruke i klika na vezu

- **txp** – označava postoji li stavka vrste txp povezana s poštom na kojoj je ta radnja provedena, odnosno, rezervacija događaja, rezervacija leta itd. 

- **type** – vrsta dokumenta koji se otvara putem veze

#### <a name="mailcompose"></a>mail.compose

Koristi se za nadzor mogućeg negativnog utjecaja na vašu mogućnost sastavljanja i odgovaranja na poruke e-pošte, na primjer nailaženje na probleme s odgovaranjem svima, formatiranjem vaših poruka e-pošte ili slanjem vaših poruka e-pošte.

Prikupljaju se sljedeća polja: 

- **draft_message_id** – ID skice razgovora koji se stvara kao skica kako bi nam pomogao prepoznati probleme u vezi sa skicama poruka e-pošte

- **message_id** – ID poruke razgovora na koji se odgovara ili iz kojeg se prosljeđuje kako bi nam pomogao prepoznati probleme u vezi s određenom porukom

- **origin** – govori nam o podrijetlu poruke, primjerice kao odgovaranje svima, kreiranje nove poruke ili brzi odgovor. Pomaže nam prepoznati probleme u vezi s određenom vrstom podrijetla odgovora.

- **is_group_escalation** – govori nam je li poruka eskalirana grupna poruka kako bismo mogli prepoznati probleme sa sastavljanjem povezane s grupama.

- **is_link** – govori nam je li se stvaranje nove skice provelo iz veze. Pomaže nam prepoznati probleme u vezi sa skicama stvorenim iz veza.

- **is_force_touch** – govori nam je li se stvaranje nove skice provelo iz radnje prisilnog dodira. Pomaže nam prepoznati probleme u vezi sa skicama stvorenim iz ove specifične radnje.

- **is_groups** – je li događaj pokrenut iz prostora grupe kako bismo mogli prepoznati probleme sa sastavljanjem u vezi s grupama.

- **source_inbox** – govori nam koja je izvorna ulazna pošta, primjerice je li to bila fokusirana ili druga ulazna pošta

- **thread_id** – ID niti razgovora na koji se odgovara ili iz kojeg se prosljeđuje kako bi nam pomogao prepoznati probleme u vezi s određenim nizom

#### <a name="meetingcalltoaction"></a>meeting.call.to.action

Koristi se za nadzor mogućeg negativnog utjecaja na vašu mogućnost provedbe ključnih radnji sastanka kao što su kreiranje, uređivanje i odgovaranje na sastanke.

Prikupljaju se sljedeća polja:

- **event_mode** – označava potječe li ovaj događaj iz grupe ili ne kako bi nam pomogao prepoznati probleme u vezi s grupnim događajima

- **meeting_id** – ID sastanka koji nam pomaže pratiti probleme tijekom cijelog trajanja sastanka kako bi nam pomogao prepoznati probleme u vezi s određenim sastancima

- **meeting_provider** – označava davatelja usluga za mrežni sastanak, na primjer, Teams, Skype za tvrtke, kako bi nam pomogao prepoznati probleme u vezi s određenim davateljima usluga mrežnih sastanaka

- **notify_type** – označava vrstu odgovora za druge vrste računa kako bi nam pomogao prepoznati probleme u vezi s različitim vrstama računa

- **recurrence** – označava koliko se često ovaj sastanak održava, odnosno, jedanput ili niz, kako bi nam pomogao prepoznati probleme u vezi s nizovima ponavljajućih sastanaka

- **response** – označava vrstu odgovora kao što je prihvaćanje ili odbijanje na određenim vrstama računa kako bi nam pomogao prepoznati probleme u vezi s odgovaranjem na događaje

- **response_message_length** – označava duljinu poruke kako bi nam pomogao prepoznati probleme u vezi s odgovorima na sastanak

- **review_time_proposal_action_type** – označava odgovor korisnika za predlaganje novog vremena kako bi nam pomogao prepoznati probleme u vezi s predlaganjem novog vremena

- **send_response** – označava je li odgovor poslan kako bi nam pomogao prepoznati probleme u vezi sa slanjem odgovora na pozivnice na sastanak

- **txp** – označava iz koje je vrste sastanka stvoren, npr. rezervacije letova i isporuke, kako bi nam mogao prepoznati probleme u vezi s ovom vrstom sastanka

- **with_message_enabled** – označava može li korisnik odgovoriti porukom kako bi nam pomogao prepoznati probleme u vezi s odgovaranjem na pozivnice na sastanak

#### <a name="officeandroiddocsuifileoperationsopendocumentmeasurements"></a>Office.Android.DocsUI.FileOperations.OpenDocumentMeasurements

Ovaj se događaj prikuplja za aplikacije sustava Office koje se pokreću na platformi Android i evidentira kada se provodi radnja otvaranja datoteke. Događaj pomaže jamčiti da je radnja otvaranja datoteke sigurna, ažurna i da se pravilno provodi. Cilj prikupljanja ovih podataka jest kontinuirano poboljšanje funkcije otvaranja datoteke. 

Prikupljaju se sljedeća polja:

- **Data_AppDocsOperationDuration** – trajanje podsloja tijekom radnje otvaranja datoteke.

- **Data_AppDuration** – trajanje obrade aplikacije tijekom radnje otvaranja datoteke. 

- **Data_AppWarmUpGain** – dobitak ostvaren u trajanju pokretanja aplikacije zbog prethodnog pokretanja dijela aplikacije.

- **Data_BootDuration** – trajanje pokretanja aplikacije tijekom radnje otvaranja datoteke.

- **Data_BootMarkers** – vrijednost niza koja evidentira trajanje vremena između nekih poziva funkcije tijekom pokretanja aplikacije, u obliku s ID-om i trajanjem funkcije.

- **Data_ClosePreviouslyOpenedMarkers** – u nekim se scenarijima otvaranja datoteka zatvaranje prethodno otvorenog dokumenta odvija prije otvaranja trenutačnog dokumenta. Trajanje razdoblja između nekih operacija koje se odvijaju u tom slučaju bilježe se u vrijednosti niza koja ima oblik \<functionId>\<functionValue>\<functionId>\<functionValue>...

- **Data_Doc_AccessMode** – enumeracija koja upućuje na način pristupa datoteke, na primjer, samo za čitanje, za čitanje i pisanje.

- **Data_Doc_AsyncOpenKind** – enumeracija koja upućuje na vrstu asinkronog toka koji se koristi za otvaranje datoteke.

- **Data_Doc_ChunkingType** – enumeracija koja upućuje na vrstu algoritma dijeljenja datoteke.

- **Data_Doc_EdpState** – enumeracija koja upućuje na stanje korporacijske zaštite podataka datoteke.

- **Data_Doc_Ext** – Datotečni nastavak datoteke.

- **Data_Doc_Fqdn** – naziv glavnog računala poslužitelja datoteke.

- **Data_Doc_FqdnHash** – globalno jedinstveni identifikator (GUID) koji jedinstveno identificira naziv glavnog računala poslužitelja.

- **Data_Doc_IdentityTelemetryId** – GUID koji jedinstveno identificira identitet koji se koristi za otvaranje datoteke. 

- **Data_Doc_InitializationScenario** – enumeracija koja upućuje na detaljnu vrstu scenarija otvaranja datoteke.

- **Data_Doc_IOFlags** – enumeracija koja označava zastavice UI operacije otvaranja datoteke, na primjer, ako je datoteka predmemorirana ili ne.

- **Data_Doc_IsCloudCollabEnabled**– bez obzira na to je li za datoteku omogućena suradnja u oblaku.

- **Data_Doc_IsIncrementalOpen** – bez obzira na to je li datoteka otvorena inkrementalno ili ne.

- **Data_Doc_IsOcsSupported** – bez obzira na to podržava li datoteka uslugu suradnje u sustavu Office.

- **Data_Doc_IsOpeningOfflineCopy** – bez obzira na to je li datoteka otvorena iz izvanmrežne predmemorirane kopije.

- **Data_Doc_IsPrefetched** – bez obzira na to je li datoteka unaprijed dohvaćena prije operacije otvaranja.

- **Data_Doc_IsSyncBacked** – bez obzira na to postoji li datoteka oblaka lokalno i je li sinkronizirana s poslužiteljem.

- **Data_Doc_Location** – enumeracija koja upućuje gdje se datoteka nalazi, na primjer, lokalno ili u oblaku.

- **Data_Doc_ReadOnlyReasons** – enumeracija koja označava razlog zbog kog je datoteka samo za čitanje.

- **Data_Doc_ResourceIdHash** – GUID koji jedinstveno identificira ID resursa poslužitelja datoteke.

- **Data_Doc_RtcType** – enumeracija koja označava vrstu kanala u stvarnom vremenu (RTC) koji se koristi u datoteci.

- **Data_Doc_ServerDocId** – GUID koji jedinstveno identificira ID dokumenta poslužitelja.

- **Data_Doc_ServerProtocol** – enumeracija koja označava poslužiteljski protokol datoteke u oblaku.

- **Data_Doc_ServerType** – enumeracija koja označava vrstu poslužitelja datoteke u oblaku.

- **Data_Doc_ServerVersion** – enumeracija koja označava verziju poslužitelja datoteke u oblaku.

- **Data_Doc_SessionId** – cijeli broj koji se povećava za 1 za svaku operaciju otvaranja datoteke u sesiji.

- **Data_Doc_SharePointServiceContext** – niz koji se koristi za povezivanje klijentskih i poslužiteljskih zapisnika, obično je vrsta ID-a.

- **Data_Doc_SizeInBytes** – veličina datoteke u bajtovima.

- **Data_Doc_SpecialChars** – enumeracija koja označava kakav poseban znak ima URL datoteke.

- **Data_Doc_UrlHash** – GUID koji jedinstveno identificira URL datoteke.

- **Data_Doc_UsedWrsDataOnOpen** – bez obzira na to je li datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka.

- **Data_Doc_WopiServiceId** – niz koji pokazuje iz koje usluge je datoteka sučelja web-aplikacije s otvorenom platformom (WOPI).

- **Data_ErrorId_Code** – kod pogreške koji označava neuspjeh tijekom radnje prikupljanja podataka

- **Data_ErrorId_Tag** – oznaka u kodu kao pomoć za pronalazak točke neuspjeha

- **Data_FileOpenFlowMarkers** – prije početka procesa otvaranja datoteke odvija se određena predobrada. Ovo vrijeme potrebno za ovu prethodnu obradu bilježi se u vrijednosti niza koja ima format \<functionId>\<functionValue>\<functionId>\<functionValue>...

- **Data_FirstPartyProviderApp** – ako se otvaranje datoteke u programu Word, Excel ili PowerPoint ili aplikacijama programa Office pozove iz druge Microsoftove aplikacije, naziv toga pružatelja aplikacije bilježi se ovdje.

- **Data_InclusiveMeasurements** – vrijednost niza koja evidentira trajanje vremena provedenog u nekim pozivima funkcije, u obliku s oznakom funkcije i trajanju koje uključuje trajanje poziva podfunkcije. 

- **Data_InitializationReason** – enumeracija koja označava kako se datoteka otvara, na primjer, element korisničkog sučelja koji je pokrenula druga aplikacija itd.

- **Data_Measurements** – vrijednost niza koja evidentira trajanje vremena provedenog u nekim pozivima funkcije, u obliku s oznakom funkcije i trajanju koje isključuje trajanje poziva podfunkcije.

- **Data_OfficeMobileInitReason** – enumeracija koja označava ulaznu točku otvaranja datoteke. 

- **Data_RenderToInSpaceDuration** – trajanje razdoblja između završetka renderiranja i animacije siluete/platna.

- **Data_SilhouetteDuration** – trajanje prikazivanja otvaranja datoteke.

- **Data_TimeSplitMeasurements** – vrijednost niza koja evidentira trajanje vremena provedenog u nekim pozivima funkcije, u obliku s oznakom funkcije, početnom vremenskom oznakom i trajanjem. 

#### <a name="officeandroiddocsuipaywallcontrolpresigninfre"></a>Office.Android.DocsUI.PaywallControl.PreSignInFRE

*[Ovaj je događaj prethodno imenovan Office.DocsUI.PaywallControl.PreSignInFRE.]*
 
To je kritična uporaba telemetrija za prodaju dodatnih opcija iskustvu prvog pokretanja za nepotpisane korisnike. Tim se događajem snima metrika za prijavu u prvom pokretanju. Podaci će se koristiti za dobivanje uvida za predprijavu i razumijevanje nastavlja li korisnik sljedeću fazu u korisničkom tijeku.
 
Prikupljaju se sljedeća polja: 

- **EventDate** – vremenska oznaka pojavljivanja događaja  

- **FunnelPoint** – Identifikator da naznači mjesto na kojem se korisnik nalazi u ovom eksperimentalnom ljevku. Identifikator će odrediti hoće li korisnik vidjeti tretman i odbaciti ili ne.

- **Sessioid** – globalno jedinstveni identifikator za povezivanje događaja po sesiji


#### <a name="officeandroiddocsuipaywallcontrolskuchoosertoggled"></a>Office.Android.DocsUI.PaywallControl.SkuChooserToggled

Telemetrija upotrebe za prikaz koliko se puta korisnik prebacuje između različitih SKU-ova prije pokušaja kupnje. Upotrebljava se za razumijevanje upotrebe birača SKU-a i optimizaciju iskustva kupnje iz aplikacije u budućim verzijama.

Prikupljaju se sljedeća polja:

- **EventDate** – vremenska oznaka pojavljivanja događaja 

- **SessionID** – GUID za povezivanje događaja po sesiji


#### <a name="officeandroiddocsuipaywallcontroluserimageclicked"></a>Office.Android.DocsUI.PaywallControl.UserImageClicked 

*[Ovaj je događaj prethodno imenovan Office.DocsUI.PaywallControl.UserImageClicked.]*
 
Ovaj događaj mjeri telemetriju kako bi utvrdio pokušavaju li korisnici dovršiti radnju klikom na avatar korisnika. Ti će se podaci koristiti za mjerenje broja korisnika koji stupaju u interakciju s ikonom avatara kako bi procijenili potrebu za daljnjim iskustvom nakon dodira.
 
Prikupljaju se sljedeća polja: 

- **EventDate** – vremenska oznaka pojavljivanja događaja  

- **Sessioid** – globalno jedinstveni identifikator za povezivanje događaja po sesiji 


#### <a name="officeandroidearlytelemetryexpansionfilesavailability"></a>Office.Android.EarlyTelemetry.ExpansionFilesAvailability

Omogućujemo ekspanzijske datoteke za komplet paketa za Android (APK) za mobilnu aplikaciju Office. Ekspanzijske datoteke APK-a jesu dopunske datoteke resursa koje razvojni programeri aplikacija na sustavu Android mogu objaviti zajedno sa svojom aplikacijom. Da bi se razumjela pouzdanost ekspanzijskih datoteka, bilježimo zastavicu koja pri svakom pokretanju označava jesu li dostupne ekspanzijske datoteke ili nisu.

Prikupljaju se sljedeća polja:

- **Data_ExpansionFilesAvailable** – Booleova zastavica koja označava jesu li ekspanzijske datoteke APK-a dostupne na uređaju tijekom pokretanja aplikacije.

#### <a name="officeandroidearlytelemetryexpansionfilesdownloader"></a>Office.Android.EarlyTelemetry.ExpansionFilesDownloader

Omogućujemo ekspanzijske datoteke za komplet paketa za Android (APK) za mobilnu aplikaciju Office. Ekspanzijske datoteke APK-a jesu dopunske datoteke resursa koje razvojni programeri aplikacija na sustavu Android mogu objaviti zajedno sa svojom aplikacijom.  Da bi se razumjela pouzdanost našeg mehanizma preuzimanja ekspanzijskih datoteka, zapisujemo zastavicu koja označava možemo li uspješno preuzeti ekspanzijske datoteke.

Prikupljaju se sljedeća polja: 

- **Data_DownloadSuccess** – Booleova zastavica koja označava je li preuzimanje ekspanzijskih datoteka APK-a bilo uspješno kad god pokušamo preuzimanje tijekom pokretanja aplikacije.

#### <a name="officeandroidearlytelemetrynotecreated"></a>Office.Android.EarlyTelemetry.NoteCreated

Ključan signal koji se koristi za nadzor mogućnosti da korisnici aplikacije Ljepljive bilješke mogu stvarati bilješke u aplikaciji. Telemetrija se koristi za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. Ako korisnici ne mogu stvoriti bilješku, time bi se izazvao incident visoke ozbiljnosti.

Prikupljaju se sljedeća polja:

- **IsExportable** – zastavica koja označava je li ovaj događaj bio rezultat radnje korisnika ili ne. Treba se postaviti na Istinito jer je NoteCreated radnja koju aktivira korisnik.

- **NoteLocalId** – prepoznatljiv jedinstveni identifikator dodijeljen bilješci u vrijeme kada korisnik stvori bilješku unutar aplikacije.

- **StickyNotes-SDKVersion** – broj verzije koji označava verziju aplikacije Sticky Notes koju korisnik koristi. Omogućuje prepoznavanje verzija proizvoda s kojima se pojavljuje problem kako bismo mogli ispravno odrediti njegov prioritet.


#### <a name="officeandroidearlytelemetrynoteviewed"></a>Office.Android.EarlyTelemetry.NoteViewed 

Ključan signal koji se koristi za nadzor mogućnosti da korisnici aplikacije Ljepljive bilješke mogu prikazivati bilješke u aplikaciji. Telemetrija se koristi za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. Ako korisnici ne mogu vidjeti svoje bilješke, time bi se izazvao incident visoke ozbiljnosti.

Prikupljaju se sljedeća polja:

- **HasImages** – zastavica koja označava jesu li u prikazanoj bilješci pohranjene slike.

- **IsExportable** – zastavica koja označava je li ovaj događaj bio rezultat radnje korisnika ili ne. Treba se postaviti na Istinito jer je NoteViewed radnja koju aktivira korisnik.

- **NoteLocalId** – prepoznatljiv jedinstveni identifikator dodijeljen bilješci u vrijeme kada korisnik stvori bilješku unutar aplikacije.

- **StickyNotes-SDKVersion** – broj verzije koji označava verziju aplikacije Sticky Notes koju korisnik koristi. Omogućuje prepoznavanje verzija proizvoda s kojima se pojavljuje problem kako bismo mogli ispravno odrediti njegov prioritet.


#### <a name="officeandroidintuneintunecompliancerequest"></a>Office.Android.Intune.IntuneComplianceRequest

Ovaj se događaj prikuplja za aplikacije sustava Office na platformi Android, uključujući Office Mobile, Word, Excel, PowerPoint i OneNote. Događaj označava pokušaj prijave na račun ustanove ili tvrtke s licencom za Intune za koji je administrator tvrtke ili ustanove konfigurirao pravilnike za uvjetni pristup aplikacijama. Koristi se za razumijevanje broja krajnjih korisnika koji pokušavaju koristiti aplikacije u okviru ove konfiguracije pravilnika i kombinira s drugim događajem, Office.Android.Intune.IntuneComplianceStatus, radi osiguravanja provedbe konfiguriranog pravilnika. 

Ne prikupljaju se nikakva polja podataka.

#### <a name="officeandroidintuneintunecompliancestatus"></a>Office.Android.Intune.IntuneComplianceStatus

Ovaj se događaj prikuplja za aplikacije sustava Office na platformi Android, uključujući Office Mobile, Word, Excel, PowerPoint i OneNote. Događaj označava pokušaj prijave na račun ustanove ili tvrtke s licencom za Intune za koji je administrator tvrtke ili ustanove konfigurirao pravilnike za uvjetni pristup aplikacijama. Ovaj događaj označava status usklađivanja aplikacije u koju se korisnik prijavio i koristi se za istraživanje kvarova. Kombinira se s drugim događajem, Office.Android.Intune.IntuneComplianceRequest, radi osiguravanja provedbe konfiguriranog pravilnika.
  
Prikupljaju se sljedeća polja:

- **Data_ComplianceStatus** – označava status usklađenosti aplikacije tijekom prijave s kodom pogreške za uspjeh ili neuspjeh.
  - -1 – Nepoznata pogreška
  -    0 – Aplikacija je u skladu s pravilnicima ustanove ili tvrtke
  - 1 – Aplikacija nije u skladu s pravilnicima ustanove ili tvrtke
  - 2 – Kvarovi u vezi sa servisom
  - 3 – Kvarovi u vezi s mrežom
  - 4 – Aplikacija nije uspjela dohvatiti token za provjeru autentičnosti 
  - 5 – Odgovor usluge još nije primljen
  - 6 – Potrebno je instalirati aplikaciju portala tvrtke

#### <a name="officeandroidodwxpssotelemetry"></a>Office.Android.ODWXPSSO.Telemetry

Ovaj događaj pomaže u razumijevanju s kojom drugom Microsoftovom aplikacijom na uređaju, naša aplikacija se tiho jedinstveno prijavila, s koje ulazne točke i tako dalje. Također pomaže u razumijevanju razloga neuspjeha zbog kojeg nije došlo do tihe jedinstvene prijave.  Dobivamo bolje uvide, primjerice, iz koje Microsoftove aplikacije na uređaju, dobivamo iskustvo jedinstvene prijave. Djelujte prema neuspjesima, gdje jedinstvena prijava ne funkcionira prema očekivanjima.

Prikupljaju se sljedeća polja:

- **AccountType** – označava vrstu računa koji se odnosi na jedinstvenu prijavu, poput osobnog Microsoftovog računa ili poslovnog računa.

- **EntryPoint** – označava ulaznu točku u aplikaciji, odakle je pokrenuta jedinstvena prijava.

- **ErrorCode** – označava kôd pogreške pri pokušaju jedinstvene prijave.

- **ErrorDescription** – označava poruku o pogrešci pri pokušaju jedinstvene prijave.

- **HResult** – označava kôd statusa rezultata pri pokušaju jedinstvene prijave.

- **ProviderPackageId** – druga Microsoftova aplikacija na uređaju na kojoj se odvija jedinstvena prijava.

#### <a name="officeandroidphonenumbersignins"></a>Office.Android.PhoneNumberSignIns

Ovaj događaj pomaže u razumijevanju ako je korisnik prijavljen ili se registrirao s računom koji se temelji na telefonskom broju ili na temelju osobnog Microsoftova računa e-pošte.  Ovaj događaj pomaže u saznanju broja korisnika koji se prijavljuju ili registriraju pomoću osobnog Microsoftovog računa temeljenog na telefonskom broju.

Prikupljaju se sljedeća polja:

- **EntryPoint** – označava ulaznu točku u aplikaciji, odakle je pokrenut pokušaj prijave.

- **IsEmailMissing** – nedostaje li e-pošta u podacima profila računa?

- **IsPhoneNumberMissing** – nedostaje li telefonski broj u podacima profila računa?

- **UserDecision** – označava izbor koji je odabrao korisnik, poput prijave ili registracije ili kasnije prijave.

#### <a name="officeandroidusersignindecision"></a>Office.Android.UserSignInDecision

Ovaj događaj pomaže u razumijevanju u kojoj se fazi korisnik odbacuje u tijeku prijave, zašto prijava ne uspijeva, koliko se korisnika uspješno prijavilo, s koje ulazne točke u aplikaciji i tako dalje.  Ovaj događaj pomaže s podacima o kanalima za prijavu, što pomaže u razumijevanju u kojoj se fazi korisnici više odbacuju i slično.

Prikupljaju se sljedeća polja:

- **AccountType** – označava vrstu računa s kojim je pokušana prijava, poput osobnog ili radnog računa.

- **AfterLicensingState** – upućuje na stanje licenciranja aplikacije nakon dovršene prijave.

- **AllowedEditsWithoutSignIn** – označava koliko je besplatnih izmjena isteklo prije pokušaja prijave.

- **BeforeLicensingState** – upućuje na stanje licenciranja aplikacije prije pokušaja prijave.

- **CompletionState** – označava fazu završetka prijave.

- **EntryPoint** – označava ulaznu točku u aplikaciji, odakle je pokrenut pokušaj prijave.

- **HRDAutoAcceleratedSignUpAttemptCount** – upućuje na broj pokušaja ubrzane registracije.

- **HRDAutoAcceleratedSignUpQuitCount** – upućuje na broj otkazanih ubrzanih registracija.

- **HResult** – označava kôd statusa rezultata operacije prijave.

- **IsPhoneOnlyAuthFeatureEnabled** – je li dopuštena prijava na temelju telefonskog broja ili nije?

- **LicenseActivationHResult** – označava kôd statusa pokušaja aktivacije licence.

- **LicenseActivationMessageCode** – označava kôd poruke iz usluge licenciranja.

- **NoFreeEditsTreatmentValue** – je li dopušteno besplatno uređivanje ili ne?

- **SignUpAttemptCount** – upućuje na broj pokušaja prijave.

- **StartMode** – označava način u kojem je pokrenut pokušaj prijave.

- **UserDecision** – označava izbor koji je odabrao korisnik, poput prijave ili registracije ili kasnije prijave.


#### <a name="officeappcompatappcompatagentscanandupload"></a>Office.AppCompat.AppCompat.AgentScanAndUpload

Prikuplja se samo kada je krajnji korisnik omogućio telemetrijsku nadzornu ploču sustava Office. Prikuplja informacije o tome kada se izvršava telemetrijski agent sustava Office.    Prikuplja se samo kada je omogućena telemetrijska nadzorna ploča sustava Office i služi za utvrđivanje stanja telemetrijskog agenta sustava Office.

Prikupljaju se sljedeća polja:

  - **Data.AgentExit** – vremenska oznaka uspješnog zatvaranja telemetrijskog agenta

  - **Data.AgentScan** – vremenska oznaka uspješnog dovršavanja pregleda telemetrijskog agenta

  - **Data.AgentUpload** – vremenska oznaka uspješnog učitavanja telemetrijskog agenta

#### <a name="officeappcompatappcompatagentupload"></a>Office.AppCompat.AppCompat.AgentUpload

Stvara se tijekom pokretanja korisnika kada je krajnji korisnik omogućio telemetrijsku nadzornu ploču sustava Office.  Prikuplja informacije o tome kada je telemetrijski agent sustava Office prenio podatke u mapu za zajedničko korištenje. Primarno korištenje ovog događaja jest nadzirati stanje telemetrijskog agenta sustava Office, a sekundarno korištenje događaja jest procijeniti korištenje telemetrijske nadzorne ploče sustava Office.

Prikupljaju se sljedeća polja:

- **UploadTime** – vremenska oznaka posljednjeg uspješnog prijenosa koji je proveo telemetrijski agent.


#### <a name="officeappcompatappcompattelemetrydashboardresiliencycrashlog"></a>Office.AppCompat.AppCompat.TelemetryDashboardResiliencyCrashLog

Prikuplja se samo kada je krajnji korisnik (najčešće administrator) omogućio telemetrijsku nadzornu ploču sustava Office. Prikuplja pojavu rušenja dodataka i dokumenata sustava Office.  Prikuplja se samo kada je korisnik omogućio telemetrijsku nadzornu ploču sustava Office i služi za utvrđivanje povećane pojave rušenja dodataka ili dokumenata.

Prikupljaju se sljedeća polja:

  - **Data.CollectionTime** – vremenska oznaka zapisivanja događaja rušenja

#### <a name="officeappdocsappdocsdocumentoperation"></a>Office.AppDocs.AppDocs.DocumentOperation

Taj se događaj prikuplja za aplikacije sustava Office na uređajima sa sustavom Android, iOS, Universal ili Windows. Događaj bilježi kada se odvija operacija datoteke (stvaranje/otvaranje/spremanje/izvoz itd.) te se upotrebljava za razumijevanje i postavljanje prioriteta korisničkog iskustva na temelju podataka o operaciji datoteke.

Prikupljaju se sljedeća polja:

- **Data_AppIdForReportEndBeforeAppKnown** – ID aplikacije kada nije poznat prije okončanja izvješća za operaciju.

- **Data_CanContinueFromOnBeforeOperationBegins** – stanje CanContinue prije uključivanja rukovatelja.

- **Data_DetachedDuration** – trajanje procesa odvajanja događaja. 

- **Data_Doc_AccessMode** – enumeracija koja upućuje na način pristupa datoteci, na primjer, samo za čitanje, za čitanje i pisanje.

- **Data_Doc_AsyncOpenKind** – enumeracija koja upućuje na vrstu asinkronog toka koji se koristi za otvaranje datoteke.

- **Data_Doc_ChunkingType** – enumeracija koja upućuje na vrstu algoritma podjele datoteke na blokove.

- **Data_Doc_EdpState** – enumeracija koja upućuje na stanje korporacijske zaštite podataka datoteke.

- **Data_Doc_Ext** – prva 4 znaka datotečnog nastavka datoteke.

- **Data_Doc_Fqdn** – naziv glavnog računala poslužitelja datoteke.

- **Data_Doc_FqdnHash** – GUID koji jedinstveno identificira naziv glavnog računala poslužitelja.

- **Data_Doc_IdentityTelemetryId** – jednosmjerno raspršivanje korisničkog identiteta kojim se izvršava otvaranje.

- **Data_Doc_InitializationScenario** – enumeracija koja upućuje na detaljnu vrstu scenarija otvaranja datoteke.

- **Data_Doc_IOFlags** – enumeracija koja označava zastavice UI operacije otvaranja datoteke, na primjer, je li datoteka predmemorirana.

- **Data_Doc_IsCloudCollabEnabled** – je li za datoteku omogućena suradnja u oblaku.

- **Data_Doc_IsIncrementalOpen** – je li datoteka otvorena inkrementalno.

- **Data_Doc_IsOcsSupported** – podržava li datoteka uslugu suradnje u sustavu Office.

- **Data_Doc_IsOpeningOfflineCopy** – je li datoteka otvorena iz izvanmrežne predmemorirane kopije.

- **Data_Doc_IsPrefetched** – je li datoteka unaprijed dohvaćena prije operacije otvaranja.

- **Data_Doc_IsSyncBacked** – postoji li datoteka oblaka lokalno i je li sinkronizirana s poslužiteljem.

- **Data_Doc_Location** – enumeracija koja upućuje gdje se datoteka nalazi, na primjer, lokalno ili u oblaku.

- **Data_Doc_ReadOnlyReasons** – enumeracija koja označava razlog zbog kojeg je datoteka samo za čitanje.

- **Data_Doc_ResourceIdHash** – GUID koji jedinstveno identificira ID resursa poslužitelja datoteke.

- **Data_Doc_RtcType** – enumeracija koja označava vrstu kanala u stvarnom vremenu (RTC) koji se koristi u datoteci.

- **Data_Doc_ServerDocId** – GUID koji jedinstveno identificira ID dokumenta poslužitelja.

- **Data_Doc_ServerProtocol** – enumeracija koja označava poslužiteljski protokol datoteke u oblaku.

- **Data_Doc_ServerType** – enumeracija koja označava vrstu poslužitelja datoteke u oblaku.

- **Data_Doc_ServerVersion** – enumeracija koja označava verziju poslužitelja datoteke u oblaku.

- **Data_Doc_SessionId** – cijeli broj koji se povećava za 1 za svaku operaciju otvaranja datoteke u sesiji.

- **Data_Doc_SharePointServiceContext** – niz koji se koristi za korelaciju klijentskih i poslužiteljskih zapisnika, obično je vrsta identifikatora.

- **Data_Doc_SizeInBytes** – veličina datoteke u bajtovima.

- **Data_Doc_SpecialChars** – enumeracija koja označava kakav poseban znak ima URL datoteke.

- **Data_Doc_UrlHash** – GUID koji jedinstveno identificira URL datoteke.

- **Data_Doc_UsedWrsDataOnOpen** – je li datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka.

- **Data_Doc_WopiServiceId** – niz koji pokazuje iz koje usluge potječe datoteka WOPI (sučelje web-aplikacije s otvorenom platformom).

- **Data_DocumentInputCurrency** – vrsta unosa dokumenta koja se koristi u operaciji.

- **Data_DocumentOperation_AppId** – enumeracijska vrijednost koja predstavlja identifikator aplikacije.

- **Data_DocumentOperation_EndEventId** – oznaka koja predstavlja mjesto završetka operacije.

- **Data_DocumentOperation_EndReason** – enumeracijska vrijednost koja predstavlja razlog završetka.

- **Data_DocumentOperation_IsReinitialized** – inicijalizira li se ponovno dokument koji je već otvoren.

- **Data_DocumentOperation_isTargetECBeginEC** – je li kontekst izvršavanja cilja jednak kontekstu korištenom za otvaranje.

- **Data_DocumentOperation_ParamsFlags** – enumeracijske zastavice koje se koriste za početak operacije.

- **Data_DocumentOperation_TelemetryReason** – enumeracijsko predstavljanje ulazne točke za događaj otvaranja. Npr. otvoren iz MRU-a ili pregledavanja, aktivacija datoteke itd.

- **Data_FileIOInclusiveMeasurements** – vrijednost niza koja bilježi trajanje vremena provedenog u nekim pozivanjima funkcija, u obliku s oznakom funkcije i trajanjem koje uključuje trajanje pozivanja podfunkcija.

- **Data_FileIOMeasurements** – vrijednost niza koja bilježi trajanje vremena provedenog u nekim pozivanjima funkcija, u obliku s oznakom funkcije i trajanjem koje isključuje trajanje pozivanja podfunkcija.

- **Data_InitializationReason** – prikaz enumeracije specifičnog razloga za operaciju. Na primjer, otvoreno iz URL-a ili staze lokalne datoteke, stvoreno s pomoću birača datoteka, kopirano u stazu datoteke, izvezeno u URL itd.

- **Data_IsDisambiguateCsiNetworkConnectivityErrorEnabled**.

- **Data_IsNameMissingInUrl** – upućuje na to je li naziv izveden iz URL-a.

- **Data_IsPathMissingForLocalFile** – upućuje na to je li to lokalna datoteka bez puta.

- **Data_IsUnpackedLinkSupportedForOpen** – upućuje na to je li pri otvaranju podržana veza koja se ne može zapakirati.

- **Data_LinksOpenRightScenario** – enumeracijska vrijednost za scenarij pravilnog otvaranja veza.

- **Data_OpEndEventId** – oznaka koja predstavlja mjesto završetka operacije.

- **Data_OperationType** – prikaz enumeracije generičke vrste operacije. Na primjer, stvaranje, otvaranje, kopiranje, spremanje itd.

- **Data_RelatedPrevOpTelemetryReason** – je li operacija povezana s prethodnom.

- **Data_StopwatchDuration** – ukupno vrijeme za događaj.

- **Data_UnpackLinkHint** – enumeracija koja predstavlja potencijalnu korisnikovu akciju na temelju veze za raspakiravanje.

- **Data_UnpackLinkPromptResult** – enumeracija koja predstavlja odgovor odzivnika veze za raspakiravanje.

#### <a name="officeappleactivateperpetual"></a>Office.Apple.ActivatePerpetual

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za nadziranje stanja trajnog tijeka aktivacije kao i za istraživanje uzroka pogrešaka pregledom vrijednosti FailedAt.

Prikupljaju se sljedeća polja:

- **Data_FailedAt** – prikupljamo niz koji predstavlja gdje smo pogriješili u tijeku aktiviranja trajne licence.

#### <a name="officeappleactivatesubscription"></a>Office.Apple.ActivateSubscription

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Prikupljamo informacije vezane za migraciju iz naslijeđenog kôd stoga za licenciranje u vNext kôd stoga za licenciranje. To se koristi za nadziranje stanja tijeka aktivacije pretplate kao i za praćenje ako je to migracija za licenciranje vNext i ako je korišten primarni identitet.

Prikupljaju se sljedeća polja:

- **Data_ActivatingPrimaryIdentity** – vrijednost true/false koja označava je li korišten primarni identitet. 

- **Data_NULSubscriptionLicensed** – vrijednost true/false koja označava stanje pretplate

#### <a name="officeapplecisauthticketwithidentity"></a>Office.Apple.CISAuthTicketWithIdentity

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za dohvaćanje neuspjelih stvaranja tokena provjere autentičnosti tijekom kupnje u aplikaciji na Macu (događaj zapisuje primljeni kod pogreške).  Ovaj događaj koristi se za prepoznavanje i pomoć pri otklanjanju poteškoća pri neuspjelim stvaranjima tokena provjere autentičnosti

Prikupljaju se sljedeća polja:

- **Data_EmptyAuthToken** – prikupljamo niz koji predstavlja gdje smo pogriješili u tijeku aktiviranja trajne licence.

- **Data_TicketAuthError** – kod pogreške koji označava uzrok pogreške

- **Data_ValidIdentity** – ako klijent ima valjani identitet

#### <a name="officeappleinappassociationactivity"></a>Office.Apple.InAppAssociationActivity

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Prikupljamo podatke povezane s vezom proizvoda nakon kupnje unutar aplikacije. Bilježimo koji pretplatni SKU povezujemo.  To se koristi za nadziranje stanja kupnje veze proizvoda unutar aplikacije.

Prikupljaju se sljedeća polja:

- **Data_ProductID** – Pretplatni SKU s kojim pokušavamo povezati proizvod.

#### <a name="officeappleinapppurchaseactivity"></a>Office.Apple.InAppPurchaseActivity

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. 

U trgovini AppStore prikupljamo informacije povezane s kupnjom proizvoda. Pratimo rezultat kupnje (neuspjeh, uspjeh, problem s plaćanjem, itd.), vrstu zahtjeva za kupnju (vraćanje, kupnja) i SKU/proizvod koji se kupuje (Microsoft 365 Family itd.).  Ti se podaci koriste za nadgledanje stanja tokova kupnje unutar aplikacije.

Prikupljaju se sljedeća polja:

- **Data_ Data_PurchaseResult** – rezultat operacije kupnje


- **Data_ProductID** – proizvod koji se kupuje

- **Data_PurchaseRequestType** – vrsta zahtjeva za kupnju

#### <a name="officeappleintune"></a>Office.Apple.InTune

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Prikupljamo da li trenutnom sesijom upravlja Intune. To se koristi za zaokretanje/filtriranje sesija kojim upravlja Intune i omogućuje nam istraživanje potencijalnih problema vezanih uz pokretanje sustava Office u obliku aplikacije kojoj upravlja Intune.

Prikupljaju se sljedeća polja:

- **Data_EventID** – prikupljamo niz koji predstavlja kôd koji pokazuje radi li se o sesiji kojom upravlja Intune.

#### <a name="officeapplelicensingmaclicensingstate"></a>Office.Apple.Licensing.Mac.LicensingState

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj bilježi trenutno stanje licence za sesiju u stroju (OLS ID licence, SKU koji se koristi, razdoblje mirovanje ili ne, RFM, itd.). Prikupljeni podaci koriste se za otkrivanje pogrešaka i istraživanje uzroka neuspjeha. 

Prikupljaju se sljedeća polja:

- **Data_DidRunPreview** – Niz koji označava je li ova sesija pokrenuta u pretpregledu

- **Data_LicensingACID** – Niz koji predstavlja unutarnji identifikator sustava licenciranja

- **Data_LicensingType** – Niz koji predstavlja vrstu licence

- **Data_OLSLicenseId** – Niz koji predstavlja identifikator licence

- **Data_State** – Niz koji predstavlja trenutno stanje licence

#### <a name="officeconnectdeviceactivitystart"></a>Office.ConnectDevice.Activity.Start

Omogućuje da utvrdimo je li uspjelo povezivanje s uređajem ili aplikacijom.  Koristi se za stanje i nadzor značajke. Taj je događaj generirao dodatak Microsoft Data Streamer za Excel.

Prikupljaju se sljedeća polja:

- **Datasource_Type** – informacije o serijskom uređaju ili servisu aplikacije

- **DataSource_Name** – naziv povezanog izvora podataka

- **Activity_Name** = naziv aktivnosti „ConnectDevice”

- **Activity_CV** = ID za povezivanje događaja u sesiji povezivanja

- **Activity_StartStopType** = početak

- **Activity_DateTimeTicks** = vrijeme podataka za aktivnost
 
#### <a name="officeconnectdeviceactivitystop"></a>Office.ConnectDevice.Activity.Stop

Omogućuje da utvrdimo je li uspjelo povezivanje s uređajem ili aplikacijom. Koristi se za stanje i nadzor značajke. Taj je događaj generirao dodatak Microsoft Data Streamer za Excel.

Prikupljaju se sljedeća polja:

- **Datasource_Type** – informacije o serijskom uređaju ili servisu aplikacije

- **DataSource_Name** – naziv povezanog izvora podataka

- **Activity_Name** – naziv aktivnosti „ConnectDevice”

- **Activity_CV** – ID za povezivanje događaja u sesiji povezivanja

- **Activity_StartStopType** – zaustavljanje

- **Activity_DateTimeTicks** – vrijeme podataka za aktivnost

#### <a name="officedocsappdocsoperationopenfrommrubypath"></a>Office.Docs.AppDocs.OperationOpenFromMruByPath

Taj se događaj prikuplja za aplikacije sustava Office na uređajima sa sustavom Android, iOS, Universal ili Windows. Događaj bilježi kada se operacija otvaranja datoteke odvija pomoću puta navedenog na popisu nedavnih datoteka te se koristi za razumijevanje i postavljanje prioriteta pogrešaka korisničkog doživljaja na temelju podataka o operaciji otvaranja datoteke.

Prikupljaju se sljedeća polja:

- **Data_AppIdForReportEndBeforeAppKnown** – ID aplikacije kada nije poznat prije okončanja izvješća za operaciju.

- **Data_CanContinueFromOnBeforeOperationBegins** – stanje CanContinue prije uključivanja rukovatelja.

- **Data_DetachedDuration** – trajanje procesa odvajanja događaja. 

- **Data_Doc_AccessMode** – enumeracija koja upućuje na način pristupa datoteci, na primjer, samo za čitanje, za čitanje i pisanje.

- **Data_Doc_AsyncOpenKind** – enumeracija koja upućuje na vrstu asinkronog toka koji se koristi za otvaranje datoteke.

- **Data_Doc_ChunkingType** – enumeracija koja upućuje na vrstu algoritma podjele datoteke na blokove.

- **Data_Doc_EdpState** – enumeracija koja upućuje na stanje korporacijske zaštite podataka datoteke.

- **Data_Doc_Ext** – prva četiri znaka datotečnog nastavka.

- **Data_Doc_Fqdn** – naziv glavnog računala poslužitelja datoteke.

- **Data_Doc_FqdnHash** – GUID koji jedinstveno identificira naziv glavnog računala poslužitelja.

- **Data_Doc_IdentityTelemetryId** – jednosmjerno raspršivanje korisničkog identiteta kojim se izvršava otvaranje.

- **Data_Doc_InitializationScenario** – enumeracija koja upućuje na detaljnu vrstu scenarija otvaranja datoteke.

- **Data_Doc_IOFlags** – enumeracija koja označava zastavice UI operacije otvaranja datoteke, na primjer, je li datoteka predmemorirana.

- **Data_Doc_IsCloudCollabEnabled** – je li za datoteku omogućena suradnja u oblaku.

- **Data_Doc_IsIncrementalOpen** – je li datoteka otvorena inkrementalno.

- **Data_Doc_IsOcsSupported** – podržava li datoteka uslugu suradnje u sustavu Office.

- **Data_Doc_IsOpeningOfflineCopy** – je li datoteka otvorena iz izvanmrežne predmemorirane kopije.

- **Data_Doc_IsPrefetched** – je li datoteka unaprijed dohvaćena prije operacije otvaranja.

- **Data_Doc_IsSyncBacked** – postoji li datoteka oblaka lokalno i je li sinkronizirana s poslužiteljem.

- **Data_Doc_Location** – enumeracija koja upućuje gdje se datoteka nalazi, na primjer, lokalno ili u oblaku.

- **Data_Doc_ReadOnlyReasons** – enumeracija koja označava razlog zbog kojeg je datoteka samo za čitanje.

- **Data_Doc_ResourceIdHash** – GUID koji jedinstveno identificira ID resursa poslužitelja datoteke.

- **Data_Doc_RtcType** – enumeracija koja označava vrstu kanala u stvarnom vremenu (RTC) koji se koristi u datoteci.

- **Data_Doc_ServerDocId** – GUID koji jedinstveno identificira ID dokumenta poslužitelja.

- **Data_Doc_ServerProtocol** – enumeracija koja označava poslužiteljski protokol datoteke u oblaku.

- **Data_Doc_ServerType** – enumeracija koja označava vrstu poslužitelja datoteke u oblaku.

- **Data_Doc_ServerVersion** – enumeracija koja označava verziju poslužitelja datoteke u oblaku.

- **Data_Doc_SessionId** – cijeli broj koji se povećava za 1 za svaku operaciju otvaranja datoteke u sesiji.

- **Data_Doc_SharePointServiceContext** – niz koji se koristi za korelaciju klijentskih i poslužiteljskih zapisnika, obično je vrsta identifikatora.

- **Data_Doc_SizeInBytes** – veličina datoteke u bajtovima.

- **Data_Doc_SpecialChars** – enumeracija koja označava kakav poseban znak ima URL datoteke.

- **Data_Doc_UrlHash** – GUID koji jedinstveno identificira URL datoteke.

- **Data_Doc_UsedWrsDataOnOpen** – je li datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka.

- **Data_Doc_WopiServiceId** – niz koji pokazuje iz koje usluge potječe datoteka WOPI (sučelje web-aplikacije s otvorenom platformom).

- **Data_DocumentInputCurrency** – vrsta unosa dokumenta koja se koristi u operaciji.

- **Data_DocumentOperation_AppId** – enumeracijska vrijednost koja predstavlja identifikator aplikacije.

- **Data_DocumentOperation_EndEventId** – oznaka koja predstavlja mjesto završetka operacije.

- **Data_DocumentOperation_EndReason** – enumeracijska vrijednost koja predstavlja razlog završetka.

- **Data_DocumentOperation_IsReinitialized** – inicijalizira li se ponovno dokument koji je već otvoren.

- **Data_DocumentOperation_ParamsFlags** – enumeracijske zastavice koje se koriste za početak operacije.

- **Data_DocumentOperation_TelemetryReason** – enumeracijsko predstavljanje ulazne točke za događaj otvaranja. Npr. otvoren iz MRU-a ili pregledavanja, aktivacija datoteke itd.

- **Data_DocumentOperation_isTargetECBeginEC** – je li kontekst izvršavanja cilja jednak kontekstu korištenom za otvaranje.

- **Data_FileIOInclusiveMeasurements** – vrijednost niza koja bilježi trajanje vremena provedenog u nekim pozivanjima funkcija, u obliku s oznakom funkcije i trajanjem koje uključuje trajanje pozivanja podfunkcija.

- **Data_FileIOMeasurements** – vrijednost niza koja bilježi trajanje vremena provedenog u nekim pozivanjima funkcija, u obliku s oznakom funkcije i trajanjem koje isključuje trajanje pozivanja podfunkcija.

- **Data_IsNameMissingInUrl** – upućuje na to je li naziv izveden iz URL-a.

- **Data_IsPathMissingForLocalFile** – upućuje na to je li to lokalna datoteka bez puta.

- **Data_IsUnpackedLinkSupportedForOpen** – upućuje na to je li pri otvaranju podržana veza koja se ne može zapakirati.

- **Data_LinksOpenRightScenario** – enumeracijska vrijednost za scenarij pravilnog otvaranja veza.

- **Data_OpEndEventId** – oznaka koja predstavlja mjesto završetka operacije.

- **Data_RelatedPrevOpTelemetryReason** – je li operacija povezana s prethodnom.

- **Data_StopwatchDuration** – ukupno vrijeme za događaj.

- **Data_UnpackLinkHint** – enumeracija koja predstavlja potencijalnu korisnikovu akciju na temelju veze za raspakiravanje.

- **Data_UnpackLinkPromptResult** – enumeracija koja predstavlja odgovor odzivnika veze za raspakiravanje.

#### <a name="officedocsappdocsoperationopenfrommrubyurl"></a>Office.Docs.AppDocs.OperationOpenFromMruByUrl

Taj se događaj prikuplja za aplikacije sustava Office na uređajima sa sustavom Android, iOS, Universal ili Windows. Događaj bilježi kada se operacija otvaranja datoteke odvija pomoću URL-a navedenog na popisu nedavnih datoteka te se koristi za razumijevanje i postavljanje prioriteta korisničkog doživljaja na temelju podataka o operaciji otvaranja datoteke. 

Prikupljaju se sljedeća polja:

- **Data_AppIdForReportEndBeforeAppKnown** – ID aplikacije kada nije poznat prije okončanja izvješća za operaciju.

- **Data_CanContinueFromOnBeforeOperationBegins** – stanje CanContinue prije uključivanja rukovatelja.

- **Data_DetachedDuration** – trajanje procesa odvajanja događaja. 

- **Data_Doc_AccessMode** – enumeracija koja upućuje na način pristupa datoteci, na primjer, samo za čitanje, za čitanje i pisanje.

- **Data_Doc_AsyncOpenKind** – enumeracija koja upućuje na vrstu asinkronog toka koji se koristi za otvaranje datoteke.

- **Data_Doc_ChunkingType** – enumeracija koja upućuje na vrstu algoritma podjele datoteke na blokove.

- **Data_Doc_EdpState** – enumeracija koja upućuje na stanje korporacijske zaštite podataka datoteke.

- **Data_Doc_Ext** – prva četiri znaka datotečnog nastavka.

- **Data_Doc_Fqdn** – naziv glavnog računala poslužitelja datoteke.

- **Data_Doc_FqdnHash** – GUID koji jedinstveno identificira naziv glavnog računala poslužitelja.

- **Data_Doc_IdentityTelemetryId** – jednosmjerno raspršivanje korisničkog identiteta kojim se izvršava otvaranje.

- **Data_Doc_InitializationScenario** – enumeracija koja upućuje na detaljnu vrstu scenarija otvaranja datoteke.

- **Data_Doc_IOFlags** – enumeracija koja označava zastavice UI operacije otvaranja datoteke, na primjer, je li datoteka predmemorirana.

- **Data_Doc_IsCloudCollabEnabled** – je li za datoteku omogućena suradnja u oblaku.

- **Data_Doc_IsIncrementalOpen** – je li datoteka otvorena inkrementalno.

- **Data_Doc_IsOcsSupported** – podržava li datoteka uslugu suradnje u sustavu Office.

- **Data_Doc_IsOpeningOfflineCopy** – je li datoteka otvorena iz izvanmrežne predmemorirane kopije.

- **Data_Doc_IsPrefetched** – je li datoteka unaprijed dohvaćena prije operacije otvaranja.

- **Data_Doc_IsSyncBacked** – postoji li datoteka oblaka lokalno i je li sinkronizirana s poslužiteljem.

- **Data_Doc_Location** – enumeracija koja upućuje gdje se datoteka nalazi, na primjer, lokalno ili u oblaku.

- **Data_Doc_ReadOnlyReasons** – enumeracija koja označava razlog zbog kojeg je datoteka samo za čitanje.

- **Data_Doc_ResourceIdHash** – GUID koji jedinstveno identificira ID resursa poslužitelja datoteke.

- **Data_Doc_RtcType** – enumeracija koja označava vrstu kanala u stvarnom vremenu (RTC) koji se koristi u datoteci.

- **Data_Doc_ServerDocId** – GUID koji jedinstveno identificira ID dokumenta poslužitelja.

- **Data_Doc_ServerProtocol** – enumeracija koja označava poslužiteljski protokol datoteke u oblaku.

- **Data_Doc_ServerType** – enumeracija koja označava vrstu poslužitelja datoteke u oblaku.

- **Data_Doc_ServerVersion** – enumeracija koja označava verziju poslužitelja datoteke u oblaku.

- **Data_Doc_SessionId** – cijeli broj koji se povećava za 1 za svaku operaciju otvaranja datoteke u sesiji.

- **Data_Doc_SharePointServiceContext** – niz koji se koristi za korelaciju klijentskih i poslužiteljskih zapisnika, obično je vrsta identifikatora.

- **Data_Doc_SizeInBytes** – veličina datoteke u bajtovima.

- **Data_Doc_SpecialChars** – enumeracija koja označava kakav poseban znak ima URL datoteke.

- **Data_Doc_UrlHash** – GUID koji jedinstveno identificira URL datoteke.

- **Data_Doc_UsedWrsDataOnOpen** – je li datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka.

- **Data_Doc_WopiServiceId** – niz koji pokazuje iz koje usluge potječe datoteka WOPI (sučelje web-aplikacije s otvorenom platformom).

- **Data_DocumentInputCurrency** – vrsta unosa dokumenta koja se koristi u operaciji.

- **Data_DocumentOperation_AppId** – enumeracijska vrijednost koja predstavlja identifikator aplikacije.

- **Data_DocumentOperation_EndEventId** – oznaka koja predstavlja mjesto završetka operacije.

- **Data_DocumentOperation_EndReason** – enumeracijska vrijednost koja predstavlja razlog završetka.

- **Data_DocumentOperation_IsReinitialized** – inicijalizira li se ponovno dokument koji je već otvoren.

- **Data_DocumentOperation_ParamsFlags** – enumeracijske zastavice koje se koriste za početak operacije.

- **Data_DocumentOperation_TelemetryReason** – enumeracijsko predstavljanje ulazne točke za događaj otvaranja. Npr. otvoren iz MRU-a ili pregledavanja, aktivacija datoteke itd.

- **Data_DocumentOperation_isTargetECBeginEC** – je li kontekst izvršavanja cilja jednak kontekstu korištenom za otvaranje.

- **Data_FileIOInclusiveMeasurements** – vrijednost niza koja bilježi trajanje vremena provedenog u nekim pozivanjima funkcija, u obliku s oznakom funkcije i trajanjem koje uključuje trajanje pozivanja podfunkcija.

- **Data_FileIOMeasurements** – vrijednost niza koja bilježi trajanje vremena provedenog u nekim pozivanjima funkcija, u obliku s oznakom funkcije i trajanjem koje isključuje trajanje pozivanja podfunkcija.

- **Data_IsNameMissingInUrl** – upućuje na to je li naziv izveden iz URL-a.

- **Data_IsPathMissingForLocalFile** – upućuje na to je li to lokalna datoteka bez puta.

- **Data_IsUnpackedLinkSupportedForOpen** – upućuje na to je li pri otvaranju podržana veza koja se ne može zapakirati.

- **Data_LinksOpenRightScenario** – enumeracijska vrijednost za scenarij pravilnog otvaranja veza.

- **Data_OpEndEventId** – oznaka koja predstavlja mjesto završetka operacije.

- **Data_RelatedPrevOpTelemetryReason** – je li operacija povezana s prethodnom.

- **Data_StopwatchDuration** – ukupno vrijeme za događaj.

- **Data_UnpackLinkHint** – enumeracija koja predstavlja potencijalnu korisnikovu akciju na temelju veze za raspakiravanje.

- **Data_UnpackLinkPromptResult** – enumeracija koja predstavlja odgovor odzivnika veze za raspakiravanje.


#### <a name="officedocsappdocsoperationopenfrompath"></a>Office.Docs.AppDocs.OperationOpenFromPath

Taj se događaj prikuplja za aplikacije sustava Office na uređajima sa sustavom Android, iOS, Universal ili Windows. Događaj bilježi kada se operacija otvaranja datoteke odvija na temelju puta te se koristi za razumijevanje i postavljanje prioriteta korisničkog iskustva na temelju podataka o operaciji otvaranja datoteke.

Prikupljaju se sljedeća polja:

- **Data_AppIdForReportEndBeforeAppKnown** – ID aplikacije kada nije poznat prije okončanja izvješća za operaciju.

- **Data_CanContinueFromOnBeforeOperationBegins** – stanje CanContinue prije uključivanja rukovatelja.

- **Data_DetachedDuration** – trajanje procesa odvajanja događaja. 

- **Data_Doc_AccessMode** – enumeracija koja upućuje na način pristupa datoteci, na primjer, samo za čitanje, za čitanje i pisanje.

- **Data_Doc_AsyncOpenKind** – enumeracija koja upućuje na vrstu asinkronog toka koji se koristi za otvaranje datoteke.

- **Data_Doc_ChunkingType** – enumeracija koja upućuje na vrstu algoritma podjele datoteke na blokove.

- **Data_Doc_EdpState** – enumeracija koja upućuje na stanje korporacijske zaštite podataka datoteke.

- **Data_Doc_Ext** – prva četiri znaka datotečnog nastavka.

- **Data_Doc_Fqdn** – naziv glavnog računala poslužitelja datoteke.

- **Data_Doc_FqdnHash** – GUID koji jedinstveno identificira naziv glavnog računala poslužitelja.

- **Data_Doc_IdentityTelemetryId** – jednosmjerno raspršivanje korisničkog identiteta kojim se izvršava otvaranje.

- **Data_Doc_InitializationScenario** – enumeracija koja upućuje na detaljnu vrstu scenarija otvaranja datoteke.

- **Data_Doc_IOFlags** – enumeracija koja označava zastavice UI operacije otvaranja datoteke, na primjer, je li datoteka predmemorirana.

- **Data_Doc_IsCloudCollabEnabled** – je li za datoteku omogućena suradnja u oblaku.

- **Data_Doc_IsIncrementalOpen** – je li datoteka otvorena inkrementalno.

- **Data_Doc_IsOcsSupported** – podržava li datoteka uslugu suradnje u sustavu Office.

- **Data_Doc_IsOpeningOfflineCopy** – je li datoteka otvorena iz izvanmrežne predmemorirane kopije.

- **Data_Doc_IsPrefetched** – je li datoteka unaprijed dohvaćena prije operacije otvaranja.

- **Data_Doc_IsSyncBacked** – postoji li datoteka oblaka lokalno i je li sinkronizirana s poslužiteljem.

- **Data_Doc_Location** – enumeracija koja upućuje gdje se datoteka nalazi, na primjer, lokalno ili u oblaku.

- **Data_Doc_ReadOnlyReasons** – enumeracija koja označava razlog zbog kojeg je datoteka samo za čitanje.

- **Data_Doc_ResourceIdHash** – GUID koji jedinstveno identificira ID resursa poslužitelja datoteke.

- **Data_Doc_RtcType** – enumeracija koja označava vrstu kanala u stvarnom vremenu (RTC) koji se koristi u datoteci.

- **Data_Doc_ServerDocId** – GUID koji jedinstveno identificira ID dokumenta poslužitelja.

- **Data_Doc_ServerProtocol** – enumeracija koja označava poslužiteljski protokol datoteke u oblaku.

- **Data_Doc_ServerType** – enumeracija koja označava vrstu poslužitelja datoteke u oblaku.

- **Data_Doc_ServerVersion** – enumeracija koja označava verziju poslužitelja datoteke u oblaku.

- **Data_Doc_SessionId** – cijeli broj koji se povećava za 1 za svaku operaciju otvaranja datoteke u sesiji.

- **Data_Doc_SharePointServiceContext** – niz koji se koristi za korelaciju klijentskih i poslužiteljskih zapisnika, obično je vrsta identifikatora.

- **Data_Doc_SizeInBytes** – veličina datoteke u bajtovima.

- **Data_Doc_SpecialChars** – enumeracija koja označava kakav poseban znak ima URL datoteke.

- **Data_Doc_UrlHash** – GUID koji jedinstveno identificira URL datoteke.

- **Data_Doc_UsedWrsDataOnOpen** – je li datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka.

- **Data_Doc_WopiServiceId** – niz koji pokazuje iz koje usluge potječe datoteka WOPI (sučelje web-aplikacije s otvorenom platformom).

- **Data_DocumentInputCurrency** – vrsta unosa dokumenta koja se koristi u operaciji.

- **Data_DocumentOperation_AppId** – enumeracijska vrijednost koja predstavlja identifikator aplikacije.

- **Data_DocumentOperation_EndEventId** – oznaka koja predstavlja mjesto završetka operacije.

- **Data_DocumentOperation_EndReason** – enumeracijska vrijednost koja predstavlja razlog završetka.

- **Data_DocumentOperation_IsReinitialized** – inicijalizira li se ponovno dokument koji je već otvoren.

- **Data_DocumentOperation_ParamsFlags** – enumeracijske zastavice koje se koriste za početak operacije.

- **Data_DocumentOperation_TelemetryReason** – enumeracijsko predstavljanje ulazne točke za događaj otvaranja. Npr. otvoren iz MRU-a ili pregledavanja, aktivacija datoteke itd.

- **Data_DocumentOperation_isTargetECBeginEC** – je li kontekst izvršavanja cilja jednak kontekstu korištenom za otvaranje.

- **Data_FileIOInclusiveMeasurements** – vrijednost niza koja bilježi trajanje vremena provedenog u nekim pozivanjima funkcija, u obliku s oznakom funkcije i trajanjem koje uključuje trajanje pozivanja podfunkcija.

- **Data_FileIOMeasurements** – vrijednost niza koja bilježi trajanje vremena provedenog u nekim pozivanjima funkcija, u obliku s oznakom funkcije i trajanjem koje isključuje trajanje pozivanja podfunkcija.

- **Data_IsNameMissingInUrl** – upućuje na to je li naziv izveden iz URL-a.

- **Data_IsPathMissingForLocalFile** – upućuje na to je li to lokalna datoteka bez puta.

- **Data_IsUnpackedLinkSupportedForOpen** – upućuje na to je li pri otvaranju podržana veza koja se ne može zapakirati.

- **Data_LinksOpenRightScenario** – enumeracijska vrijednost za scenarij pravilnog otvaranja veza.

- **Data_OpEndEventId** – oznaka koja predstavlja mjesto završetka operacije.

- **Data_RelatedPrevOpTelemetryReason** – je li operacija povezana s prethodnom.

- **Data_StopwatchDuration** – ukupno vrijeme za događaj.

- **Data_UnpackLinkHint** – enumeracija koja predstavlja potencijalnu korisnikovu akciju na temelju veze za raspakiravanje.

- **Data_UnpackLinkPromptResult** – enumeracija koja predstavlja odgovor odzivnika veze za raspakiravanje.

#### <a name="officedocsappdocsoperationopenfromprotocolhandler"></a>Office.Docs.AppDocs.OperationOpenFromProtocolHandler

Taj se događaj prikuplja za aplikacije sustava Office na uređajima sa sustavom Android, iOS, Universal ili Windows. Događaj bilježi kada se operacija otvaranja datoteke odvija iz neke druge aplikacije putem sučelja rukovatelja protokolima te se koristi za razumijevanje i postavljanje prioriteta korisničkog iskustva na temelju podataka o operaciji otvaranja datoteke.

Prikupljaju se sljedeća polja:

- **Data_AppIdForReportEndBeforeAppKnown** – ID aplikacije kada nije poznat prije okončanja izvješća za operaciju.

- **Data_CanContinueFromOnBeforeOperationBegins** – stanje CanContinue prije uključivanja rukovatelja.

- **Data_DetachedDuration** – trajanje procesa odvajanja događaja. 

- **Data_Doc_AccessMode** – enumeracija koja upućuje na način pristupa datoteci, na primjer, samo za čitanje, za čitanje i pisanje.

- **Data_Doc_AsyncOpenKind** – enumeracija koja upućuje na vrstu asinkronog toka koji se koristi za otvaranje datoteke.

- **Data_Doc_ChunkingType** – enumeracija koja upućuje na vrstu algoritma podjele datoteke na blokove.

- **Data_Doc_EdpState** – enumeracija koja upućuje na stanje korporacijske zaštite podataka datoteke.

- **Data_Doc_Ext** – prva četiri znaka datotečnog nastavka.

- **Data_Doc_Fqdn** – naziv glavnog računala poslužitelja datoteke.

- **Data_Doc_FqdnHash** – GUID koji jedinstveno identificira naziv glavnog računala poslužitelja.

- **Data_Doc_IdentityTelemetryId** – jednosmjerno raspršivanje korisničkog identiteta kojim se izvršava otvaranje.

- **Data_Doc_InitializationScenario** – enumeracija koja upućuje na detaljnu vrstu scenarija otvaranja datoteke.

- **Data_Doc_IOFlags** – enumeracija koja označava zastavice UI operacije otvaranja datoteke, na primjer, je li datoteka predmemorirana.

- **Data_Doc_IsCloudCollabEnabled** – je li za datoteku omogućena suradnja u oblaku.

- **Data_Doc_IsIncrementalOpen** – je li datoteka otvorena inkrementalno.

- **Data_Doc_IsOcsSupported** – podržava li datoteka uslugu suradnje u sustavu Office.

- **Data_Doc_IsOpeningOfflineCopy** – je li datoteka otvorena iz izvanmrežne predmemorirane kopije.

- **Data_Doc_IsPrefetched** – je li datoteka unaprijed dohvaćena prije operacije otvaranja.

- **Data_Doc_IsSyncBacked** – postoji li datoteka oblaka lokalno i je li sinkronizirana s poslužiteljem.

- **Data_Doc_Location** – enumeracija koja upućuje gdje se datoteka nalazi, na primjer, lokalno ili u oblaku.

- **Data_Doc_ReadOnlyReasons** – enumeracija koja označava razlog zbog kojeg je datoteka samo za čitanje.

- **Data_Doc_ResourceIdHash** – GUID koji jedinstveno identificira ID resursa poslužitelja datoteke.

- **Data_Doc_RtcType** – enumeracija koja označava vrstu kanala u stvarnom vremenu (RTC) koji se koristi u datoteci.

- **Data_Doc_ServerDocId** – GUID koji jedinstveno identificira ID dokumenta poslužitelja.

- **Data_Doc_ServerProtocol** – enumeracija koja označava poslužiteljski protokol datoteke u oblaku.

- **Data_Doc_ServerType** – enumeracija koja označava vrstu poslužitelja datoteke u oblaku.

- **Data_Doc_ServerVersion** – enumeracija koja označava verziju poslužitelja datoteke u oblaku.

- **Data_Doc_SessionId** – cijeli broj koji se povećava za 1 za svaku operaciju otvaranja datoteke u sesiji.

- **Data_Doc_SharePointServiceContext** – niz koji se koristi za korelaciju klijentskih i poslužiteljskih zapisnika, obično je vrsta identifikatora.

- **Data_Doc_SizeInBytes** – veličina datoteke u bajtovima.

- **Data_Doc_SpecialChars** – enumeracija koja označava kakav poseban znak ima URL datoteke.

- **Data_Doc_UrlHash** – GUID koji jedinstveno identificira URL datoteke.

- **Data_Doc_UsedWrsDataOnOpen** – je li datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka.

- **Data_Doc_WopiServiceId** – niz koji pokazuje iz koje usluge potječe datoteka WOPI (sučelje web-aplikacije s otvorenom platformom).

- **Data_DocumentInputCurrency** – vrsta unosa dokumenta koja se koristi u operaciji.

- **Data_DocumentOperation_AppId** – enumeracijska vrijednost koja predstavlja identifikator aplikacije.

- **Data_DocumentOperation_EndEventId** – oznaka koja predstavlja mjesto završetka operacije.

- **Data_DocumentOperation_EndReason** – enumeracijska vrijednost koja predstavlja razlog završetka.

- **Data_DocumentOperation_IsReinitialized** – inicijalizira li se ponovno dokument koji je već otvoren.

- **Data_DocumentOperation_ParamsFlags** – enumeracijske zastavice koje se koriste za početak operacije.

- **Data_DocumentOperation_TelemetryReason** – enumeracijsko predstavljanje ulazne točke za događaj otvaranja. Npr. otvoren iz MRU-a ili pregledavanja, aktivacija datoteke itd.

- **Data_DocumentOperation_isTargetECBeginEC** – je li kontekst izvršavanja cilja jednak kontekstu korištenom za otvaranje.

- **Data_FileIOInclusiveMeasurements** – vrijednost niza koja bilježi trajanje vremena provedenog u nekim pozivanjima funkcija, u obliku s oznakom funkcije i trajanjem koje uključuje trajanje pozivanja podfunkcija.

- **Data_FileIOMeasurements** – vrijednost niza koja bilježi trajanje vremena provedenog u nekim pozivanjima funkcija, u obliku s oznakom funkcije i trajanjem koje isključuje trajanje pozivanja podfunkcija.

- **Data_IsNameMissingInUrl** – upućuje na to je li naziv izveden iz URL-a.

- **Data_IsPathMissingForLocalFile** – upućuje na to je li to lokalna datoteka bez puta.

- **Data_IsUnpackedLinkSupportedForOpen** – upućuje na to je li pri otvaranju podržana veza koja se ne može zapakirati.

- **Data_LinksOpenRightScenario** – enumeracijska vrijednost za scenarij pravilnog otvaranja veza.

- **Data_OpEndEventId** – oznaka koja predstavlja mjesto završetka operacije.

- **Data_RelatedPrevOpTelemetryReason** – je li operacija povezana s prethodnom.

- **Data_StopwatchDuration** – ukupno vrijeme za događaj.

- **Data_UnpackLinkHint** – enumeracija koja predstavlja potencijalnu korisnikovu akciju na temelju veze za raspakiravanje.

- **Data_UnpackLinkPromptResult** – enumeracija koja predstavlja odgovor odzivnika veze za raspakiravanje.

#### <a name="officedocsappdocsoperationopenfromshell"></a>Office.Docs.AppDocs.OperationOpenFromShell

Taj se događaj prikuplja za aplikacije sustava Office na uređajima sa sustavom Android, iOS, Universal ili Windows. Događaj bilježi kada se operacija otvaranja datoteke odvija iz ljuske te se koristi za razumijevanje i postavljanje prioriteta korisničkog iskustva na temelju podataka o operaciji otvaranja datoteke.

Prikupljaju se sljedeća polja:

- **Data_AppIdForReportEndBeforeAppKnown** – ID aplikacije kada nije poznat prije okončanja izvješća za operaciju.

- **Data_CanContinueFromOnBeforeOperationBegins** – stanje CanContinue prije uključivanja rukovatelja.

- **Data_DetachedDuration** – trajanje procesa odvajanja događaja. 

- **Data_Doc_AccessMode** – enumeracija koja upućuje na način pristupa datoteci, na primjer, samo za čitanje, za čitanje i pisanje.

- **Data_Doc_AsyncOpenKind** – enumeracija koja upućuje na vrstu asinkronog toka koji se koristi za otvaranje datoteke.

- **Data_Doc_ChunkingType** – enumeracija koja upućuje na vrstu algoritma podjele datoteke na blokove.

- **Data_Doc_EdpState** – enumeracija koja upućuje na stanje korporacijske zaštite podataka datoteke.

- **Data_Doc_Ext** – prva četiri znaka datotečnog nastavka.

- **Data_Doc_Fqdn** – naziv glavnog računala poslužitelja datoteke.

- **Data_Doc_FqdnHash** – GUID koji jedinstveno identificira naziv glavnog računala poslužitelja.

- **Data_Doc_IdentityTelemetryId** – jednosmjerno raspršivanje korisničkog identiteta kojim se izvršava otvaranje.

- **Data_Doc_InitializationScenario** – enumeracija koja upućuje na detaljnu vrstu scenarija otvaranja datoteke.

- **Data_Doc_IOFlags** – enumeracija koja označava zastavice UI operacije otvaranja datoteke, na primjer, je li datoteka predmemorirana.

- **Data_Doc_IsCloudCollabEnabled** – je li za datoteku omogućena suradnja u oblaku.

- **Data_Doc_IsIncrementalOpen** – je li datoteka otvorena inkrementalno.

- **Data_Doc_IsOcsSupported** – podržava li datoteka uslugu suradnje u sustavu Office.

- **Data_Doc_IsOpeningOfflineCopy** – je li datoteka otvorena iz izvanmrežne predmemorirane kopije.

- **Data_Doc_IsPrefetched** – je li datoteka unaprijed dohvaćena prije operacije otvaranja.

- **Data_Doc_IsSyncBacked** – postoji li datoteka oblaka lokalno i je li sinkronizirana s poslužiteljem.

- **Data_Doc_Location** – enumeracija koja upućuje gdje se datoteka nalazi, na primjer, lokalno ili u oblaku.

- **Data_Doc_ReadOnlyReasons** – enumeracija koja označava razlog zbog kojeg je datoteka samo za čitanje.

- **Data_Doc_ResourceIdHash** – GUID koji jedinstveno identificira ID resursa poslužitelja datoteke.

- **Data_Doc_RtcType** – enumeracija koja označava vrstu kanala u stvarnom vremenu (RTC) koji se koristi u datoteci.

- **Data_Doc_ServerDocId** – GUID koji jedinstveno identificira ID dokumenta poslužitelja.

- **Data_Doc_ServerProtocol** – enumeracija koja označava poslužiteljski protokol datoteke u oblaku.

- **Data_Doc_ServerType** – enumeracija koja označava vrstu poslužitelja datoteke u oblaku.

- **Data_Doc_ServerVersion** – enumeracija koja označava verziju poslužitelja datoteke u oblaku.

- **Data_Doc_SessionId** – cijeli broj koji se povećava za 1 za svaku operaciju otvaranja datoteke u sesiji.

- **Data_Doc_SharePointServiceContext** – niz koji se koristi za korelaciju klijentskih i poslužiteljskih zapisnika, obično je vrsta identifikatora.

- **Data_Doc_SizeInBytes** – veličina datoteke u bajtovima.

- **Data_Doc_SpecialChars** – enumeracija koja označava kakav poseban znak ima URL datoteke.

- **Data_Doc_UrlHash** – GUID koji jedinstveno identificira URL datoteke.

- **Data_Doc_UsedWrsDataOnOpen** – je li datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka.

- **Data_Doc_WopiServiceId** – niz koji pokazuje iz koje usluge potječe datoteka WOPI (sučelje web-aplikacije s otvorenom platformom).

- **Data_DocumentInputCurrency** – vrsta unosa dokumenta koja se koristi u operaciji.

- **Data_DocumentOperation_AppId** – enumeracijska vrijednost koja predstavlja identifikator aplikacije.

- **Data_DocumentOperation_EndEventId** – oznaka koja predstavlja mjesto završetka operacije.

- **Data_DocumentOperation_EndReason** – enumeracijska vrijednost koja predstavlja razlog završetka.

- **Data_DocumentOperation_IsReinitialized** – inicijalizira li se ponovno dokument koji je već otvoren.

- **Data_DocumentOperation_ParamsFlags** – enumeracijske zastavice koje se koriste za početak operacije.

- **Data_DocumentOperation_TelemetryReason** – enumeracijsko predstavljanje ulazne točke za događaj otvaranja. Npr. otvoren iz MRU-a ili pregledavanja, aktivacija datoteke itd.

- **Data_DocumentOperation_isTargetECBeginEC** – je li kontekst izvršavanja cilja jednak kontekstu korištenom za otvaranje.

- **Data_FileIOInclusiveMeasurements** – vrijednost niza koja bilježi trajanje vremena provedenog u nekim pozivanjima funkcija, u obliku s oznakom funkcije i trajanjem koje uključuje trajanje pozivanja podfunkcija.

- **Data_FileIOMeasurements** – vrijednost niza koja bilježi trajanje vremena provedenog u nekim pozivanjima funkcija, u obliku s oznakom funkcije i trajanjem koje isključuje trajanje pozivanja podfunkcija.

- **Data_IsNameMissingInUrl** – upućuje na to je li naziv izveden iz URL-a.

- **Data_IsPathMissingForLocalFile** – upućuje na to je li to lokalna datoteka bez puta.

- **Data_IsUnpackedLinkSupportedForOpen** – upućuje na to je li pri otvaranju podržana veza koja se ne može zapakirati.

- **Data_LinksOpenRightScenario** – enumeracijska vrijednost za scenarij pravilnog otvaranja veza.

- **Data_OpEndEventId** – oznaka koja predstavlja mjesto završetka operacije.

- **Data_RelatedPrevOpTelemetryReason** – je li operacija povezana s prethodnom.

- **Data_StopwatchDuration** – ukupno vrijeme za događaj.

- **Data_UnpackLinkHint** – enumeracija koja predstavlja potencijalnu korisnikovu akciju na temelju veze za raspakiravanje.

- **Data_UnpackLinkPromptResult** – enumeracija koja predstavlja odgovor odzivnika veze za raspakiravanje.


#### <a name="officedocsappdocsoperationopenfromurl"></a>Office.Docs.AppDocs.OperationOpenFromUrl

Taj se događaj prikuplja za aplikacije sustava Office na uređajima sa sustavom Android, iOS, Universal ili Windows. Događaj bilježi kada se operacija otvaranja datoteke odvija na temelju URL-a te se koristi za razumijevanje i postavljanje prioriteta korisničkog iskustva na temelju podataka o operaciji otvaranja datoteke.

Prikupljaju se sljedeća polja:

- **Data_AppIdForReportEndBeforeAppKnown** – ID aplikacije kada nije poznat prije okončanja izvješća za operaciju.

- **Data_CanContinueFromOnBeforeOperationBegins** – stanje CanContinue prije uključivanja rukovatelja.

- **Data_DetachedDuration** – trajanje procesa odvajanja događaja. 

- **Data_Doc_AccessMode** – enumeracija koja upućuje na način pristupa datoteci, na primjer, samo za čitanje, za čitanje i pisanje.

- **Data_Doc_AsyncOpenKind** – enumeracija koja upućuje na vrstu asinkronog toka koji se koristi za otvaranje datoteke.

- **Data_Doc_ChunkingType** – enumeracija koja upućuje na vrstu algoritma podjele datoteke na blokove.

- **Data_Doc_EdpState** – enumeracija koja upućuje na stanje korporacijske zaštite podataka datoteke.

- **Data_Doc_Ext** – prva četiri znaka datotečnog nastavka.

- **Data_Doc_Fqdn** – naziv glavnog računala poslužitelja datoteke.

- **Data_Doc_FqdnHash** – GUID koji jedinstveno identificira naziv glavnog računala poslužitelja.

- **Data_Doc_IdentityTelemetryId** – jednosmjerno raspršivanje korisničkog identiteta kojim se izvršava otvaranje.

- **Data_Doc_InitializationScenario** – enumeracija koja upućuje na detaljnu vrstu scenarija otvaranja datoteke.

- **Data_Doc_IOFlags** – enumeracija koja označava zastavice UI operacije otvaranja datoteke, na primjer, je li datoteka predmemorirana.

- **Data_Doc_IsCloudCollabEnabled** – je li za datoteku omogućena suradnja u oblaku.

- **Data_Doc_IsIncrementalOpen** – je li datoteka otvorena inkrementalno.

- **Data_Doc_IsOcsSupported** – podržava li datoteka uslugu suradnje u sustavu Office.

- **Data_Doc_IsOpeningOfflineCopy** – je li datoteka otvorena iz izvanmrežne predmemorirane kopije.

- **Data_Doc_IsPrefetched** – je li datoteka unaprijed dohvaćena prije operacije otvaranja.

- **Data_Doc_IsSyncBacked** – postoji li datoteka oblaka lokalno i je li sinkronizirana s poslužiteljem.

- **Data_Doc_Location** – enumeracija koja upućuje gdje se datoteka nalazi, na primjer, lokalno ili u oblaku.

- **Data_Doc_ReadOnlyReasons** – enumeracija koja označava razlog zbog kojeg je datoteka samo za čitanje.

- **Data_Doc_ResourceIdHash** – GUID koji jedinstveno identificira ID resursa poslužitelja datoteke.

- **Data_Doc_RtcType** – enumeracija koja označava vrstu kanala u stvarnom vremenu (RTC) koji se koristi u datoteci.

- **Data_Doc_ServerDocId** – GUID koji jedinstveno identificira ID dokumenta poslužitelja.

- **Data_Doc_ServerProtocol** – enumeracija koja označava poslužiteljski protokol datoteke u oblaku.

- **Data_Doc_ServerType** – enumeracija koja označava vrstu poslužitelja datoteke u oblaku.

- **Data_Doc_ServerVersion** – enumeracija koja označava verziju poslužitelja datoteke u oblaku.

- **Data_Doc_SessionId** – cijeli broj koji se povećava za 1 za svaku operaciju otvaranja datoteke u sesiji.

- **Data_Doc_SharePointServiceContext** – niz koji se koristi za korelaciju klijentskih i poslužiteljskih zapisnika, obično je vrsta identifikatora.

- **Data_Doc_SizeInBytes** – veličina datoteke u bajtovima.

- **Data_Doc_SpecialChars** – enumeracija koja označava kakav poseban znak ima URL datoteke.

- **Data_Doc_UrlHash** – GUID koji jedinstveno identificira URL datoteke.

- **Data_Doc_UsedWrsDataOnOpen** – je li datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka.

- **Data_Doc_WopiServiceId** – niz koji pokazuje iz koje usluge potječe datoteka WOPI (sučelje web-aplikacije s otvorenom platformom).

- **Data_DocumentInputCurrency** – vrsta unosa dokumenta koja se koristi u operaciji.

- **Data_DocumentOperation_AppId** – enumeracijska vrijednost koja predstavlja identifikator aplikacije.

- **Data_DocumentOperation_EndEventId** – oznaka koja predstavlja mjesto završetka operacije.

- **Data_DocumentOperation_EndReason** – enumeracijska vrijednost koja predstavlja razlog završetka.

- **Data_DocumentOperation_IsReinitialized** – inicijalizira li se ponovno dokument koji je već otvoren.

- **Data_DocumentOperation_ParamsFlags** – enumeracijske zastavice koje se koriste za početak operacije.

- **Data_DocumentOperation_TelemetryReason** – enumeracijsko predstavljanje ulazne točke za događaj otvaranja. Npr. otvoren iz MRU-a ili pregledavanja, aktivacija datoteke itd.

- **Data_DocumentOperation_isTargetECBeginEC** – je li kontekst izvršavanja cilja jednak kontekstu korištenom za otvaranje.

- **Data_FileIOInclusiveMeasurements** – vrijednost niza koja bilježi trajanje vremena provedenog u nekim pozivanjima funkcija, u obliku s oznakom funkcije i trajanjem koje uključuje trajanje pozivanja podfunkcija.

- **Data_FileIOMeasurements** – vrijednost niza koja bilježi trajanje vremena provedenog u nekim pozivanjima funkcija, u obliku s oznakom funkcije i trajanjem koje isključuje trajanje pozivanja podfunkcija.

- **Data_IsNameMissingInUrl** – upućuje na to je li naziv izveden iz URL-a.

- **Data_IsPathMissingForLocalFile** – upućuje na to je li to lokalna datoteka bez puta.

- **Data_IsUnpackedLinkSupportedForOpen** – upućuje na to je li pri otvaranju podržana veza koja se ne može zapakirati.

- **Data_LinksOpenRightScenario** – enumeracijska vrijednost za scenarij pravilnog otvaranja veza.

- **Data_OpEndEventId** – oznaka koja predstavlja mjesto završetka operacije.

- **Data_RelatedPrevOpTelemetryReason** – je li operacija povezana s prethodnom.

- **Data_StopwatchDuration** – ukupno vrijeme za događaj.

- **Data_UnpackLinkHint** – enumeracija koja predstavlja potencijalnu korisnikovu akciju na temelju veze za raspakiravanje.

- **Data_UnpackLinkPromptResult** – enumeracija koja predstavlja odgovor odzivnika veze za raspakiravanje.



#### <a name="officedocsappledocsuxiossaveasthroughfilemenu"></a>Office.Docs.Apple.DocsUXiOSSaveAsThroughFileMenu 

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se bilježi kada se odvija operacija „Spremi kao” i koristi se za razumijevanje i određivanje prioriteta korisničkog iskustva na temelju podataka o radu datoteke, poput kategorija lokacije.  Operacija „Spremi kao” događa se kada god korisnik stvori novu datoteku i spremi je prvi put ili spremi kopiju postojeće datoteke na novu lokaciju.

Prikupljaju se sljedeća polja:

- **Data_OriginServiceType** – apstraktna kategorizacija izvorne lokacije datoteke kao što su „SharePoint”, „OneDrive”, „Lokalno”, „WOPI” itd., a izričito ne stvarna lokacija datoteke.

- **Data_ServiceType** – apstraktna kategorizacija nove lokacije datoteke nakon dovršetka spremanja kao što su „SharePoint”, „OneDrive” „Lokalno”, „WOPI”, itd., a izričito ne stvarna lokacija datoteke.

#### <a name="officedocsappledocsuxmacatmentioninsertedatmention"></a>Office.Docs.Apple.DocsUXMacAtMentionInsertedAtMention 

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Taj događaj bilježi kada korisnik „@” spominje drugog korisnika i koristi se za razumijevanje i postavljanje prioriteta korisničkog iskustva na temelju načina na koji korisnici surađuju s drugim korisnicima.

Prikupljaju se sljedeća polja:

- **Data_CharactersTyped** – numerička vrijednost koja označava ukupni broj znakova unesenih u spomenuti tekst „@”.

#### <a name="officedocsappledocsuxmacodspsharingwebviewsharingcompleted"></a>Office.Docs.Apple.DocsUXMacODSPSharingWebViewSharingCompleted 

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Ovaj se događaj bilježi kada korisnik izabere zajedničko korištenje dokumenta u oblaku pomoću značajke zajedničkog korištenja servisa OneDrive i koristi se za bolje razumijevanje i postavljanje prioriteta korisničkog iskustva na temelju zajedničkog korištenja dokumenata.

Prikupljaju se sljedeća polja:

- **Data_ShareType** – niz ugrađen u kod koji označava koja vrsta operacije zajedničkog korištenja je dovršena, uključujući, ali ne ograničavajući se na „Kopiraj vezu”, „Više aplikacija”, „Teams”.

- **Data_ShareWebViewMode** – niz ugrađen u kod koji označava koji način rada za zajedničko korištenje je bio aktivan kada je zajedničko korištenje dovršeno uključujući, ali ne ograničavajući se na „Upravljanje pristupom”, „Spominjanja”, „Zajedničko korištenje”.

#### <a name="officedocsuicollaborationcoauthorgalleryrowtapped"></a>Office.DocsUI.Collaboration.CoauthorGalleryRowTapped 

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Ovaj događaj bilježi kada korisnik izabere pregled popisa trenutnih suautora.  Ti se podaci koriste za bolje razumijevanje i određivanje prioriteta korisničkih iskustava koji se odnose na istodobno suautorstvo dokumenta.

Prikupljaju se sljedeća polja:

- **Data_CoauthorCount** – Numerička vrijednost koja predstavlja ukupni broj osoba koje trenutno uređuju isti dokument kao i korisnik.

#### <a name="officedocsuicollaborationcollabcornerpeoplegallerycoauthorsupdated"></a>Office.DocsUI.Collaboration.CollabCornerPeopleGalleryCoauthorsUpdated 

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj bilježi kada se promijeni broj aktivnih suautora u dokumentu u oblaku.  Ti se podaci koriste za bolje razumijevanje i određivanje prioriteta korisničkih iskustava koji se odnose na istodobno suautorstvo dokumenta.

Prikupljaju se sljedeća polja:

- **Data_CoauthorsJoined** – broj suautora koji su se pridružili dokumentu.

- **Data_CoauthorsLeft** – broj suautora koji su napustili dokument.

- **Data_NewCoauthorCount** – novi broj aktivnih suautora u dokumentu. 

- **Data_OldCoauthorCount** – prethodni broj aktivnih suautora prije ažuriranja.

- **Data_ServiceType** – apstraktna kategorizacija lokacije datoteke kao što su „SharePoint”, „OneDrive”, „Lokalno”, „WOPI” itd., a izričito ne stvarna lokacija datoteke.

#### <a name="officedocsuidocstagedocstagecreatenewfromtemplate"></a>Office.DocsUI.DocStage.DocStageCreateNewFromTemplate 

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj bilježi kada se stvara nova datoteka iz sučelja „Novo iz predloška” i koristi se za bolje razumijevanje i postavljanje prioriteta korisničkog iskustva na temelju podataka o stvaranju dokumenta.

Prikupljaju se sljedeća polja:

- **Data_InHomeTab** – Booleova vrijednost koja označava je li nova datoteka iz predloška stvorena na kartici Polazno novog sučelja datoteke.

- **Data_InSearch** – Booleova vrijednost koja označava je li datoteka stvorena kada je korisnik tražio predložak.

- **Data_IsHomeTabEnabled** – Booleova vrijednost koja označava je li kartica Polazno trenutno dostupna korisniku.

- **Data_IsRecommendedEnabled** – Booleova vrijednost koja označava je li korisniku trenutno dostupno sučelje „Preporučeno”.

- **Data_TemplateIndex** – numerički indeks datoteke predloška dok se vizualno prikazuje korisniku.

- **Data_TemplateType** – klasifikacija koja će vam pomoći u razlikovanju vrste predložaka poput, ali ne ograničavajući se na „Mrežne predloške”, predloške „Mrežnog pretraživanja”, „Lokalne” predloške.

#### <a name="officedocsuidocstagerecommendedopen"></a>Office.DocsUI.DocStage.RecommendedOpen

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj bilježi kada se operacija otvaranja datoteke odvija iz odjeljka s preporučenim datotekama galerije dokumenata i koristi se za razumijevanje i postavljanje prioriteta korisničkog iskustva na temelju podataka operacije otvaranja datoteke.

Prikupljaju se sljedeća polja:

- **Data_Success** – Booleova vrijednost koja označava je li operacija uspjela.

#### <a name="officedocsuifileoperationsdocsuifileopenmacrequired"></a>Office.DocsUI.FileOperations.DocsUIFileOpenMacRequired

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj bilježi operaciju otvaranja datoteke i koristi se za razumijevanje i postavljanje prioriteta korisničkog iskustva na temelju podataka operacije otvaranja datoteke kao što su kategorije lokacije „ServiceType” i prva četiri znaka proširenja.

Prikupljaju se sljedeća polja:

- **Data_Ext** – Datotečni nastavak ograničen na prva četiri znaka proširenja ili manje.

- **Data_ServiceType** – apstraktna kategorizacija lokacije datoteke kao što su „SharePoint”, „OneDrive”, „Lokalno”, „WOPI” itd.

#### <a name="officedocsuifileoperationsopendocumentmeasurements"></a>Office.DocsUI.FileOperations.OpenDocumentMeasurements

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na iOS platformi. Događaj bilježi kada se operacija otvaranja datoteke odvija i koristi se za razumijevanje i postavljanje prioriteta korisničkog iskustva na temelju podataka operacije otvaranja datoteke.

Prikupljaju se sljedeća polja:

- **Data_AppDuration** – trajanje provedeno u obradi aplikacije tijekom operacije otvaranja datoteke.

- **Data_BootDuration** – trajanje postupka pokretanja otvorene datoteke.

- **Data_ClickOrigin** – niz koji označava iz kojeg je dijela veza nastala kada je korisnik kliknuo vezu u aplikaciji iOS Outlook kako bi otvorio datoteku u aplikaciji Office.

- **Data_ClickTime** – vrijeme Unix epohe kada je korisnik kliknuo vezu u aplikaciji iOS Outlook kako bi otvorio datoteku u aplikaciji Office.

- **Data_ClosePreviouslyOpenedMarkers** – vrijednost niza koja evidentira trajanje vremena između nekih poziva funkcije, u obliku s ID-om i trajanjem funkcije.

- **Data_DetachedDuration** – trajanje procesa odvajanja događaja. 

- **Data_Doc_AccessMode** – enumeracija koja upućuje na način pristupa datoteke, na primjer, samo za čitanje, za čitanje i pisanje.

- **Data_Doc_AsyncOpenKind** – enumeracija koja upućuje na vrstu asinkronog toka koji se koristi za otvaranje datoteke.

- **Data_Doc_ChunkingType** – enumeracija koja upućuje na vrstu algoritma dijeljenja datoteke.

- **Data_Doc_EdpState** – enumeracija koja upućuje na stanje korporacijske zaštite podataka datoteke.

- **Data_Doc_Ext** – Datotečni nastavak datoteke.

- **Data_Doc_Fqdn** – naziv glavnog računala poslužitelja datoteke.

- **Data_Doc_FqdnHash** – GUID koji jedinstveno identificira naziv glavnog računala poslužitelja.

- **Data_Doc_IdentityTelemetryId** – GUID koji jedinstveno identificira identitet koji se koristi za otvaranje datoteke.

- **Data_Doc_InitializationScenario** – enumeracija koja upućuje na detaljnu vrstu scenarija otvaranja datoteke.

- **Data_Doc_IOFlags** – enumeracija koja označava zastavice UI operacije otvaranja datoteke, na primjer, ako je datoteka predmemorirana ili ne.

- **Data_Doc_IsCloudCollabEnabled**– bez obzira na to je li za datoteku omogućena suradnja u oblaku.

- **Data_Doc_IsIncrementalOpen** – bez obzira na to je li datoteka otvorena inkrementalno ili ne.

- **Data_Doc_IsOcsSupported** – bez obzira na to podržava li datoteka uslugu suradnje u sustavu Office.

- **Data_Doc_IsOpeningOfflineCopy** – bez obzira na to je li datoteka otvorena iz izvanmrežne predmemorirane kopije.

- **Data_Doc_IsPrefetched** – bez obzira na to je li datoteka unaprijed dohvaćena prije operacije otvaranja.

- **Data_Doc_IsSyncBacked** – bez obzira na to postoji li datoteka oblaka lokalno i je li sinkronizirana s poslužiteljem.

- **Data_Doc_Location** – enumeracija koja upućuje gdje se datoteka nalazi, na primjer, lokalno ili u oblaku.

- **Data_Doc_ReadOnlyReasons** – enumeracija koja označava razlog zbog kog je datoteka samo za čitanje.

- **Data_Doc_ResourceIdHash** – GUID koji jedinstveno identificira ID resursa poslužitelja datoteke.

- **Data_Doc_RtcType** – enumeracija koja označava vrstu kanala u stvarnom vremenu (RTC) koji se koristi u datoteci.

- **Data_Doc_ServerDocId** – GUID koji jedinstveno identificira ID dokumenta poslužitelja.

- **Data_Doc_ServerProtocol** – enumeracija koja označava poslužiteljski protokol datoteke u oblaku.

- **Data_Doc_ServerType** – enumeracija koja označava vrstu poslužitelja datoteke u oblaku.

- **Data_Doc_ServerVersion** – enumeracija koja označava verziju poslužitelja datoteke u oblaku.

- **Data_Doc_SessionId** – cijeli broj koji se povećava za 1 za svaku operaciju otvaranja datoteke u sesiji.

- **Data_Doc_SharePointServiceContext** – niz koji se koristi za povezivanje klijentskih i poslužiteljskih zapisnika, obično je vrsta ID-a.

- **Data_Doc_SizeInBytes** – veličina datoteke u bajtovima.

- **Data_Doc_SpecialChars** – enumeracija koja označava kakav poseban znak ima URL datoteke.

- **Data_Doc_UrlHash** – GUID koji jedinstveno identificira URL datoteke.

- **Data_Doc_UsedWrsDataOnOpen** – bez obzira na to je li datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka.

- **Data_Doc_WopiServiceId** – niz koji pokazuje iz koje usluge je datoteka WOPI (sučelje web-aplikacije s otvorenom platformom).

- **Data_HWModel** – vrijednost niza kojom se bilježi model uređaja iPad ili uređaja iPhone.

- **Data_InclusiveMeasurements** – vrijednost niza koja evidentira trajanje vremena provedenog u nekim pozivima funkcije, u obliku s oznakom funkcije i trajanju koje uključuje trajanje poziva podfunkcije.

- **Data_InitializationReason** – enumeracija koja označava kako se datoteka otvara, na primjer, iz kojeg elementa korisničkog sučelja ili je pokreće druga aplikacija.

- **Data_IsDocumentAlreadyOpen** – je li datoteka već otvorena ili ne.

- **Data_IsInterrupted** – je li postupak otvaranja datoteke prekinut prelaskom aplikacije na pozadinu ili ne.

- **Data_Measurements** – vrijednost niza koja evidentira trajanje vremena provedenog u nekim pozivima funkcije, u obliku s oznakom funkcije i trajanju koje isključuje trajanje poziva podfunkcije.

- **Data_OpenInPlace** – bez obzira na to treba li se datoteka kopirati u spremnik za testiranje u sustavu Office prije no što ga korisnik otvori.

- **Data_OpenStartTime** – vrijeme Unix epohe kada je počelo otvaranje datoteke.

- **Data_SilhouetteDuration** – trajanje prikazivanja otvaranja datoteke.

- **Data_SourceApplication** – niz koji pokazuje ID kompleta izvorišne aplikacije kada je druga aplikacija pokrenula otvaranje datoteke.

- **Data_StopwatchDuration** – trajanje od početka događaja do kraja događaja.

- **Data_TimeSplitMeasurements** – vrijednost niza koja evidentira trajanje vremena provedenog u nekim pozivima funkcije, u obliku s oznakom funkcije, početnom vremenskom oznakom i trajanjem.

#### <a name="officedocsuifileoperationsopenfilewithreason"></a>Office.DocsUI.FileOperations.OpenFileWithReason 

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj bilježi operaciju otvaranja datoteke i koristi se za razumijevanje i postavljanje prioriteta korisničkog iskustva na temelju podataka operacije otvaranja datoteke kao što su kategorije lokacije „ServiceType”, a odakle je u aplikaciji korisnik zatražio otvaranje datoteke.

Prikupljaju se sljedeća polja:

- **Data_IsCandidateDropboxFile** – ovo je Booleova vrijednost koja se zapisuje ako uvidom u putanju datoteke mislimo da bi mogla biti iz mape koju sinkronizira DropBox.

- **Data_IsSignedIn** – bez obzira na to je li korisnik prijavljen ili ne kada je datoteka spremljena.

- **Data_OpenReason** – otvoreni razlog numerička je vrijednost koja označava odakle je unutar aplikacije korisnik otvorio datoteku.

- **Data_ServiceType** – apstraktna numerička kategorizacija lokacije datoteke kao što su „SharePoint”, „OneDrive”, „Lokalno”, „WOPI” itd., a izričito ne stvarna lokacija datoteke.

#### <a name="officedocsuifileoperationssavetourl"></a>Office.DocsUI.FileOperations.SaveToURL

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se bilježi kada se odvija operacija „Spremi kao” i koristi se za razumijevanje i određivanje prioriteta korisničkog iskustva na temelju podataka o radu datoteke, poput kategorija lokacije i prva četiri znaka proširenja.  Operacija „Spremi kao” događa se kada god korisnik stvori novu datoteku i spremi je prvi put ili spremi kopiju postojeće datoteke na novu lokaciju.

Prikupljaju se sljedeća polja:

- **Data_FileExtension** – prva četiri znaka proširenja nove datoteke.

- **Data_IsNewFileCreation** – označava je li operacija spremanja za novu datoteku ili kopiju postojeće datoteke.

- **Data_IsSignedIn** – bez obzira na to je li korisnik prijavljen ili ne kada je datoteka spremljena.

- **Data_SaveErrorCode** – numerička vrijednost koja se postavlja ako postoji pogreška koja omogućuje prepoznavanje vrste pogreške.

- **Data_SaveErrorDomain** – određuje domenu koda SaveErrorCode kako je definirano u SaveErrorDomains tvrtke Apple „to su proizvoljni nizovi koji se koriste za razlikovanje grupe kodova”.

- **Data_SaveLocation** – apstraktna kategorizacija lokacije datoteke kao što su „SharePoint”, „OneDrive”, „Lokalno”, „WOPI” itd., a izričito ne stvarna lokacija datoteke.

- **Data_SaveOperationType** – numerička vrijednost definirana u grupi vrijednosti tvrtke Apple NSSaveOperationType.


#### <a name="officedocsuisharinguicloudupsellshown"></a>Office.DocsUI.SharingUI.CloudUpsellShown 

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Ovaj se događaj bilježi kada korisnik prođe kroz nadogradnju dokumenta u protok oblaka.  Ti se podaci koriste za bolje razumijevanje i određivanje prioriteta korisničkih iskustava povezanih s premještanjem dokumenata na lokacije u oblaku.

Prikupljaju se sljedeća polja:

- **Data_FileStyle** – numerička vrijednost koja pokazuje iz kojeg scenarija je prikazano iskustvo nadogradnje, primjerice, pomoću prekidača za automatsko spremanje ili gumba za zajedničko korištenje.

- **Data_FileType** – prva četiri znaka proširenja trenutne datoteke.

- **Data_InDocStage** – Booleova vrijednost koja označava je li iskustvo nadogradnje prikazano iz galerije dokumenta ili iz prozora dokumenta.

- **Data_IsDocumentOpened** – Booleova vrijednost koja označava je li trenutni dokument za koji se prikazuje iskustvo nadogradnje također otvoren.

- **Data_IsDraft** – Booleova vrijednost koja označava je li trenutna datoteka ikada bila spremljena.

- **Data_IsSheetModal** – Booleova vrijednost koja označava je li iskustvo nadogradnje predstavljeno modalno ili ne.

#### <a name="officedocsuisharinguicloudupsellupload"></a>Office.DocsUI.SharingUI.CloudUpsellUpload 

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Ovaj se događaj bilježi kada korisnik odluči prenijeti novu ili lokalnu datoteku u oblak i rezultat te operacije.  Ti se podaci koriste za bolje razumijevanje i određivanje prioriteta korisničkih iskustava povezanih s premještanjem dokumenata na lokacije u oblaku.

Prikupljaju se sljedeća polja:

- **Data_FileStyle** – numerička vrijednost koja pokazuje iz kojeg scenarija je prikazano iskustvo nadogradnje poput prekidača za automatsko spremanje ili gumba za zajedničko korištenje.

- **Data_FileType** – prva četiri znaka proširenja trenutne datoteke.

- **Data_InDocStage** – Booleova vrijednost koja označava je li iskustvo nadogradnje prikazano iz galerije dokumenta ili iz prozora dokumenta.

- **Data_IsDefaultServiceLocation** – Booleova vrijednost koja označava je li odabrana lokacija za učitavanje dokumenta zadana lokacija.

- **Data_IsDocumentOpened** – Booleova vrijednost koja označava je li trenutni dokument za koji se prikazuje iskustvo nadogradnje također otvoren.

- **Data_IsDraft** – Booleova vrijednost koja označava je li trenutna datoteka ikada bila spremljena.

- **Data_IsSheetModal** – Booleova vrijednost koja označava je li iskustvo nadogradnje predstavljeno modalno ili ne.

- **Data_LocationServiceType** – apstraktna kategorizacija lokacije datoteke kao što su „SharePoint”, „OneDrive”, „Lokalno”, „WOPI” itd., a izričito ne stvarna lokacija datoteke.

- **Data_UploadAction** – niz ugrađen u kod koji označava je li prijenos bila operacija premještanja ili kopiranja.

- **Data_UploadResult** – niz ugrađen u kod koji označava rezultat pokušaja prijenosa, uključujući ali ne ograničavajući se na: „Uspjeh”, „Korisnik je otkazao prijenos” i „Predautorizacija nije uspjela”.

#### <a name="officedocsuisharinguicopylinkoperation"></a>Office.DocsUI.SharingUI.CopyLinkOperation

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Ovaj se događaj bilježi kada korisnik izabere zajedničko korištenje generiranjem veze na dokument u oblaku i koristi se za bolje razumijevanje i postavljanje prioriteta korisničkog iskustva na temelju zajedničkog korištenja dokumenata.

Prikupljaju se sljedeća polja:

- **Data_ServiceType** – apstraktna kategorizacija lokacije datoteke kao što su „SharePoint”, „OneDrive”, „Lokalno”, „WOPI” itd., a izričito ne stvarna lokacija datoteke.

- **Data_LinkType** – niz ugrađen u kod koji opisuje izvedenu vrstu poziva poput „ViewOnly” i „ViewAndEdit”.

- **Data_ShareScenario** – opis lokacije niza ugrađenog u kod unutar korisničkog sučelja aplikacije odakle se datoteka zajednički koristi uključujući ali ne ograničavajući se na „FileMenu”, „OpenTabShareActionMenu”, „RecentTabShareActionMenu”.

#### <a name="officedocsuisharinguidocsuionedriveshare"></a>Office.DocsUI.SharingUI.DocsUIOneDriveShare 

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Ovaj se događaj bilježi kada korisnik izabere zajedničko korištenje dokumenta u oblaku pomoću značajke zajedničkog korištenja servisa OneDrive i koristi se za bolje razumijevanje i postavljanje prioriteta korisničkog iskustva na temelju zajedničkog korištenja dokumenata.

Prikupljaju se sljedeća polja:

- **Data_ODSPShareWebviewShareError** – Ako iskustvo zajedničkog korištenja doživi pogrešku, to je numerička vrijednost koja će vam pomoći da identificirate razlog neuspjeha.

- **Data_ODSPShareWebviewShareGrantAccessResult** – Booleova vrijednost koja kada je vrijednost „true“ ukazuje da je lagana operacija zajedničkog korištenja uspješno dovršena.

- **Data_ODSPShareWebviewShareSuccessType** – Kada se operacija zajedničkog korištenja uspješno dovrši, to je numerička vrijednost koja se koristi za određivanje vrste završetka operacije zajedničkog korištenja.

- **Data_WebViewInfoResult** – Ako se korisničko sučelje ne učita, to je numerička vrijednost koja će vam pomoći u prepoznavanju razloga za neuspjeh. 

- **Data_WebViewLoadTimeInMs** – Numerička vrijednost koja bilježi vrijeme potrebno za učitavanje web korisničkog sučelja.

#### <a name="officedocsuisharinguiinvitepeople"></a>Office.DocsUI.SharingUI.InvitePeople 

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Ovaj se događaj bilježi kada korisnik odluči pozvati ljude u dokument u oblaku i koristi se za bolje razumijevanje i postavljanje prioriteta korisničkog iskustva na temelju zajedničkog korištenja dokumenata.

Prikupljaju se sljedeća polja:

- **Data_ServiceType** – apstraktna kategorizacija lokacije datoteke kao što su „SharePoint”, „OneDrive”, „Lokalno”, „WOPI” itd., a izričito ne stvarna lokacija datoteke.

- **Data_InviteeCount** – ukupni broj kontakata pozvanih u dokument u jednoj akciji poziva.

- **Data_LinkType** – niz ugrađen u kod koji opisuje izvedenu vrstu poziva poput „ViewOnly” i „ViewAndEdit”.

- **Data_MessageLength** – numerički broj ukupnog broja znakova poslanih u pozivnoj poruci.

- **Data_ShareScenario** – opis lokacije niza ugrađenog u kod unutar korisničkog sučelja aplikacije odakle se datoteka zajednički koristi uključujući ali ne ograničavajući se na „FileMenu”, „OpenTabShareActionMenu”, „RecentTabShareActionMenu”.

#### <a name="officedocsuisharinguisendacopyoperation"></a>Office.DocsUI.SharingUI.SendACopyOperation

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Ovaj se događaj bilježi kada korisnik odluči poslati kopiju dokumenta i koristi se za bolje razumijevanje i postavljanje prioriteta korisničkog iskustva na temelju zajedničkog korištenja dokumenata.

Prikupljaju se sljedeća polja:

- **Data_IsHomeTabEnabled** – Booleova vrijednost koja označava je li kartica Polazno trenutno dostupna korisniku.

- **Data_IsRecommendedEnabled** – Booleova vrijednost koja označava je li korisniku trenutno dostupno sučelje „Preporučeno”.

- **Data_OperationType** – numerička vrijednost koja označava koja je vrsta slanja postupka kopiranja koja se odvija kao što je slanje kopije u poruci e-pošte ili slanje kopije pomoću kontrole za zajedničko korištenje tvrtke Apple.

- **Data_ServiceType** – apstraktna kategorizacija lokacije datoteke kao što su „SharePoint”, „OneDrive”, „Lokalno”, „WOPI” itd., a izričito ne stvarna lokacija datoteke.

- **Data_ShareFileType** – Niz ugrađen u kod opisa vrste objekta koji se zajednički koristi uključujući ali ne ograničavajući se na „Dokument”, „PDF”, „Slika”.

- **Data_ShareScenario** – opis lokacije niza ugrađenog u kod unutar korisničkog sučelja aplikacije odakle se datoteka zajednički koristi uključujući ali ne ograničavajući se na „FileMenu”, „OpenTabShareActionMenu”, „RecentTabShareActionMenu”.

- **Data_SharingService** – Booleova vrijednost koja označava je li datoteka stvorena kada je korisnik tražio predložak.

#### <a name="officedocsuisharinguiupsellshare"></a>Office.DocsUI.SharingUI.UpsellShare 

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Ovaj se događaj bilježi kada korisnik prođe kroz nadogradnju dokumenta u protok oblaka prilikom pokušaja zajedničkog korištenja dokumenta.  Ti se podaci koriste za bolje razumijevanje i određivanje prioriteta korisničkih iskustava povezanih s premještanjem dokumenata na lokacije u oblaku.

Prikupljaju se sljedeća polja:

- **Data_FileOperationResult** – numerička vrijednost koja pokazuje je li operacija uspjela.

- **Data_HostedFromDocStage** – Booleova vrijednost koja označava prolazi li korisnik kroz nadogradnju na protok oblaka iz sučelja DocStage ili iz otvorenog dokumenta.

- **Data_isLocalCopyOn** – Booleova vrijednost koja označava je li korisnik odlučio zadržati lokalnu kopiju dokumenta koji se prenosi na oblak ili premjestiti postojeći dokument u oblak.

- **Data_NewFileType** – apstraktna kategorizacija lokacije nove lokacije datoteke kao što su „SharePoint”, „OneDrive”, „Lokalno”, „WOPI” itd., a izričito ne stvarna lokacija datoteke.

- **Data_OriginalFileType** – apstraktna kategorizacija lokacije datoteke kao što su „SharePoint”, „OneDrive”, „Lokalno”, „WOPI” itd., a izričito ne stvarna lokacija datoteke.

- **Data_UploadButtonPressed** – Booleova vrijednost koja označava je li korisnik odlučio prenijeti trenutni dokument u oblak.

- **Data_UploadError** – Numerička vrijednost koja pokazuje vrstu pogreške koja se dogodila ako operacija prijenosa ne uspije.

- **Data_UpsellAppearsFromDelegate** – Booleova vrijednost koja označava je li prikaz prikazan iz izbornika za zajedničko korištenje. 

#### <a name="officeextensibilitycatalogexchangeprocessentitlement"></a>Office.Extensibility.Catalog.ExchangeProcessEntitlement

Podaci vezani uz obradu pojedinačnih prava dodatka koji je dodijelio administrator klijenta sustava Office 365.

Koristi se u izradi grafikona (zahtijeva ga upravljanje timom) uspjeha klijenata i analizu korisničkih problema.

Prikupljaju se sljedeća polja:

  - **AppVersion** – verzija glavne aplikacije dodatka

  - **SolutionId** – GUID koji predstavlja jedinstveni dodatak

  - **TelemetryId** – GUID koji predstavlja jedinstvenog korisnika

#### <a name="officeextensibilitycatalogexchangeprocessmanifest"></a>Office.Extensibility.Catalog.ExchangeProcessManifest

Podaci vezani uz obradu pojedinačnog manifesta za dodatak koji je dodijelio administrator klijenta sustava Office 365. Koristi se za analizu problema korisnika i izradu grafikona uspjeha korisnika.
 
Prikupljaju se sljedeća polja:

- **AppVersion** – verzija aplikacije

- **IsAllReturnedManifestsParsed** – Booleova vrijednost koja označava da smo raščlanili sve vraćene manifeste

- **IsAppCommand** – Booleova vrijednost koja označava je li ovo aplikacija za upravljanje aplikacijama 

- **ReturnedManifestsParsed** – broj raščlanjenih manifesta

- **SolutionId** – ID rješenja

- **TelemetryId** – telemetrijski ID na temelju prijavljenog identiteta

#### <a name="officeextensibilityodpappcommandsribbonclick"></a>Office.Extensibility.ODPAppCommandsRibbonClick

Prikuplja podatke o tome je li klik na prilagođenu kontrolu dodatka bio uspješan ili nije. Koristi se za prepoznavanje problema u interakciji korisnika s kontrolama dodatka.
 
Prikupljaju se sljedeća polja:

- **CommandActionType** – vrsta naredbe dodatka

- **CommandLabel** – oznaka naredbe na koju se kliknulo

- **SolutionId** – ID rješenja

#### <a name="officefeedeventsinitializing"></a>Office.Feed.Events.Initializing

Taj se događaj prikuplja kada se sažetak sadržaja počne pokretati. Taj se događaj upotrebljava da bi se pokazalo da se sažetak sadržaja pokreće te da bi se dijagnosticirali problemi s pouzdanošću prilikom pokretanja sažetka sadržaja.

- **AppInfo.Language** – jezik aplikacije u obliku jezične oznake IETF.

- **AppInfo.Name** – ime komponente koja se upotrebljava (Sažetak sustava Office).

- **AppInfo.Version** – verzija aplikacije.

- **clientCorrelationId** – globalno jedinstveni identifikator za sesiju aplikacije.

- **clientType** – aplikacija na kojoj se komponenta izvodi.

- **DeviceInfo.Make** – proizvođač uređaja ili naziv OEM uređaja.

- **DeviceInfo.NetworkProvider** – mrežni ili mobilni operator, kao što je „AT&T”.

- **DeviceInfo.NetworkType** – vrsta mrežne povezivosti uređaja koji se upotrebljava, npr. „Ožičena”, "WiFi" ili "WWAN" (podatkovna/mobilna).

- **DeviceInfo.OsName** – naziv operacijskog sustava uređaja.

- **DeviceInfo.SDKUid** – jedinstveno označava uređaj iz telemetrijske perspektive SDK-a.

- **eventId** – identifikator imena događaja. 

- **EventInfo.SdkVersion** – verzija telemetrijskog SDK-a koji upotrebljava klijent radi izrade događaja.

- **eventpriority** – vrijednost numeriranje za prioritet slanja događaja.

- **feature** – upotrebljava se za grupiranje raznih događaja iste značajke.

- **hostAppRing** – populacija korisnika kojima je aplikacija raspoređena.

- **properties** – sadržava dodatna svojstva metapodataka prikupljenih za svaki događaj.
        
    - **ClientTimeStamp** – timestamp kada je događaj prijavljeni u klijentu.

- **publicEventName** – naziv događaja u javnom sučelju.  

- **region** – zemljopisno područje usluge sažetka sadržaja s kojim je korisnik povezan. 

- **tenantAadObjectId** – globalno jedinstveni identifikator za korisnikovu klijentelu velikih tvrtki.

- **type** – vrsta zapisanog događaja, npr. Praćenje, Pogreška, Događaj, QoS.

- **userAadObjectId** – globalno jedinstveni identifikator korisnika za Microsoftov račun za velike tvrtke.

- **UserInfo.Id** – globalno jedinstveni identifikator korisnika za Microsoftov račun za velike tvrtke.

- **UserInfo.IdType** – određuje vrstu korisničkog ID-ja. 

- **UserInfo.Language** – jezik aplikacije u obliku jezične oznake IETF.

- **UserInfo.MsaId** – globalno jedinstveni identifikator korisnika za Microsoftov potrošački račun.

- **UserInfo.OMSTenantId** – klijent s kojim je povezana pretplata korisnika. Omogućuje klasifikaciju problema i utvrđivanje je li problem rasprostranjen ili ograničen na skup korisnika ili određenog klijenta.

- **UserInfo.TimeZone** – korisnikova vremenska zona u odnosu na UTC.

- **userPuid** – globalno jedinstveni identifikator korisnika za Microsoftov potrošački račun.

- **version** ― verzija klijenta sažetka sadržaja.

#### <a name="officefeedeventsofficefeeddidappear"></a>Office.Feed.Events.OfficeFeedDidAppear

Taj se događaj prikuplja kada se sažetak sadržaja prikazuje korisniku. Taj se događaj upotrebljava da bi se potvrdilo da je sažetak dovršio korak inicijalizacije te da bi se dijagnosticirali problemi s pouzdanošću prilikom pokretanja sažetka sadržaja.

- **AppInfo.Language** – jezik aplikacije u obliku jezične oznake IETF.

- **AppInfo.Name** – ime komponente koja se upotrebljava (Sažetak sustava Office).

- **AppInfo.Version** – verzija aplikacije.

- **bridgeWaitingTime** – metrika za dijagnosticiranje performansi u prikazivanju sažetka sadržaja.

- **clientCorrelationId** – globalno jedinstveni identifikator za sesiju aplikacije.

- **clientScenario** – diskriminator scenarija za različite varijante sažetka sadržaja.

- **ClientTimeStamp** – timestamp kada je događaj prijavljeni u klijentu.

- **clientType** – aplikacija na kojoj se komponenta izvodi.

- **DeviceInfo.Make** – proizvođač uređaja ili naziv OEM uređaja.

- **DeviceInfo.NetworkProvider** – mrežni ili mobilni operator, kao što je „AT&T”.

- **DeviceInfo.NetworkType** – vrsta mrežne povezivosti uređaja koji se upotrebljava, npr. „Ožičena”, "WiFi" ili "WWAN" (podatkovna/mobilna).

- **DeviceInfo.OsName** – naziv operacijskog sustava uređaja.

- **DeviceInfo.SDKUid** – jedinstveno označava uređaj iz telemetrijske perspektive SDK-a.

- **eventId** – identifikator imena događaja.

- **EventInfo.SdkVersion** – verzija telemetrijskog SDK-a koji upotrebljava klijent radi izrade događaja.

- **eventpriority** – vrijednost numeriranje za prioritet slanja događaja.

- **feature** – upotrebljava se za grupiranje raznih događaja iste značajke.

- **hostAppRing** – populacija korisnika kojima je aplikacija raspoređena.

- **properties** – sadržava dodatna svojstva metapodataka prikupljenih za svaki događaj. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

- **publicEventName** – naziv događaja u javnom sučelju.  

- **region** – zemljopisno područje usluge sažetka sadržaja s kojim je korisnik povezan. 

- **renderTime** – metrika za dijagnosticiranje performansi u prikazivanju sažetka sadržaja.

- **tenantAadObjectId** – globalno jedinstveni identifikator za korisnikovu klijentelu velikih tvrtki.

- **type** – vrsta zapisanog događaja, npr. Praćenje, Pogreška, Događaj, QoS.

- **userAadObjectId** – globalno jedinstveni identifikator korisnika za Microsoftov račun za velike tvrtke.

- **UserInfo.Id** – globalno jedinstveni identifikator korisnika za Microsoftov račun za velike tvrtke.

- **UserInfo.IdType** – određuje vrstu korisničkog ID-ja. 

- **UserInfo.Language** – jezik aplikacije u obliku jezične oznake IETF.

- **UserInfo.MsaId** – globalno jedinstveni identifikator korisnika za Microsoftov potrošački račun.

- **UserInfo.OMSTenantId** – klijent s kojim je povezana pretplata korisnika. Omogućuje klasifikaciju problema i utvrđivanje je li problem rasprostranjen ili ograničen na skup korisnika ili određenog klijenta.

- **UserInfo.TimeZone** – korisnikova vremenska zona u odnosu na UTC.

- **userPuid** – globalno jedinstveni identifikator korisnika za Microsoftov potrošački račun.

- **version** ― verzija klijenta sažetka sadržaja.


#### <a name="officefeedbacksurveyfloodgateclientsurveytracked"></a>Office.Feedback.Survey.FloodgateClient.SurveyTracked

Prati kada uređaj koji ispunjava uvjete za upitnik pokrene aplikaciju. Upotrebljava se za procjenu stanja procesa odabira korisnika upitnika i osiguravanje signala koji se upotrebljava za utvrđivanje radi li funkcija analize korisničkih problema i stanja pravilno.

Prikupljaju se sljedeća polja:

- **ExpirationTimeUTC** – datum/vrijeme isteka upitnika

- **SurveyName** – naziv prikazanog upitnika

- **SurveyId** – jedinstvena instanca kampanje

- **UniqueId** – ID za identifikaciju individualnog elementa telemetrije

#### <a name="officefeedbacksurveyfloodgateclienttriggermet"></a>Office.Feedback.Survey.FloodgateClient.TriggerMet

Prati kada je uređaj ispunio uvjete za prikaz ankete. Upotrebljava se za procjenu stanja procesa aktivacije upitnika i osiguravanje signala koji se upotrebljava za utvrđivanje radi li funkcija analize korisničkih problema i stanja pravilno.

Prikupljaju se sljedeća polja:

- **ExpirationTimeUTC** – datum/vrijeme isteka upitnika

- **SurveyName** – naziv prikazanog upitnika

- **SurveyId** – jedinstvena instanca kampanje

- **UniqueId** – ID za identifikaciju individualnog elementa telemetrije

#### <a name="officefeedbacksurveyfloodgateclientuserselected"></a>Office.Feedback.Survey.FloodgateClient.UserSelected

Prati kada je uređaj odabran za upitnik. Upotrebljava se za procjenu stanja procesa odabira korisnika upitnika i osiguravanje signala koji se upotrebljava za utvrđivanje radi li funkcija analize korisničkih problema i stanja pravilno.

Prikupljaju se sljedeća polja:

- **ExpirationTimeUTC** – datum/vrijeme isteka upitnika

- **SurveyName** – naziv prikazanog upitnika

- **SurveyId** – jedinstvena instanca kampanje

- **UniqueId** – ID za identifikaciju individualnog elementa telemetrije

#### <a name="officefeedbacksurveyuiandroid"></a>Office.Feedback.Survey.UI.Android

Na uređaju sa sustavom Android prati kada korisnik na uređaju komunicira s upitom upitnika i korisničkim sučeljem upitnika. Upotrebljava se za procjenu stanja cijelog iskustva upitnika i osiguravanje signala koji se upotrebljava za utvrđivanje radi li funkcija analize korisničkih problema i stanja pravilno.

Prikupljaju se sljedeća polja:

- **ExpirationTimeUTC** – datum/vrijeme isteka upitnika

- **SurveyName** – naziv prikazanog upitnika

- **SurveyId** – jedinstvena instanca kampanje

- **UniqueId** – ID za identifikaciju individualnog elementa telemetrije

#### <a name="officefeedbacksurveyuiios"></a>Office.Feedback.Survey.UI.IOS

Na uređaju sa sustavom iOS prati kada korisnik na uređaju komunicira s upitom upitnika i korisničkim sučeljem upitnika. Upotrebljava se za procjenu stanja cijelog iskustva upitnika i osiguravanje signala koji se upotrebljava za utvrđivanje radi li funkcija analize korisničkih problema i stanja pravilno.

Prikupljaju se sljedeća polja:

- **ExpirationTimeUTC** – datum/vrijeme isteka upitnika

- **SurveyName** – naziv prikazanog upitnika

- **SurveyId** – jedinstvena instanca kampanje

- **UniqueId** – ID za identifikaciju individualnog elementa telemetrije

#### <a name="officefeedbacksurveyuimac"></a>Office.Feedback.Survey.UI.Mac

Na uređaju Mac prati kada korisnik na uređaju komunicira s upitom upitnika i korisničkim sučeljem upitnika. Upotrebljava se za procjenu stanja cijelog iskustva upitnika i osiguravanje signala koji se upotrebljava za utvrđivanje radi li funkcija analize korisničkih problema i stanja pravilno.

Prikupljaju se sljedeća polja:

- **ExpirationTimeUTC** – datum/vrijeme isteka upitnika

- **SurveyName** – naziv prikazanog upitnika

- **SurveyId** – jedinstvena instanca kampanje

- **UniqueId** – ID za identifikaciju individualnog elementa telemetrije

#### <a name="officefeedbacksurveyuiwin32"></a>Office.Feedback.Survey.UI.Win32

Na uređaju Win32 prati kada korisnik na uređaju komunicira s upitom upitnika i korisničkim sučeljem upitnika. Upotrebljava se za procjenu stanja cijelog iskustva upitnika i osiguravanje signala koji se upotrebljava za utvrđivanje radi li funkcija analize korisničkih problema i stanja pravilno.

Prikupljaju se sljedeća polja:

- **ExpirationTimeUTC** – datum/vrijeme isteka upitnika

- **SurveyName** – naziv prikazanog upitnika

- **SurveyId** – jedinstvena instanca kampanje

- **UniqueId** – ID za identifikaciju individualnog elementa telemetrije

#### <a name="officefeedbacksurveyuiwin32toast"></a>Office.Feedback.Survey.UI.Win32.Toast

Prati kada se prikaže upit za upitnik. Upotrebljava se za procjenu stanja procesa upita upitnika i osiguravanje signala koji se upotrebljava za utvrđivanje radi li funkcija analize korisničkih problema i stanja pravilno.

Prikupljaju se sljedeća polja:

- **ExpirationTimeUTC** – datum/vrijeme isteka upitnika

- **SurveyName** – naziv prikazanog upitnika

- **SurveyId** – jedinstvena instanca kampanje

- **UniqueId** – ID za identifikaciju individualnog elementa telemetrije

#### <a name="officefileiocsiccachedfilecsiloadfilebasic"></a>Office.FileIO.CSI.CCachedFileCsiLoadFileBasic

Omogućuje da utvrdimo je li datoteka uspješno otvorena u FIO sloju. Koristi se za stanje i nadzor značajke.

Prikupljaju se sljedeća polja:

  - **Activity.Group –** oznaka koja omogućuje postavljanje grupiranja događaja nadzora za upravljanje ukupnim uspjehom

  - **Activity.IsHVA –** zastavica koja označava da je događaj ključan za uspjeh korisnika

  - **Data.AsyncOpen –** zastavica koja označava da se u otvorenom nalazi sadržaj koji je primljen nakon otvaranja glavnog tijela

  - **Data.CacheFileId –** povezuje se s telemetrijom predmemorije dokumenta sustava Office radi omogućivanja analize utjecaja problema s predmemorijom na korisničko iskustvo
 
  - **Data. CFREnabled** – ukazuje da je za sesiju omogućen CacheFileRuntime.

  - **Data.CFRFailure** – Ukazuje da je CacheFileRuntime naišao na pogrešku.
  
  - **Data.CoauthStatus –** izvješćuje status suradnje dokumenta pri otvaranju

  - **Data.CountOfMultiRoundTripsDownload –** broj povratnih prijenosa na poslužitelj koji se koristi za otklanjanje poteškoća s performansama i mrežom

  - **Data.CountOfMultiRoundTripsUpload –** broj povratnih prijenosa na poslužitelj koji se koristi za otklanjanje poteškoća s performansama i mrežom

  - **Data.DialogId –** postavljeno ako je otvoren dijaloški okvir korisničkog sučelja tijekom otvaranja, što upućuje da je poruka upozorenja prikazana korisniku

  - **Data.DidFallbackToDAV –** postavljeno ako je dokument otvoren pomoću starijeg protokola za prijenos datoteka

  - **Data.Doc.AccessMode –** dokument je samo za čitanje/uređivanje

  - **Data.Doc.AssistedReadingReasons –** postavljeno ako dokument ima aktiviranu zaštitu elektroničkih podataka

  - **Data.Doc.AsyncOpenKind –** označava je li otvorena predmemorirana verzija dokumenta u oblaku i koja je logika za asinkrono osvježavanje korištena.

  - **Data.Doc.ChunkingType –** jedinice koje se koriste za inkrementalno otvaranje dokumenta

  - **Data.Doc.EdpState –** postavka zaštite elektroničkih podataka za dokument

  - **Data.Doc.Ext –** nastavak dokumenta (docx/xlsb/pptx itd.)

  - **Data.Doc.Extension –** zastarjelo

  - **Data.Doc.FileFormat –** verzija protokola oblika datoteke

  - **Data.Doc.Fqdn –** naziv domene servisa OneDrive ili sustava SharePoint Online

  - **Data.Doc.FqdnHash –** jednosmjerno raspršivanje naziva domene koji identificira korisnika

  - **Data.Doc.IdentityTelemetryId –** jednosmjerno raspršivanje korisničkog identiteta kojim se izvršava otvaranje

  - **Data.Doc.IdentityUniqueId –** zastarjelo

  - **Data.Doc.InitializationScenario –** bilježi način otvaranja dokumenta

  - **Data.Doc.IOFlags –** izvješćuje o predmemoriranim zastavicama za postavljanje mogućnosti zahtjeva

  - **Data.Doc.IrmRights –** radnje koje dopuštaju pravila zaštite elektroničkih podataka koja su primijenjena na dokument/korisnika

  - **Data.Doc.IsCloudCollabEnabled –** zastavica koja označava da servis podržava suradnju u oblaku

  - **Data.Doc.IsIncrementalOpen –** zastavica koja označava da je dokument inkrementalno otvoren

  - **Data.Doc.IsOcsSupported –** zastavica koja označava da je dokument podržan u servisu za suradnju

  - **Data.Doc.IsOpeningOfflineCopy –** zastavica koja označava da je otvorena izvanmrežna kopija dokumenta

  - **Data.Doc.IsSyncBacked –** zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

  - **Data.Doc.Location –** označava koji je servis pružio dokument (OneDrive, File Server, SharePoint itd.)

  - **Data.Doc.LocationDetails –** označava koja je poznata mapa pružila lokalno pohranjeni dokument

  - **Data.Doc.NumberCoAuthors –** broj drugih korisnika u sesiji zajedničkog uređivanja

  - **Data.Doc.PasswordFlags –** označava postavljene zastavice za čitanje/pisanje lozinke

  - **Data.Doc.ReadOnlyReasons –** razlozi zbog kojih je dokument otvoren samo za čitanje

  - **Data.Doc.ResourceIdHash –** anonimizirani identifikator dokumenta za dijagnosticiranje problema

  - **Data.Doc.ServerDocId –** nepromjenjivi anonimizirani identifikator dokumenta za dijagnosticiranje problema

  - **Data.Doc.ServerProtocol –** verzija protokola za komuniciranje sa servisom

  - **Data.Doc.ServerType –** vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.)

  - **Data.Doc.ServerVersion –** verzija poslužitelja koji pruža servis

  - **Data.Doc.SessionId –** označava određenu sesiju uređivanja dokumenta u cijeloj sesiji

  - **Data.Doc.SharePointServiceContext –** dijagnostičke informacije iz zahtjeva sustava SharePoint Online

  - **Data.Doc.SizeInBytes –** pokazatelj veličine dokumenta

  - **Data.Doc.SpecialChars –** pokazatelj posebnih znakova u URL-u ili putu dokumenta

  - **Data.Doc.StorageProviderId –** zastarjelo

  - **Data.Doc.StreamAvailability –** pokazatelj je li niz dokumenata dostupan/onemogućen

  - **Data.Doc.SyncBackedType –** pokazatelj vrste dokumenta (lokalni ili na servisu)

  - **Data.Doc.UrlHash –** jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta

  - **Data.Doc.UsedWrsDataOnOpen –** dijagnostički pokazatelj za inkrementalno otvaranje dokumenta

  - **Data.Doc.WopiServiceId –** sadrži jedinstveni identifikator davatelja usluga WOPI

  - **Data.DocumentLoadEndpoint –** zastarjeli/suvišni duplikat (Data.Doc.Location i Data.Doc.IsSyncbacked)

  - **Data.DocumentSizeInBytes –** zastarjelo/suvišno je nadomjestio Data.Doc. SizeInBytes

  - **Data.DocumentSizeOnDisk –** zastarjelo

  - **Data.DoesBaseHaveContentOnOpen –** promjena dijagnostike praćenja kako bismo imali najnoviju verziju zajedničke datoteke

  - **Data.DoesWorkingBranchHaveExcludedDataOnOpen –** promjena dijagnostike praćenja kako bismo imali najnoviju verziju zajedničke datoteke

  - **Data.DownloadFragmentSize –** veličina podataka poslanih u podzahtjevu za dijagnosticiranje problema s mrežom

  - **Data.DsmcStartedTooEarly –** označava pogrešku prilikom pokretanja sesije zajedničkog uređivanja

  - **Data.EditorsCount –** broj drugih suradnika koji uređuju dokument

  - **Data.ExcludedDataThresholdInBytes –** veličina datoteke potrebna za otvaranje putem značajke Asynch

  - **Data.FileIOResult.Code –** predmemorija povratnog koda zadnjeg otvaranja iz sloja protokola

  - **Data.FileIOResult.Success –** predmemorija pokazatelja uspjeha zadnjeg otvaranja iz sloja protokola

  - **Data.FileIOResult.Tag –** predmemorija oznake pogreške zadnjeg otvaranja iz sloja protokola

  - **Data.FileIOResult.Type –** predmemorija vrste pogreške zadnjeg otvaranja iz sloja protokola

  - **Data.FqdnHash –** zastarjelo, zamijenjeno funkcijom Data\_Doc\_FqdnHash

  - **Data.FullIError –** predmemorija svih kodova pogrešaka otvaranja iz sloja protokola

  - **Data.FullyQualifiedDomainName –** zastarjelo, zamijenjeno funkcijom Data\_Doc\_Fqdn

  - **Data.Input.FileOpenState –** stanje koje je zatražila aplikacija (čitanje/čitanje i pisanje itd.)

  - **Data.Input.OpenAsync –** otvaranje značajke Async zatražila je aplikacija

  - **Data.Input.OpenOfflineCopy –** otvaranje iz izvanmrežne kopije zatražila je aplikacija

  - **Data.IOFlags –** zastarjelo

  - **Data.IsBaseBranchEmptyOnOpen –** promjena dijagnostike praćenja kako bismo imali najnoviju verziju zajedničke datoteke

  - **Data.IsCachedHistoricalVersion –** predmemorija sadrži stariju verziju dokumenta

  - **Data.IsDocEnterpriseProtected –** dokument je zaštićen šifriranjem (zaštita elektroničkih dokumenata / EDP)

  - **Data.IsDocInODC –** dokument je prethodno otvoren i već se nalazi u predmemoriji

  - **Data.IsMapUnMapCase –** dio stanja predmemorirane datoteke

  - **Data.IsMapUnMapCase.End –** dio stanja predmemorirane datoteke

  - **Data.IsOfficeHydrationInProgress –** Windows vraća dokument iz izvanmrežne pohrane

  - **Data.isOfficeHydrationRequired –** dokument se trenutno nalazi u izvanmrežnoj pohrani

  - **Data.isOpenFromCollab –** najnovija kopija dokumenta dohvaćena je iz servisa za zajedničku suradnju

  - **Data.isPendingNameExist –** preimenovanje dokumenta je u tijeku

  - **Data.IsStubFile –** dokument još nije spremljen na servis u oblaku

  - **Data.IsSyncBackedStateDifferentThanOnLastOpen –** stanje dokumenta promijenjeno je, a promjene su možda stigle kada dokument nije bio otvoren

  - **Data.isTaskCanceledAfterOpenComplete –** zastarjelo

  - **Data.IsWorkingBranchAvailableOnOpen –** promjena dijagnostike praćenja kako bismo imali najnoviju verziju zajedničke datoteke

  - **Data.LicenseStatus** – status dijagnostike licence za proizvod koji se upotrebljava za potvrdu da su odgovarajuće značajke proizvoda omogućene za korisnikovu vrstu licence 

  - **Data.LicenseType –** označava stanje licence (besplatno/plaćeno/probna verzija itd.)

  - **Data.Location –** označava vrstu/lokaciju medija za pohranu (USB, oblak itd.)

  - **Data.LockRequestDocMode –** označava je li dokument dostupan drugim korisnicima

  - **Data.MyDeferredValue –** zastarjelo

  - **Data.Network.BytesReceived –** zastarjelo

  - **Data.Network.BytesSent –** zastarjelo

  - **Data.Network.ConnectionsCreated –** zastarjelo

  - **Data.Network.ConnectionsEnded –** zastarjelo

  - **Data.OcsDisableReasons –** razlog zbog kojeg za dokument nije dostupan servis za zajedničku suradnju

  - **Data.OcsHostOnOpen –** zastavica koja označava da će se kontrola prebaciti na servis za zajedničku suradnju tijekom otvaranja

  - **Data.OpeningOfflineCopy –** zastavica koja označava da će se otvoriti lokalna kopija dokumenta

  - **Data.Partition –** zastarjelo

  - **Data.RequestTime –** zastarjelo

  - **Data.ResourceIdHash –** zastarjelo

  - **Data.ResumedIncrementalOpen –** zastarjelo

  - **Data.RTCEnabled –** pokrenut je protokol za distribuciju brze promjene

  - **Data.SaveOnOpen –** nespremljene promjene u lokalnom dokumentu spremljene su na servis tijekom otvaranja

  - **Data.ServerProtocol –** zastarjelo, zamijenio protokol Data\_Doc\_ServerProtocol

  - **Data.ServerType –** zastarjelo, zamijenio protokol Data\_Doc\_ServerType

  - **Data.ServerVersione –** zastarjelo, zamijenio protokol Data\_Doc\_ServerVersion

  - **Data.ServiceId –** zastarjelo, zamijenio protokol Data\_Doc\_WopiServiceId

  - **Data.SessionId –** zastarjelo

  - **Data.ShouldSwitchToServerOnly –** lokalna kopija dokumenta ne može se koristiti i mora se koristiti poslužiteljska verzija

  - **Data.SpecialChars –** zastarjelo

  - **Data.StopwatchDuration –** zastarjelo

  - **Data.SyncBackedFileTelemetrySessionId –** zastarjelo

  - **Data.SyncElapsedTime –** zastarjelo

  - **Data.SyncRequestId –** zastarjelo

  - **Data.TestProperty –** zastarjelo

  - **Data.TransitionToHostOnOpen –** zastavica koja označava da će se sesija povezati sa servisom koji hostira dokument

  - **Data.TransitionToHostOnOpenResult –** status prelaska na servis glavnog računala

  - **Data.UseCachedNetworkConnection –** zastavica koja označava je li veza ponovno korištena ili je stvorena nova veza

  - **Data.UseClientIdAsSchemaLockId –** zastavica za kontrolu zaključavanja dokumenata na servisu

  - **Data. VersionType** – ukazuje na vrstu verzije trenutno otvorene operacije.

  - **Data.WopiServiceId –** zastarjelo, zamijenio protokol Data\_Doc\_WopiServiceId

#### <a name="officefileiocsiccachedfilecsisavefilebasic"></a>Office.FileIO.CSI.CCachedFileCsiSaveFileBasic

Omogućuje da utvrdimo je li datoteka uspješno spremljena u FIO sloju. Koristi se za stanje i nadzor značajke.

Prikupljaju se sljedeća polja:

  - **Activity.Group –** oznaka koja omogućuje postavljanje grupiranja događaja nadzora za upravljanje ukupnim uspjehom

  - **Activity.IsHVA –** zastavica koja označava da je događaj ključan za uspjeh korisnika

  - **Data.AsyncOpen –** zastavica koja označava da je dokument otvoren sa sadržajem koji je primljen nakon otvaranja glavnog tijela

  - **Data.BaseDownloadTriggered –** promjena dijagnostike praćenja koja označava da je zatražena osnovna verzija dokumenta

  - **Data.BlockAutoUploadReasons –** kodovi razloga za stanje blokiranog prijenosa (na primjer, isključeno automatsko spremanje, dokument je u prijelazu)

  - **Data.BlockUploadDueToFailedSaveAsOverExisting –** prijenos je blokiran jer ne bi uspio da je ponovljen

  - **Data.CacheFileId –** povezuje se s telemetrijom predmemorije dokumenta sustava Office radi omogućivanja analize utjecaja problema s predmemorijom na korisničko iskustvo

  - **Data.ChartType –** zastarjelo

  - **Data.CoAuthStatus –** izvješćuje status suradnje dokumenta pri spremanju

  - **Data.CoauthUpdatesContext –** izvješćuje kontekst (spajanje/inkrementalno otvaranje)

  - **Data.CountOfMultiRoundTripsDownload –** broj povratnih prijenosa na poslužitelj koji se koristi za otklanjanje poteškoća s performansama i mrežom

  - **Data.CountOfMultiRoundTripsUpload –** broj povratnih prijenosa na poslužitelj koji se koristi za otklanjanje poteškoća s performansama i mrežom
  
  - **Data. CFREnabled** – ukazuje da je za sesiju omogućen CacheFileRuntime.

  - **Data.CFRFailure** – Ukazuje da je CacheFileRuntime naišao na pogrešku.

  - **Data.DialogChoice –** bilježi odabir u dijaloškim okvirima s pogreškom

  - **Data.DialogId –** bilježi DialogId dijaloških okvira s pogreškom prikazanih tijekom spremanja

  - **Data.Dmc.IsOcsSupported –** zastarjelo

  - **Data.Doc.AccessMode –** dokument je samo za čitanje

  - **Data.Doc.AssistedReadingReasons –** postavljeno ako dokument ima aktiviranu zaštitu elektroničkih podataka

  - **Data.Doc.AsyncOpenKind –** označava je li otvorena predmemorirana verzija dokumenta u oblaku i koja je logika za asinkrono osvježavanje korištena.

  - **Data.Doc.ChunkingType –** jedinice koje se koriste za inkrementalno otvaranje dokumenta

  - **Data.Doc.EdpState –** postavka zaštite elektroničkih podataka za dokument

  - **Data.Doc.Ext –** nastavak dokumenta (docx/xlsm/pptx itd.)

  - **Data.Doc.Extension –** zastarjelo

  - **Data.Doc.FileFormat –** verzija protokola oblika datoteke

  - **Data.Doc.Fqdn –** naziv domene servisa OneDrive ili sustava SharePoint Online

  - **Data.Doc.FqdnHash –** jednosmjerno raspršivanje naziva domene koji identificira korisnika

  - **Data.Doc.FqdnHasi –** zastarjelo

  - **Data.Doc.IdentityTelemetryId –** jednosmjerno raspršivanje korisničkog identiteta kojim se izvršava spremanje

  - **Data.Doc.IdentityUniqueId –** zastarjelo

  - **Data.Doc.IKFlags –** zastarjelo

  - **Data.Doc.InitializationScenario –** bilježi način otvaranja dokumenta

  - **Data.Doc.IOFlags –** izvješćuje o predmemoriranim zastavicama za postavljanje mogućnosti zahtjeva

  - **Data.Doc.IrmRights –** radnje koje dopuštaju pravila zaštite elektroničkih podataka koja su primijenjena na dokument/korisnika

  - **Data.Doc.IsCloudCollabEnabled –** zastavica koja označava da aplikacija podržava suradnju u oblaku

  - **Data.Doc.IsIncrementalOpen –** zastavica koja označava da je dokument otvoren inkrementalno

  - **Data.Doc.IsOcsSupported –** zastavica koja označava da dokument podržava suradnju u oblaku

  - **Data.Doc.IsOpeningOfflineCopy –** zastavica koja označava da je otvorena izvanmrežna kopija dokumenta

  - **Data.Doc.IsSyncBacked –** zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

  - **Data.Doc.Location –** označava koji je servis pružio dokument (OneDrive, File Server, SharePoint itd.)

  - **Data.Doc.LocationDetails –** označava koja je poznata mapa pružila lokalno pohranjeni dokument

  - **Data.Doc.NumberCoAuthors –** broj drugih korisnika u sesiji zajedničkog uređivanja

  - **Data.Doc.PasswordFlags –** označava postavljene zastavice za čitanje/pisanje lozinke

  - **Data.Doc.ReadOnlyReasons –** razlozi zbog kojih je dokument otvoren samo za čitanje

  - **Data.Doc.ResourceIdHash –** anonimizirani identifikator dokumenta za dijagnosticiranje problema

  - **Data.Doc.ServerDocId –** nepromjenjivi anonimizirani identifikator dokumenta za dijagnosticiranje problema

  - **Data.Doc.ServerProtocol –** verzija protokola za komuniciranje sa servisom

  - **Data.Doc.ServerType –** vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.)

  - **Data.Doc.ServerVersion –** verzija poslužitelja koji pruža servis

  - **Data.Doc.SessionId –** označava određenu sesiju uređivanja dokumenta u cijeloj sesiji

  - **Data.Doc.SharePointServiceContext –** dijagnostičke informacije iz zahtjeva sustava SharePoint Online

  - **Data.Doc.SizeInBytes –** pokazatelj veličine dokumenta

  - **Data.Doc.SpecialChars –** pokazatelj posebnih znakova u URL-u ili putu dokumenta

  - **Data.Doc.StorageProviderId –** zastarjelo

  - **Data.Doc.StreamAvailability –** pokazatelj je li niz dokumenata dostupan/onemogućen

  - **Data.Doc.SussionId –** zastarjelo

  - **Data.Doc.SyncBackedType –** pokazatelj vrste dokumenta (lokalni ili na servisu)

  - **Data.Doc.UrlHash –** jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta

  - **Data.Doc.UsedWrsDataOnOpen –** dijagnostički pokazatelj za inkrementalno otvaranje dokumenta

  - **Data.Doc.WopiServiceId –** sadrži jedinstveni identifikator davatelja usluga WOPI

  - **Data.DocnReadOnlyReasons –** zastarjelo

  - **Data.DocumentSaveEndpoint –** zastarjelo, zamijenio protokol Data\_Doc\_Location

  - **Data.DocumentSaveType –** vrsta spremanja (Normalno, Stvori, Spremi kao)

  - **Data.DocumentSizeOnDisk –** zastarjelo, zamijenio protokol Data\_Doc\_SizeInBytes

  - **Data.DoesBaseHaveContentOnOpen –** promjena dijagnostike praćenja kako bismo imali najnoviju verziju zajedničke datoteke

  - **Data.DoesWorkingBranchHaveExcludedDataOnOpen –** promjena dijagnostike praćenja kako bismo imali najnoviju verziju zajedničke datoteke

  - **Data.DstDoc.AccessMode –** novi dokument je samo za čitanje/uređivanje

  - **Data.DstDoc.EdpState –** postavka zaštite elektroničkih podataka za novi dokument

  - **Data.DstDoc.Extension –** nastavak novog dokumenta (docx/xlsm/pptx itd.)

  - **Data.DstDoc.FileFormat –** protokol za oblik datoteke novog dokumenta

  - **Data.DstDoc.Fqdn –** naziv domene servisa OneDrive ili sustava SharePoint Online za novi dokument

  - **Data.DstDoc.FqdnHash –** jednosmjerno raspršivanje naziva domene koji identificira korisnika za novi dokument

  - **Data.DstDoc.IdentityUniqueId –** zastarjelo

  - **Data.DstDoc.IOFlags –** predmemorirane zastavice mogućnosti novog dokumenta prilikom otvaranja

  - **Data.DstDoc.IsOpeningOfflineCopy –** zastavica koja označava da je otvorena izvanmrežna kopija novog dokumenta

  - **Data.DstDoc.IsSyncBacked –** zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

  - **Data.DstDoc.Location –** označava koji je servis pružio novi dokument (OneDrive, File Server, SharePoint itd.)

  - **Data.DstDoc.NumberCoAuthors –** broj drugih korisnika u sesiji zajedničkog uređivanja novog dokumenta

  - **Data.DstDoc.ReadOnlyReasons –** razlozi zbog kojih je novi dokument otvoren samo za čitanje

  - **Data.DstDoc.ResourceIdHash –** anonimizirani identifikator dokumenta za dijagnosticiranje problema s novim dokumentom

  - **Data.DstDoc.ServerDocId –** nepromjenjivi anonimizirani identifikator dokumenta za dijagnosticiranje problema s novim dokumentom

  - **Data.DstDoc.ServerProtocol –** verzija protokola za komuniciranje sa servisom prilikom stvaranja novog dokumenta

  - **Data.DstDoc.ServerType –** vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.) za novi dokument

  - **Data.DstDoc.ServerVersion –** verzija poslužitelja koji pruža servis za novi dokument

  - **Data.DstDoc.SessionId –** označava određenu sesiju uređivanja dokumenta u cijeloj sesiji za novi dokument

  - **Data.DstDoc.SharePointServiceContext –** dijagnostičke informacije iz zahtjeva sustava SharePoint Online za novi dokument

  - **Data.DstDoc.SizeInBytes –** pokazatelj veličine dokumenta za novi dokument

  - **Data.DstDoc.UrlHash –** jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta za novi dokument

  - **Data.EditorsCount –** broj drugih suradnika koji uređuju dokument

  - **Data.FullIError –** predmemorija svih kodova pogrešaka iz sloja protokola

  - **Data.HasFilteredCategories –** zastarjelo

  - **Data.HasFilteredCategoryNames –** zastarjelo

  - **Data.HasFilteredSeries –** zastarjelo

  - **Data.HasFilteredSeriesNames –** zastarjelo

  - **Data.HasPendingSaveAs –** označava da je zahtjev Spremi kao/Spremi kopiju u tijeku

  - **Data.Input.FileOpenState –** stanje koje je zatražila aplikacija (čitanje/čitanje i pisanje itd.)

  - **Data.Input.FileSaveState –** stanje koje je zatražila aplikacija (Spremi prilikom otvaranja, Spremi u obliku itd.)

  - **Data.Input.NetworkCost –** označava trošak/vrstu mreže (s ograničenim prometom, s ograničenim prometom s gornjom granicom itd.)

  - **Data.Input.OpenAsync –** zastavica koja označava da je aplikacija zatražila otvaranje značajke async

  - **Data.Input.OpenOfflineCopy –** zastavica koja označava da je aplikacija zatražila izvanmrežno otvaranje

  - **Data.IsCachedHistoricalVersion –** označava da ova predmemorirana datoteka nije najnovija verzija

  - **Data.IsHtml –** označava da je zalijepljen tekst oblika HTML

  - **Data.IsLegacyCode –** označava da je zalijepljen tekst oblika naslijeđenog koda

  - **Data.IsLocalOnlyFile –** označava da je datoteka otvorena samo iz lokalnog prostora za pohranu

  - **Data.IsLocalOrSyncBackedFile –** označava da je datoteka otvorena lokalno i mapirana na servis

  - **Data.IsMapUnMapCase –** dio stanja predmemorirane datoteke

  - **Data.isOpenFromCollab –** označava da je datoteka otvorena na servisu za zajedničku suradnju

  - **Data.IsStubFile –** dokument još nije podijeljen na servis u oblaku

  - **Data.IsSyncBackedFile –** dokument se nalazi u mapi koja se automatski ažurira putem sinkronizacije

  - **Data.IsSyncBackedStateDifferentThanOnLastOpen –** stanje dokumenta promijenjeno je, a promjene su možda stigle kada dokument nije bio otvoren

  - **Data.IsWorkingBranchAvailableOnOpen –** promjena dijagnostike praćenja kako bismo imali najnoviju verziju zajedničke datoteke

  - **Data.Location –** označava vrstu/lokaciju medija za pohranu (USB, oblak itd.)

  - **Data.LockRequestDocMode –** označava je li dokument dostupan drugim korisnicima

  - **Data.MruRequestResult –** zastarjelo

  - **Data.NewDataNotAvailableReason –** zastarjelo

  - **Data.OcsDisableReasons –** ne koristi ga spremanje

  - **Data.OcsHostOnOpen –** ne koristi ga spremanje

  - **Data.Output.FileSaveState –** stanje nakon dovršetka spremanja

  - **Data.PivotChart –** zastarjelo

  - **Data.resolveConflictState –** kodovi razloga za zahtjev za rješavanje sukoba prilikom spajanja

  - **Data.RTCEnabled –** pokrenut je protokol za distribuciju brze promjene

  - **Data.SaveAsToCurrent –** označava da će aktivni dokument prebrisati pohranjenu datoteku

  - **Data.ServiceId –** zastarjelo, zamijenio protokol Data\_Doc\_WopiServiceId

  - **Data.SessionId –** zastarjelo

  - **Data.SizeInBytes –** zastarjelo, zamijenio protokol Data\_Doc\_SizeInBytes

  - **Data.StopwatchDuration –** zastarjelo

  - **Data.SyncBackedFileRequiresOnlineTransition –** zastavica koja označava da je mrežni prijelaz privremeno blokirao radnju spremanja

  - **Data.SyncBackedFileSaveOnOpen –** zastavica koja označava da je za promjene unesene automatskom sinkronizacijom potrebno spremanje nakon otvaranja

  - **Data.TelemetryId –** zastarjelo

  - **Data.TriggerSaveAfterBaseDownload –** promjena dijagnostike praćenja kako bismo imali najnoviju verziju zajedničke datoteke

  - **Data.UploadBlockedDueToCoherencyFailure –** spremanje na servis blokirano je dok korisnik ne riješi sukobljene promjene

  - **Data.UploadBlockedDueToFailedSaveAsOverExisting –** spremanje na servis blokirano je zbog neuspjelog pokušaja prebrisivanja postojeće datoteke

  - **Data.UploadPreemptedForCoherency –** spremanje na servis odbačeno je jer korisnik unosi dodatne promjene

  - **Data.UploadPreemptedForSaveAsOverExistingFailure –** spremanje na servis odbačeno je zbog ranije pogreške SaveAsOverExisting

  - **Data.UploadScheduled –** datoteka je spremna za asinkroni prijenos na servis

  - **Data.UseClientIdAsSchemaLockId –** zastavica za kontrolu zaključavanja dokumenata na servisu

  - **Data.WorkingCopySaved –** promjena dijagnostike praćenja kako bismo imali najnoviju verziju zajedničke datoteke

  - **Data.ZrtSaveAsforSyncBackedBusinessEnabled –** zastavica koja označava da je brzo spremanje omogućeno za SharePoint Online

  - **Data.ZrtSaveAsforSyncBackedConsumerEnabled –** zastavica koja označava da je brzo spremanje omogućeno za OneDrive za privatne korisnike

  - **Data.ZrtSaveAsforSyncBackedCTBusinessEnabled –** zastavica koja označava da je brzo spremanje vrsta sadržaja omogućeno za SharePoint Online

  - **Data.ZrtSaveAsforSyncBackedCTConsumerEnabled –** zastavica koja označava da je brzo spremanje vrsta sadržaja omogućeno za OneDrive za privatne korisnike

  - **Data.ZrtSaveAsforSyncBackedMetaDataBusinessEnabled –** zastavica koja označava da je brzo spremanje metapodataka datoteke omogućeno za SharePoint Online

  - **Data.ZrtSaveAsforSyncBackedMetaDataConsumerEnabled –** zastavica koja označava da je brzo spremanje metapodataka datoteke omogućeno za OneDrive za privatne korisnike

#### <a name="officefindtimeappfailedtostart"></a>Office.FindTime.AppFailedToStart

Prikuplja se ako se aplikacija ne uspijeva pokrenuti zbog neočekivane pogreške prilikom pokretanja. Koristi se za praćenje iznimki i rušenja. Omogućuje nadzor i ispravljanje pogrešaka stanja aplikacije.

Prikupljaju se sljedeća polja:
- **Datum i vrijeme** –vremenska oznaka zapisivanja događaja

- **EventName** –naziv događaja koji se zapisuje

#### <a name="officefirstrunappleactivationresult"></a>Office.FirstRun.Apple.ActivationResult

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za nadziranje stanja tijeka aktivacije naše aplikacije. Prikupljamo podatke kako bismo utvrdili ishod aktiviranja pretplate na Office 365 zajedno s protokom koji se upotrebljava za aktiviranje (iskustvo prvog pokretanja, protok u aplikaciji, kupnja itd.).

Prikupljaju se sljedeća polja:

- **Data_ActivationStatusCollectionTime** – vremenska oznaka

- **Data_ActivationStatusError** – Kôd pogreške pri aktivaciji.

- **Data_ActivationStatusFlowType** – numerička vrijednost koja pokazuje vrstu protoka aktivacije

#### <a name="officefirstrunappleactivationstatus"></a>Office.FirstRun.Apple.ActivationStatus

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se upotrebljava za utvrđivanje rezultata aktiviranja pretplate na Office 365 zajedno s protokom koji se upotrebljava za aktiviranje (FRE, unutar aplikacije, kupnja itd.). Prikupljamo podatke koji sadrže vrstu aktivacije, vrstu protoka (FRE/DocStage /Kupnja) i ID servisa za licenciranje sustava Office.

Prikupljaju se sljedeća polja:

- **Data_ActivationTypeCollectionTime** – vremenska oznaka

- **Data_ActivationTypeFlowType** – numerička vrijednost koja pokazuje vrstu protoka aktivacije

- **Data_ActivationTypeOLSLicense** – identifikator licence

- **Data_ActivationTypeStatus** – kôd statusa aktivacije.

#### <a name="officefirstrunapplefirstruncomplete"></a>Office.FirstRun.Apple.FirstRunComplete

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj nam omogućuje da znamo koristi li korisnik aplikaciju besplatno uz ograničenja, koja je vrsta protoka (FRE/DocStage/Kupnja) i vrsta identiteta (MSP/OrgID). Ovaj događaj koristimo kako bismo saznali je li iskustvo prvog pokretanja (FRE) dovršeno i vrstu identiteta koja se koristi za prijavu (MSA/OrgID).

Prikupljaju se sljedeća polja:

- **Data_FirstRunCompletedCollectionTime** – vremenska oznaka koja bilježi vrijeme dovršetka protoka

- **Data_FirstRunCompletedFlowType** – kôd koji označava vrstu korisničkog protoka koji je dovršen 

- **Data_FirstRunCompletedFreemiumStatus** – kôd koji prikazuje status dovršenosti za protok korisnika besplatne usluge uz ograničenja

- **Data_FirstRunCompletedIdentityType** – vrsta identiteta korisnika koji je dovršio protok

#### <a name="officefirstrunapplefirstrunstart"></a>Office.FirstRun.Apple.FirstRunStart

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj nam omogućuje da znamo je li korisnik ušao u iskustvo prvog pokretanja i vrstu protoka koji se izvodi (FRE/DocStage/Kupnja). Ovaj događaj koristimo kako bismo saznali je li iskustvo prvog pokretanja (FRE) uspješno pokrenuto.

Prikupljaju se sljedeća polja:

- **Data_FirstRunStartedCollectionTime** – vremenska oznaka koja bilježi vrijeme dovršetka protoka

- **Data_FirstRunStartedFlowType** – kôd koji označava vrstu korisničkog protoka koji je dovršen 

#### <a name="officefirstrunapplefirstrunstartedandcompleted"></a>Office.FirstRun.Apple.FirstRunStartedAndCompleted

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj nam omogućuje da znamo koristi li korisnik aplikaciju besplatno uz ograničenja, koja je vrsta protoka (FRE/DocStage/Kupnja) i vrsta identiteta (MSP/OrgID). Ovaj događa koristimo za utvrđivanje stanja i učinkovitosti tijeka iskustva prvog pokretanja (FRE).

Prikupljaju se sljedeća polja:

- **Data_FirstRunCompletedCollectionTime** – vremenska oznaka koja bilježi vrijeme dovršetka protoka

- **Data_FirstRunCompletedFlowType** – kôd koji označava vrstu korisničkog protoka koji je dovršen  

- **Data_FirstRunCompletedFreemiumStatus** – kôd koji prikazuje status dovršenosti za protok korisnika besplatne usluge uz ograničenja

- **Data_FirstRunCompletedIdentityType** – vrsta identiteta korisnika koji je dovršio protok

- **Data_FirstRunStartedCollectionTime** – vremenska oznaka koja bilježi vrijeme pokretanja protoka

- **Data_FirstRunStartedFlowType** – kôd koji označava vrstu korisničkog protoka koji je pokrenut

#### <a name="officefirstrunappleinapppurchaseactivationfail"></a>Office.FirstRun.Apple.InAppPurchaseActivationFail

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za nadziranje stanja tijeka aktivacije naše aplikacije. Prikupljamo podatke kako bismo utvrdili ishod aktivacije kupnje unutar aplikacije zajedno s protokom koji se koristi za aktiviranje (iskustvo prvog pokretanja, protok u aplikaciji, kupnja itd.). 

Prikupljaju se sljedeća polja:

- **Data_ActivationFailCollectionTime** – vremenska oznaka koja registrira vrijeme u kojem se dogodio neuspjeh prilikom aktivacije 

- **Data_ActivationFailFlowType** – kôd koji označava vrstu korisničkog protoka koji se provodio

- **Data_AssoicatedSuccessfullyCollectionTime** – vremenska oznaka koja registrira vrijeme u kojem se dogodio neuspjeh prilikom aktivacije 

- **Data_AssoicatedSuccessfullyFlowType** – kôd koji označava vrstu korisničkog protoka koji se provodio

#### <a name="officefirstrunappleinapppurchaseactivationsuccess"></a>Office.FirstRun.Apple.InAppPurchaseActivationSuccess

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za nadziranje stanja tijeka aktivacije naše aplikacije. Prikupljamo podatke kako bismo utvrdili ishod aktivacije kupnje unutar aplikacije zajedno s protokom koji se koristi za aktiviranje (iskustvo prvog pokretanja, protok u aplikaciji, kupnja itd.). 

Prikupljaju se sljedeća polja:

- **Data_AssoicatedSuccessfullyCollectionTime** – vremenska oznaka koja registrira vrijeme kada je došlo do aktivacije 

- **Data_ActivatedSuccessfullyFlowType** – kôd koji označava vrstu korisničkog protoka koji se provodio

- **Data_AssoicatedSuccessfullyCollectionTime** – vremenska oznaka koja registrira vrijeme u kojem se dogodio neuspjeh prilikom aktivacije 

- **Data_AssoicatedSuccessfullyFlowType** – kôd koji označava vrstu korisničkog protoka koji se provodio

#### <a name="officefirstrunappleinapppurchaseassociationfailed"></a>Office.FirstRun.Apple.InAppPurchaseAssociationFailed

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za nadziranje stanja tijeka aktivacije naše aplikacije. Prikupljamo podatke kako bismo utvrdili ishod aktivacije kupnje unutar aplikacije zajedno s protokom koji se koristi za aktiviranje (iskustvo prvog pokretanja, protok u aplikaciji, kupnja itd.). 

Prikupljaju se sljedeća polja:

- **Data_AssoicatedSuccessfullyCollectionTime** – vremenska oznaka koja registrira vrijeme kada je kupnja naplaćena

- **Data_AppChargedSuccessfullyFlowType** – kôd koji označava vrstu korisničkog protoka koji se provodio

- **Data_AssoicationFailedCollectionTime** – vremenska oznaka koja registrira vrijeme u kojem udruživanje aplikacija nije uspjelo

- **Data_AssoicationFailedFlowType** – kôd koji označava vrstu korisničkog protoka koji se provodio

- **Data_AssoicationFailedResult** – kôd koji označava vrstu opažene pogreške

#### <a name="officefirstrunappleinapppurchaseassociationsuccess"></a>Office.FirstRun.Apple.InAppPurchaseAssociationSuccess

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za nadziranje stanja tijeka aktivacije naše aplikacije. Prikupljamo podatke kako bismo utvrdili ishod aktivacije kupnje unutar aplikacije zajedno s protokom koji se koristi za aktiviranje (iskustvo prvog pokretanja, protok u aplikaciji, kupnja itd.). 

Prikupljaju se sljedeća polja:

- **Data_AssoicatedSuccessfullyCollectionTime** – vremenska oznaka koja registrira vrijeme kada je kupnja naplaćena

- **Data_AppChargedSuccessfullyFlowType** – kôd koji označava vrstu korisničkog protoka koji se provodio

- **Data_AssoicatedSuccessfullyCollectionTime** – vremenska oznaka koja registrira vrijeme u kojem udruživanje aplikacija nije uspjelo

- **Data_AssoicatedSuccessfullyFlowType** – kôd koji označava vrstu korisničkog protoka koji se provodio

#### <a name="officefirstrunappleinapppurchasefailures"></a>Office.FirstRun.Apple.InAppPurchaseFailures

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za nadziranje stanja tijeka aktivacije naše aplikacije. Prikupljamo podatke o ishodu tijeka kupnje unutar aplikacije.

Prikupljaju se sljedeća polja:

- **Data_AppStoreFailureFlowType** – kôd koji označava vrstu korisničkog protoka koji se provodio

- **Data_AppStoreFailureResult** – opažen rezultat neuspjeha

- **Data_CancelRequestFlowType** – kôd koji označava vrstu korisničkog protoka koji se provodio

- **Data_EventId** – kôd koji označava vrstu neuspjeha koji je opažen

#### <a name="officefirstrunappleinapppurchasesattempted"></a>Office.FirstRun.Apple.InAppPurchasesAttempted

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za nadziranje stanja protoka kupnje unutar aplikacije. Prikupljamo podatke za praćenje pokušaja kupnje unutar aplikacije i njihove vrste SKU-a koji se kupuje (mjesečno/godišnje/kućna upotreba/osobno).

Prikupljaju se sljedeća polja:

- **Data_EventId** – kôd koji označava vrstu opaženog rezultata

- **Data_PurchasedClickedOfferType** – vrsta SKU-a koja se pokušala kupiti

- **Data_PurchaseSuccessfulFlowType** – kôd koji označava vrstu korisničkog protoka koji se provodio

#### <a name="officefirstrunappleinapprestoreattempted"></a>Office.FirstRun.Apple.InAppRestoreAttempted

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za nadziranje stanja protoka kupnje unutar aplikacije. Prikupljamo podatke za praćenje pokušaja obnove unutar aplikacije

Prikupljaju se sljedeća polja:

- **Data_EventId** – kôd koji označava vrstu ishoda pokušaja

- **Data_RestoreAttemptFlowType** – kôd koji označava vrstu korisničkog protoka koji se provodio

#### <a name="officefirstrunappleinapprestoreattemptfailed"></a>Office.FirstRun.Apple.InAppRestoreAttemptFailed

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za nadziranje stanja protoka kupnje unutar aplikacije. Prikupljamo podatke za praćenje pokušaja obnove unutar aplikacije i njihove povezane tokove i pogreške.

Prikupljaju se sljedeća polja:

- **Data_RestoreButtonFlowType** – kôd koji označava vrstu korisničkog protoka koji se provodio

- **Data_RestoredFailedPaymentCancelledFlowType** – kôd koji označava vrstu tijeka otkazivanja plaćanja koje je izvršeno

- **Data_RestoredFailedUnKnownFlowType** – je li pokušaj propao zbog provođenja neočekivanog protoka korisnika

- **Data_RestoredFailedUnKnownResult** – je li pokušaj propao iz nepoznatih razloga

#### <a name="officefirstrunapplemacfirstruncompleted"></a>Office.FirstRun.Apple.MacFirstRunCompleted

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj nam daje do znanja da je korisnik prošao kroz iskustvo prvog pokretanja. Ovaj događaj koristimo kako bismo saznali je li iskustvo prvog pokretanja (FRE) uspješno dovršeno.

Prikupljaju se sljedeća polja:

- **Data_FirstRunCollectionTime** – vremenska oznaka koja bilježi vrijeme dovršetka protoka.

#### <a name="officefirstrunapplemacwxpfirstrunstarted"></a>Office.FirstRun.Apple.MacWXPFirstRunStarted

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj nam daje do znanja da je korisnik ušao u iskustvo prvog pokretanja. Ovaj događaj koristimo kako bismo saznali je li iskustvo prvog pokretanja (FRE) uspješno pokrenuto.

Prikupljaju se sljedeća polja:

- **Data_FirstRunPanelName** – naziv ploče na kojoj je započelo iskustvo

#### <a name="officelenslenssdkcloudconnectorlaunch"></a>Office.Lens.LensSdk.CloudConnectorLaunch

Kada korisnik izreže sliku i dodirne „Potvrdi“ na posljednjem izboru slike za korištenje OCR-a, taj će se događaj prikupiti.     
Ovo je zapis korisnika za zahtjev za uslugu, jer na usluzi ne postoji mapiranje posla korisnika od usluge. UserId je potreban da bi ispunio GDPR zahtjeve jer usluga nije izravno izložena korisnicima, već putem klijenata i identificira ukupan broj ljudi koji koriste uslugu, pomažući usluzi da prati količinu korisnika koji koriste proizvod, kao i identificirajući promjene u trendovima, pomoć u traženju i ispravljanju problema u proizvodu.

Prikupljaju se sljedeća polja:

- **CallType** – Niz za identificiranje je li API poziv bio sinkroni ili asinkroni.

- **CloudConnectorRequestId**– niz koji identificira zahtjev za servis koji je stvoren za pretvorbu slika putem servisa. 

- **CloudConnectorTarget** – Niz koji potvrđuje koju će vrstu pretvorbe usluga izvršiti na slikama, poput pretvaranja u PDF, Docx, tekst itd.

- **CustomerId** – niz koji identificira korisnika koji je vlasnik slika koje se obrađuju.

- **CustomerType**-niz koji identificira klijenta kao poduzeće ili pojedinačnog korisnika. Ta razlika utječe na broj slika (kvota) koje klijent može pretvoriti istodobno. 

- **Relid** – niz koji identificira korelacije između Leća i servisa koji se koristi za obradu datoteka.


#### <a name="officelenslenssdkcloudconnectoruploaderror"></a>Office.Lens.LensSdk.CloudConnectorUploadError

U slici u tablicu, kada korisnik dodirne ili Dijeli, Kopiraj ili Otvori, ispravci u tablici koje je napravio korisnik dijele se sa uslugom radi poboljšanja OCR-a. Ovaj se događaj prikuplja na temelju odgovora na pogrešku te usluge i sadrži relevantne identifikatore za rješavanje različitih problema na usluzi. 

Prikupljaju se sljedeća polja:

- **CloudConnectorRequestId** – Identifikator niza za povezivanje zadatka usluge s trenutnim zahtjevom usluge za koji su podijeljeni podaci o poboljšanju.

- **Odnos** – niz koji sadrži identifikator trenutnog zadatka servisa.

- **Razlog** – niz koji sadrži kôd pogreške i opis pogreške.

- **TargetType** – niz koji identificira krajnju točku na servisu.

- **TaskType** – niz koji identificira namjeru poziva usluge.


#### <a name="officelenslenssdkcloudconnectoruploadsuccess"></a>Office.Lens.LensSdk.CloudConnectorUploadSuccess

U slici u tablicu, kada korisnik dodirne ili Dijeli, Kopiraj ili Otvori, ispravci u tablici koje je napravio korisnik dijele se sa uslugom radi poboljšanja OCR-a. Ovaj se događaj prikuplja nakon uspješnog odgovora te usluge i sadrži relevantne identifikatore za rješavanje problema. Također pomaže u analizi upotrebe cjevovoda za poboljšanje usluga.

Prikupljaju se sljedeća polja:

- **CloudConnectorRequestId** – Identifikator niza za povezivanje zadatka usluge s trenutnim zahtjevom usluge za koji su podijeljeni podaci o poboljšanju.

- **Odnos** – niz koji sadrži identifikator trenutnog zadatka servisa.

- **TargetType** – niz koji identificira krajnju točku na servisu.

- **TaskType** – niz koji identificira namjeru poziva usluge.


#### <a name="officelenslenssdkpermission"></a>Office.Lens.LensSdk.Permission

Dopuštenja su osjetljiva značajka, jer bez njih korisnik ne može iskusiti nijednu značajku Objektiva. Dozvole se prate kako bi se razumjele korisničke navike za pružanje / ukidanje dozvola. Kada korisnik stupi u interakciju s bilo kojim dijaloškim okvirom za dozvole u našoj aplikaciji, prikupljamo te događaje. Na temelju korisničkih trendova za prihvaćanje i odbijanje dozvola, identificiramo poboljšanja značajki kako bismo korisnicima pomogli razumjeti zašto su dopuštenja kritična.

Prikupljaju se sljedeća polja:

- **Data_action** – Sadrži vrijednosti kao što su „CameraPermissionAllowed (ili odbijena), StoragePermissionGranted (ili odbijen), što nam omogućuje da shvaćamo je li korisnik prihvatio ili odbio dozvole za pohranu i fotoaparat.

- **Data_Action** – Ovo nam polje pomaže razumjeti koju je vrstu dopuštenja zatražio korisnik, poput Kamere ili pohrane

- **Data_status** – Sadrži vrijednosti kao što su dopuštene, uskraćene i DeniedForever, što nam omogućuje da shvaćamo je li korisnik prihvatio ili odbio dozvole za pohranu i fotoaparat.


#### <a name="officelenslenssdksavemedia"></a>Office.Lens.LensSdk.SaveMedia

Ovaj se događaj poziva kada korisnik klikne na gumb „Gotovo“ i spremi slike na Android i iOS. Pomaže u mjerenju razine korisničkog angažmana kvantificirajući korisnike koji na kraju spremaju slike putem naše aplikacije.

Sljedeća se polja prikupljaju samo za Android:

- **Data_FileSizeAfterCleanUp** – Veličina datoteke nakon što je aplikacija očisti da bi se razumjelo kolika je kompresija postignuta nakon čišćenja.

- **Data_FileSizeAfterSave** – Veličina datoteke nakon što je korisnik spremi kako bi razumjela kolika je kompresija postignuta nakon spremanja.

- **Data_FileSizeBeforeCleanUp** – Veličina datoteke prije nego što je aplikacija očisti kako bi shvatila kolika je veličina snimljene datoteke

- **Data_Filter** – filtar primijenjen na sliku.

- **Data_ImageHeightAfterCleanUp** – Visina slike nakon što ju je aplikacija očistila.

- **Data_ImageWidthAfterCleanUp** – visina slike prije no što ju je očistila aplikacija.

- **Data_ImageWidthAfterCleanUp** – širina slike prije no što ju je očistila aplikacija.

- **Data_ImageWidthAfterCleanUp** – širina slike prije no što ju je očistila aplikacija.

- **Data_MediaId** – identifikator za slike da bi vam se pomoglo pri praćenju uspjeha postupka.

- **Data_ProcessMode** – Način rada korisnika u trenutku spremanja slike od strane korisnika.

- **Data_Source** – određuje odakle je slika, primjerice, snimljena kamerom, uvoz iz galerije itd. 

Sljedeća se polja prikupljaju samo za iOS:

- **Data_Filter** – filtar primijenjen na sliku. 

- **Data_imageDPI** – Smanjenje slike primijenjeno je na sliku spremljene datoteke

- **Data_imageSize** – veličina slike nakon što je korisnik spremio sliku

- **Data_MediaId** – identifikator za slike da bi vam se pomoglo pri praćenju uspjeha postupka.

- **Data_mode** – Način korisnika u trenutku spremanja slike od strane korisnika.

- **Data_sizeinPixel** – veličina slike u obliku piksela

- **Data_Source** – određuje odakle je slika, primjerice, snimljena kamerom, uvoz iz galerije itd. 


#### <a name="officelenslenssdkserviceidmapping"></a>Office.Lens.LensSdk.ServiceIDMapping

Kada se slika uspješno prenese na uslugu, taj se događaj prikuplja. Označava da će usluga sada pokrenuti jedan ili više poslova za obradu slike i sadržavanje relevantnih ID-ova koji pomažu u rješavanju problema. Također pomaže u analizi upotrebe različitih značajki usluge.

Prikupljaju se sljedeća polja:

- **CloudConnectorRequestId**– niz koji identificira zahtjev za servis koji je stvoren za pretvorbu slika putem servisa.

- **I2DserviceProcessID** – niz koji identificira posao usluge koji izvodi određeni podzahtjev 


#### <a name="officeiospaywallpaywallpresented"></a>Office.iOS.Paywall.Paywall.Presented

Ova se telemetrija kritične uporabe prikuplja kada se korisniku prikaže kontrola Paywall-a i upotrebljava se za razumijevanje iskustva kupnje u aplikaciji za korisnika i optimizaciju istog za buduće verzije.

Prikupljaju se sljedeća polja:

- **entryPoint** – niz – gumb/tijek s kojeg je prikazan Paywall. Kao što je „Premium Upgrade Button" ili „First run flow“

- **isFRE** – Booleov – prikazujemo li iskustvo prvog pokretanja ili redovno korisničko sučelje?

#### <a name="officeiospaywallpaywallstats"></a>Office.iOS.Paywall.Paywall.Stats

Ovi metapodaci temeljeni na sesiji prikupljaju se kada se korisniku prikaže korisničko sučelje Paywall, trajanje interakcije i je li kupnja pokušana i uspjela ili nije uspjela.  Podaci se koriste za razumijevanje korištenja i stanja cijelog iskustva plaćanja i otklanjanja pogrešaka, optimizaciju i otklanjanje poteškoća s iskustvom kupnje unutar aplikacije u budućim verzijama.

Prikupljaju se sljedeća polja:

- **entryPoint** – niz – gumb/tijek s kojeg je prikazan Paywall. Kao što je "Premium Upgrade Button" ili „First run flow“

- **isFRE** – Booleov – prikazujemo li iskustvo prvog pokretanja ili redovno korisničko sučelje?

- **stanje** – niz – izlazni status Paywalla. Kao što je „initiated", "paymentDone", "provisionFailed"

- **userDuration** – udvostručeno – trajanje u milisekundama koje je korisnik proveo na Paywall-u

#### <a name="officeiospaywallskuchoosermorebenefitsstats"></a>Office.iOS.Paywall.SKUChooser.MoreBenefits.Stats

Ovaj događaj prikuplja značajke i aplikacije koje korisnik proširuje iz odjeljka „Pogledajte više pogodnostii" i trajanje provedenog vremena.  Podaci se upotrebljavaju za razumijevanje upotrebe značajke „Pogledajte sve pogodnosti" te daljnju optimizaciju iskustva u budućim verzijama.

Prikupljaju se sljedeća polja:

- **appsExpanded** – niz – popis servisa/aplikacija odvojenih zarezom za koje su pogodnosti proširene.

- **productId** – niz – ID proizvoda trgovine App Store za koji korisnik pregledava dodatne ponuđene pogodnosti

- **userDuration** – udvostručeno – trajanje u milisekundama koje je korisnik proveo na Zaslonu s pogodnostima.

#### <a name="officeiospaywallskuchooserstats"></a>Office. iOS. paywall. Skubirač. Stats

Ta se uporaba telemetrije prikuplja da bi vam se prikazao način na koji je korisnik unio birač SKU-a, koliko vremena korisnik provodi na zaslonu birača SKU-a i zašto je izašao iz istog.  Podaci se upotrebljavaju za razumijevanje upotrebe birača SKU-a i optimizaciju iskustva kupnje aplikacija u budućim verzijama.

Prikupljaju se sljedeća polja:

- **entryPoint** – niz – gumb/tijek s kojeg je prikazan Paywall. Kao što je "Premium Upgrade Button" ili „First run flow“

- **exitReason** – niz – razlog izlaza iz birača SKU-a. Kao što je „BuyButton”, „CloseButton

- **isFRE** – Booleov – prikazujemo li iskustvo prvog pokretanja ili redovno korisničko sučelje?

- **userDuration** – udvostručeno – trajanje u milisekundama koje je korisnik proveo na biraču SKU-a


#### <a name="officelivepersonacardconfigurationsetaction"></a>Office.LivePersonaCard.ConfigurationSetAction

Bilježimo kada se korisnik nalazi u aplikaciji koja učitava Osobnu karticu u iščekivanju da korisnik otvori karticu Osobnost za Live.  Podaci se upotrebljavaju da bi se odredile je li kartica ispravno učitana. 

Prikupljaju se sljedeća polja: 

- **Data.accountType** – pripada li korisnik tvrtki ili ustanovi ili je potrošač

- **Data.appContextId** – nasumično generirani identifikacijski broj koji se koristi za identifikaciju različitih računa u istoj aplikaciji

- **Data.AppInfo.Name** – naziv usluge koja se upotrebljava (kartica Profil)

- **Data.AppInfo_Id** – naziv glavne aplikacije

- **Data.AppInfo_Version** – verzija glavne aplikacije

- **Data.cardCorrelationId** – globalno jedinstveni identifikator za karticu osobnosti

- **Data.cardPersonaCorrelationId** – globalno jedinstveni identifikator za određenu osobnost prikazanu na kartici

- **Data.clientCorrelationId** – globalno jedinstveni identifikator za sesiju aplikacije

- **Data.clientType** – vrsta uređaja na kojem je aplikacija pokrenuta

- **Data.contextType** – iz kojeg je konteksta (aplikacije) kartica pokrenuta

- **Data.ecsConfigIds** – identifikatori verzije za značajke omogućene na kartici

- **Data.ecsTagId** – identifikator oznake za značajke

- **Data.eventId** – identifikator naziva događaja, na primjer, „LivePersonaCardRenderedAction”

- **Data.eventpriority** – vrijednost numeriranja za prioritet slanja događaja.

- **Data.feature** – koristi se za grupiranje raznih događaja iste značajke (kartica Profil)

- **Data.flights** – značajke omogućene na kartici

- **Data.fromCache** – jesu li podaci preuzeti iz memorije

- **Data.hasFinePointer** – ima li uređaj mogućnost rada s mišem-pokazivačem

- **Data.hasHoverEvents** – ima li uređaj mogućnost zadržavanja pokazivača miša

- **Data.immersiveProfileCorrelationId** – globalno jedinstven identifikator za sesiju proširenog prikaza profila

- **Data.offlineResolved** – jesu li podaci preuzeti izvan mreže

- **Data.OTelJS.Version** – verzija zapisnika OTel

- **Data.personaCorrelationId** – globalno jedinstven identifikator za jedinstvene osobnosti u sesiji

- **Data.properties** – dodatni metapodaci prikupljeni za svaki događaj na sljedeći način: *[Ovo je polje uklonjeno iz aktualnih međuverzija sustava Office, ali će se možda i dalje prikazivati u starijim međuverzijama.]*

  - **cardCorrelationId** – duplikat za gornji Data.appContextId
  - **cardPersonaCorrelationId** – duplikat za gornji Data.cardCorrelationId
  - **ClientTimeStamp** – vrijeme na aplikaciji prilikom zapisivanja događaja
  - **consumerCorrelationId** – duplikat za gornji Data.clientCorrelationId

  - **externalAppSessionCorrelationId** – globalno jedinstven identifikator za aplikaciju za identifikaciju svih kartica osobnosti otvorenih u istoj podsesiji

- **Data.region** – zemljopisna regija usluge pozadinskog sustava kartice profila s kojom je korisnik povezan

- **Data.tenantAadObjectId** – klijent s kojim je korisnikova pretplata povezana. Omogućuje klasifikaciju problema i utvrđivanje je li problem rasprostranjen ili ograničen na skup korisnika ili određenog klijenta

- **Data.type** – vrsta zapisanog događaja, na primjer, Praćenje, Pogreška, Događaj

- **Data.userAadObjectId** – globalno jedinstveni identifikator korisnika za Microsoftov račun za velike tvrtke (duplikat za Data.UserInfo.Id)

- **Data.UserInfo.Id** – globalno jedinstveni identifikator korisnika za Microsoftov račun za velike tvrtke

- **Data.UserInfo.MsaId** – globalno jedinstveni identifikator korisnika za Microsoftov potrošački račun

- **Data.UserInfo.OMSTenantId** – klijent s kojim je korisnikova pretplata povezana. Omogućuje klasifikaciju problema i utvrđivanje je li problem rasprostranjen ili ograničen na skup korisnika ili određenog klijenta

- **Data.userPuid** – globalno jedinstveni identifikator korisnika za Microsoftov potrošački račun (duplikat za Data.UserInfo.MsaId)

- **Data.version** – verzija usluge (kartica Profil)

- **Data.workloadCulture** – niz kulture u glavnoj aplikaciji

- **DeviceInfo_Id** – globalno jedinstven identifikator uređaja za uređaj

- **DeviceInfo_Make** – marka operacijskog sustava

- **DeviceInfo_Model** – model uređaja

- **DeviceInfo_OsName** – naziv operacijskog sustava uređaja

- **DeviceInfo_OsVersion** – verzija operacijskog sustava

- **DeviceInfo_SDKUid** – jedinstveno označava uređaj iz telemetrijske perspektive SDK-a

#### <a name="officelivepersonacarduseractionsclosedexpandedpersonacard"></a>Office.LivePersonaCard.UserActions.ClosedExpandedPersonaCard

Zapisuje se kada korisnik zatvori proširenu karticu Osobnost. Upotrebljava se za promatranje ključnih anomalija u stopama neuspjeha pri zatvaranju kartice Osobnost za Live.

Prikupljaju se sljedeća polja:

- **AppInfo_Id** – ime glavne aplikacije

- **AppInfo_Version** – verzija glavne aplikacije

- **Data.appContextId** – nasumično generirani identifikacijski broj koji se koristi za identifikaciju različitih računa u istoj aplikaciji

- **Data.AppInfo.Name** – naziv usluge koja se koristi (kartica Profil)

- **Data.cardCorrelationId** – globalno jedinstveni identifikator za karticu osobnosti

- **Data.cardPersonaCorrelationId** – globalno jedinstveni identifikator za određenu osobnost prikazanu na kartici

- **Data.clientCorrelationId** – globalno jedinstveni identifikator za sesiju aplikacije

- **Data.clientType** – vrsta uređaja na kojem je aplikacija pokrenuta, npr. „Outlook_Win32”

- **Data.eventId** – identifikator naziva događaja, na primjer, „LivePersonaCardRenderedAction”

- **Data.exportName** – naziv čitljiv ljudima za događaj radnje korisnika, npr. „ClosedExpandedPersonaCard”

- **Data.exportType** – kategorija događaja za zahtjev izvoza GDPR-a

- **Data.externalAppSessionCorrelationId** – globalno jedinstven identifikator za aplikaciju za identifikaciju svih kartica osobnosti otvorenih u istoj podsesiji

- **Data.feature** – koristi se za grupiranje raznih događaja iste značajke (kartica Profil)

- **Data.immersiveProfileCorrelationId** – globalno jedinstven identifikator za sesiju proširenog prikaza profila

- **Data.OTelJS.Version** – verzija zapisnika OTel

- **Data.personaCorrelationId** – globalno jedinstven identifikator za jedinstvene osobnosti u sesiji

- **Data.properties** – dodatni metapodaci prikupljeni za svaki događaj na sljedeći način: *[Ovo je polje uklonjeno iz aktualnih međuverzija sustava Office, ali će se možda i dalje prikazivati u starijim međuverzijama.]*

   - **cardCorrelationId** – duplikat za gornji Data.appContextId 
   - **cardPersonaCorrelationId** – duplikat za gornji Data.cardCorrelationId
   - **ClientTimeStamp** – vrijeme kada je događaj nastupio u vremenu Unix epohe
   - **consumerCorrelationId** – duplikat za gornji Data.clientCorrelationId 

- **Data.region** – zemljopisna regija usluge pozadinskog sustava kartice profila s kojom je korisnik povezan

- **Data.tenantAadObjectId** – klijent s kojim je korisnikova pretplata povezana. Omogućuje klasifikaciju problema i utvrđivanje je li problem rasprostranjen ili ograničen na skup korisnika ili određenog klijenta

- **Data.type** – vrsta zapisanog događaja, na primjer, Praćenje, Pogreška, Događaj

- **Data.userAadObjectId** – globalno jedinstveni identifikator korisnika za Microsoftov račun za velike tvrtke (duplikat za Data.UserInfo.Id)

- **Data.UserInfo.Id** – globalno jedinstveni identifikator korisnika za Microsoftov račun za velike tvrtke 

- **Data.UserInfo.MsaId** – globalno jedinstveni identifikator korisnika za Microsoftov potrošački račun

- **Data.UserInfo.OMSTenantId** – klijent s kojim je korisnikova pretplata povezana. Omogućuje klasifikaciju problema i utvrđivanje je li problem rasprostranjen ili ograničen na skup korisnika ili određenog klijenta.

- **Data.userPuid** – globalno jedinstveni identifikatora za Microsoftov potrošački račun (duplikat za Data.UserInfo.MsaId)

- **Data.version** – verzija usluge (kartica Profil)

- **DeviceInfo_Id** – globalno jedinstven identifikator za uređaj

- **DeviceInfo_Make** – marka operacijskog sustava

- **DeviceInfo_Model** – model uređaja

- **DeviceInfo.NetworkCost** – označava trošak/vrstu mreže (s ograničenim prometom, s ograničenim prometom s gornjom granicom itd.)

- **DeviceInfo_OsName** – naziv operacijskog sustava uređaja

- **DeviceInfo_OsVersion** – verzija operacijskog sustava

- **PipelineInfo.ClientCountry** – pozivni broj države pošiljatelja na temelju nepročišćene IP adrese klijenta


#### <a name="officelivepersonacarduseractionsclosedpersonacard"></a>Office.LivePersonaCard.UserActions.ClosedPersonaCard

Evidentiramo kada korisnik zatvori karticu Osobnost.  Podaci se koriste da bi se utvrdilo je li kartica ispravno zatvorena. 

Prikupljaju se sljedeća polja: 

- **BatchId** – globalno jedinstveni identifikator ako je kreiran skup zahtjeva

- **Data.appContextId** – nasumično generirani identifikacijski broj koji se koristi za identifikaciju različitih računa u istoj aplikaciji

- **Data.AppInfo.Name** – naziv usluge koja se upotrebljava (kartica Profil)

- **Data.AppInfo_Id** – naziv glavne aplikacije

- **Data.AppInfo_Version** – verzija glavne aplikacije

- **Data.cardCorrelationId** – globalno jedinstveni identifikator za karticu osobnosti

- **Data.cardPersonaCorrelationId** – globalno jedinstveni identifikator za određenu osobnost prikazanu na kartici

- **Data.clientCorrelationId** – globalno jedinstveni identifikator za sesiju aplikacije

- **Data.clientType** – vrsta uređaja na kojem je aplikacija pokrenuta

- **Data.eventId** – identifikator naziva događaja, na primjer, „LivePersonaCardRenderedAction”

- **Data.externalAppSessionCorrelationId** – globalno jedinstven identifikator za aplikaciju za identifikaciju svih kartica osobnosti otvorenih u istoj podsesiji.

- **Data.feature** – koristi se za grupiranje raznih događaja iste značajke (kartica Profil)

- **Data.immersiveProfileCorrelationId** – globalno jedinstven identifikator za sesiju proširenog prikaza profila

- **Data.OTelJS.Version** – verzija zapisnika OTel

- **Data.personaCorrelationId** – globalno jedinstven identifikator za jedinstvene osobnosti u sesiji

- **Data.properties** – dodatni metapodaci prikupljeni za svaki događaj na sljedeći način: *[Ovo je polje uklonjeno iz aktualnih međuverzija sustava Office, ali će se možda i dalje prikazivati u starijim međuverzijama.]*

  - **ClientTimeStamp** – vrijeme na aplikaciji tijekom zapisivanja događaja
  - **cardCorrelationId** – duplikat za gornji Data.appContextId
  - **cardPersonaCorrelationId** – duplikat za gornji Data.cardCorrelationId
  - **consumerCorrelationId** – duplikat za gornji Data.clientCorrelationId

- **Data.region** – zemljopisna regija usluge pozadinskog sustava kartice profila s kojom je korisnik povezan

- **Data.tenantAadObjectId** – klijent s kojim je korisnikova pretplata povezana. Omogućuje klasifikaciju problema i utvrđivanje je li problem rasprostranjen ili ograničen na skup korisnika ili određenog klijenta

- **Data.type** – vrsta zapisanog događaja, na primjer, Praćenje, Pogreška, Događaj

- **Data.userAadObjectId** – globalno jedinstveni identifikator korisnika za Microsoftov račun za velike tvrtke (duplikat za Data.UserInfo.Id)

- **Data.UserInfo.Id** – globalno jedinstveni identifikator korisnika za Microsoftov račun za velike tvrtke

- **Data.UserInfo.MsaId** – globalno jedinstveni identifikator korisnika za Microsoftov potrošački račun

- **Data.UserInfo.OMSTenantId** – klijent s kojim je korisnikova pretplata povezana. Omogućuje klasifikaciju problema i utvrđivanje je li problem rasprostranjen ili ograničen na skup korisnika ili određenog klijenta

- **Data.userPuid** – globalno jedinstveni identifikatora za Microsoftov potrošački račun (duplikat za Data.UserInfo.MsaId)

- **Data.version** – verzija usluge (kartica Profil)

- **Data_hostAppRing** – implementacijski prsten kartice Osobnost

- **Event_ReceivedTime** – vrijeme tijekom kojeg je događaj bio prijavljen u uslugu

#### <a name="officelivepersonacarduseractionsopenedexpandedpersonacard"></a>Office.LivePersonaCard.UserActions.OpenedExpandedPersonaCard

Zapisuje se kada korisnik otvori proširenu karticu Osobnost. Koristi se za promatranje ključnih anomalija u stopama neuspjeha pri pokretanju kartice Osobnost za Live.

Prikupljaju se sljedeća polja:

- **AppInfo_Id** – ime glavne aplikacije

- **AppInfo_Version** – verzija glavne aplikacije

- **Data.appContextId** – nasumično generirani identifikacijski broj koji se koristi za identifikaciju različitih računa u istoj aplikaciji

- **Data.AppInfo.Name** – naziv usluge koja se koristi (kartica Profil)

- **Data.cardCorrelationId** – globalno jedinstveni identifikator za karticu osobnosti

- **Data.cardPersonaCorrelationId** – globalno jedinstveni identifikator za određenu osobnost prikazanu na kartici

- **Data.clientCorrelationId** – globalno jedinstveni identifikator za sesiju aplikacije

- **Data.clientScenario** – za identifikaciju značajke u aplikaciji putem koje je otvorena kartica osobnosti

- **Data.clientType** – vrsta uređaja na kojem je aplikacija pokrenuta

- **Data.eventId** – identifikator naziva događaja, na primjer, „LivePersonaCardRenderedAction”

- **Data.externalAppSessionCorrelationId** – globalno jedinstven identifikator za aplikaciju za identifikaciju svih kartica osobnosti otvorenih u istoj podsesiji.

- **Data.exportName** – naziv čitljiv ljudima za događaj radnje korisnika, npr. „OpenedPersonaCard”

- **Data.exportType** – kategorija događaja za zahtjev izvoza GDPR-a

- **Data.feature** – koristi se za grupiranje raznih događaja iste značajke (kartica Profil)

- **Data.hasPersonaInsightRing** – uvidi iz sustava Office ili servisa LinkedIn mogu biti dostupni korisniku

- **Data.hostAppRing** – krug kojim je aplikacija bila distribuirana

- **Data.immersiveProfileCorrelationId** – globalno jedinstven identifikator za sesiju proširenog prikaza profila

- **Data.OTelJS.Version** – verzija zapisnika OTel

- **Data.personaCorrelationId** – globalno jedinstven identifikator za jedinstvene osobnosti u sesiji

- **Data.properties** – dodatni metapodaci prikupljeni za svaki događaj na sljedeći način: *[Ovo je polje uklonjeno iz aktualnih međuverzija sustava Office, ali će se možda i dalje prikazivati u starijim međuverzijama.]*

  - **cardCorrelationId** – duplikat za gornji Data.appContextId 
  - **cardPersonaCorrelationId** – duplikat za gornji Data.cardCorrelationId
  - **consumerCorrelationId** – duplikat za gornji Data.clientCorrelationId 

- **Data.region** – zemljopisna regija usluge pozadinskog sustava kartice profila s kojom je korisnik povezan

- **Data.section** – aktivni odjeljak proširene kartice

- **Data.tenantAadObjectId** – klijent s kojim je korisnikova pretplata povezana. Omogućuje klasifikaciju problema i utvrđivanje je li problem rasprostranjen ili ograničen na skup korisnika ili određenog klijenta

- **Data.type** – vrsta zapisanog događaja, na primjer, Praćenje, Pogreška, Događaj

- **Data.userAadObjectId** – globalno jedinstveni identifikator korisnika za Microsoftov račun za velike tvrtke (duplikat za Data.UserInfo.Id)

- **Data.UserInfo.Id** – globalno jedinstveni identifikator korisnika za Microsoftov račun za velike tvrtke 

- **Data.UserInfo.MsaId** – globalno jedinstveni identifikator korisnika za Microsoftov potrošački račun

- **Data.UserInfo.OMSTenantId** – klijent s kojim je korisnikova pretplata povezana. Omogućuje klasifikaciju problema i utvrđivanje je li problem rasprostranjen ili ograničen na skup korisnika ili određenog klijenta

- **Data.userPuid** – globalno jedinstveni identifikatora za Microsoftov potrošački račun (duplikat za Data.UserInfo.MsaId)

- **Data.version** – verzija usluge (kartica Profil)

- **DeviceInfo_Id** – globalno jedinstven identifikator za uređaj

- **DeviceInfo_Make** – marka operacijskog sustava

- **DeviceInfo_Model** – model uređaja

- **DeviceInfo_OsName** – naziv operacijskog sustava uređaja

- **DeviceInfo_OsVersion** – verzija operacijskog sustava

- **DeviceInfo_SDKUid** – jedinstveno označava uređaj iz telemetrijske perspektive SDK-a

- **NetworkCost** – označava trošak/vrstu mreže (s ograničenim prometom, s ograničenim prometom s gornjom granicom itd.)

- **NetworkCountry** – pozivni broj države pošiljatelja na temelju nepročišćene IP adrese klijenta


#### <a name="officelivepersonacarduseractionsopenedpersonacard"></a>Office.LivePersonaCard.UserActions.OpenedPersonaCard

Zapisuje se kada korisnik otvori karticu Osobnost. Koristi se za promatranje ključnih anomalija u stopama neuspjeha pri pokretanju kartice Osobnost za Live.

Prikupljaju se sljedeća polja:

- **Data.appContextId** – nasumično generirani identifikacijski broj koji se koristi za identifikaciju različitih računa u istoj aplikaciji

- **Data.AppInfo.Name** – naziv usluge koja se koristi (kartica Profil)

- **bandwidthEstimateMbps** – procjena efektivne propusnosti u Mbps

- **Data.cardCorrelationId** – globalno jedinstveni identifikator za karticu osobnosti

- **Data.cardPersonaCorrelationId** – globalno jedinstveni identifikator za određenu osobnost prikazanu na kartici

- **Data.clientCorrelationId** – globalno jedinstveni identifikator za sesiju aplikacije

- **Data.clientType** – vrsta uređaja na kojem je aplikacija pokrenuta.

- **Data.eventId** – identifikator naziva događaja, na primjer, „LivePersonaCardRenderedAction”

- **Data.exportName** – naziv čitljiv ljudima za događaj radnje korisnika, npr. „OpenedPersonaCard”

- **Data.exportType** – kategorija događaja za zahtjev izvoza GDPR-a

- **Data.externalAppSessionCorrelationId** – globalno jedinstven identifikator za aplikaciju za identifikaciju svih kartica osobnosti otvorenih u istoj podsesiji

- **Data.feature** – koristi se za grupiranje raznih događaja iste značajke (kartica Profil)

- **Data.hasPersonaInsightRing** – uvidi iz sustava Office ili servisa LinkedIn mogu biti dostupni korisniku

- **Data.hostAppRing** – krug kojim je aplikacija bila distribuirana

- **Data.immersiveProfileCorrelationId** – globalno jedinstven identifikator za sesiju proširenog prikaza profila

- **Data.OTelJS.Version** – verzija zapisnika OTel

- **Data.personaCorrelationId** – globalno jedinstven identifikator za jedinstvene osobnosti u sesiji

- **Data.properties** – dodatni metapodaci prikupljeni za svaki događaj kako slijedi. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

    - **cardCorrelationId** – duplikat za gornji Data.appContextId 
    - **cardPersonaCorrelationId** – duplikat za gornji Data.cardCorrelationId
    - **consumerCorrelationId** – duplikat za gornji Data.clientCorrelationId 
    - **networkEffectiveType** – učinkovita vrsta mrežne veze, na primjer „slow-2g Online” za prepoznavanje je li korisnik povezan s internetom u vrijeme prikazivanja kartice osobnosti
    - **networkType** – vrsta mrežne povezivosti uređaja koji se koristi
    - **roundTripEstimateMs** – procijenjeni učinkoviti povratni put trenutačne veze u milisekundama

- **Data.region** – zemljopisna regija usluge pozadinskog sustava kartice profila s kojom je korisnik povezan

- **Data.tenantAadObjectId** – klijent s kojim je korisnikova pretplata povezana. Omogućuje klasifikaciju problema i utvrđivanje je li problem rasprostranjen ili ograničen na skup korisnika ili određenog klijenta

- **Data.type** – vrsta zapisanog događaja, na primjer, Praćenje, Pogreška, Događaj

- **Data.userAadObjectId** – globalno jedinstveni identifikator korisnika za Microsoftov račun za velike tvrtke (duplikat za Data.UserInfo.Id)

- **Data.UserInfo.Id** – globalno jedinstveni identifikator korisnika za Microsoftov račun za velike tvrtke 

- **Data.UserInfo.MsaId** – globalno jedinstveni identifikator korisnika za Microsoftov potrošački račun

- **Data.UserInfo.OMSTenantId** – klijent s kojim je korisnikova pretplata povezana. Omogućuje klasifikaciju problema i utvrđivanje je li problem rasprostranjen ili ograničen na skup korisnika ili određenog klijenta

- **Data.userPuid** – globalno jedinstveni identifikatora za Microsoftov potrošački račun (duplikat za Data.UserInfo.MsaId)

- **Data.version** – verzija usluge (kartica Profil)

- **Data.viewType** – definira vrstu prikazane kartice Profil

- **Data.wasOpenedAsCompactCard** – koristi se za prepoznavanje je li kartica prvo bila otvorena kao kompaktan prikaz

- **NetworkCost** – označava trošak/vrstu mreže (s ograničenim prometom, s ograničenim prometom s gornjom granicom itd.)

- **NetworkCountry** – pozivni broj države pošiljatelja na temelju nepročišćene IP adrese klijenta.

#### <a name="officemanageabilityclient-fetchpolicyprechecks"></a>Office.Manageability.Client Fetch.PolicyPreChecks

Ključna telemetrija za uspjeh praćenja\\pogreške provjere dohvaćanja pravilnika u oblaku. ExitReason sadrži na mapiranje identifikatora na zahtjev prethodne provjere koja nije uspjela.

Prikupljaju se sljedeća polja:

  - **Data.ExitReason** – vrijednost identifikatora koja navodi razlog Izlaza, ako prethodna provjera ne uspije

  - **Data.Log** –prilagođena poruka zapisnika koja označava uspješnost ili neuspješnost prethodne provjere

#### <a name="officemanageabilityclientfetchandapplypolicy"></a>Office.Manageability.Client.Fetch.AndApplyPolicy

Ključna telemetrija za uspjeh praćenja\\pogreške pokretanja dohvaćanja pravilnika u oblaku iz aplikacije. Razlog izlaza sadrži mapu identifikatora za razlog pogreške.

Prikupljaju se sljedeća polja:

  - **Data.ExitReason** – vrijednost identifikatora koja navodi razlog Izlaza, ako prethodna provjera ne uspije

  - **Data.Log** –prilagođena poruka zapisnika koja označava uspješnost ili neuspješnost prethodne provjere

#### <a name="officeofficemobilepdfviewerpdffileopenmeasurements"></a>Office.OfficeMobile.PdfViewer.PdfFileOpenMeasurements

Taj se događaj prikuplja za aplikaciju Office za iOS, a bilježi kada dolazi do operacije otvaranja datoteke. Prikupljamo te podatke da bi se osigurala dobra izvedba za sva otvaranja datoteka u aplikaciji. 

Prikupljaju se sljedeća polja:

- **Data_Doc_ActivationFQDN** – naziv domene aplikacije Davatelj usluge za scenarij aktivacije datoteke (bilježe se samo informacije o prvim stranama)

- **Data_Doc_CreateTelemetryReason** – telemetrijski razlog stvaranja PDF-a. (Na primjer: stvaranje iz skena, upotreba radnje „slika u PDF”, upotreba radnje „dokument u PDF” itd.)

- **Data_Doc_DownloadDurationms** – vrijeme za preuzimanje PDF datoteke u oblaku.

- **Data_Doc_DownloadEndTime** – vremenska oznaka za kraj preuzimanja datoteke u oblaku.

- **Data_Doc_DownloadStartTime** – vremenska oznaka za početak preuzimanja datoteke u oblaku.

- **Data_Doc_FileOpSessionID** – jedinstveni ID za sesiju dokumenta.

- **Data_Doc_Location** – mjesto na kojem se nalazi datoteka (lokalno, ODSP, iCloud, datotečna aplikacija drugih proizvođača, wopi

- **Data_Doc_OpenCompletionTime** – vremenska oznaka za kraj otvorene operacije PDF datoteke.

- **Data_Doc_OpenDurationms** – vrijeme za otvaranje PDF datoteke u milisekundama.

- **Data_Doc_OpenStartTime** – vremenska oznaka za početak otvorene operacije PDF datoteke.

- **Data_Doc_TelemetryReason** – telemetrijski razlog za otvoren događaj (na primjer: otvaranje iz MRU-a ili pregledavanje, aktivacija datoteka, aktivacija protokola itd.).

- **Doc_RenderDurationms** – vrijeme za renderiranje PDF datoteke


#### <a name="officeofficemobilepdfviewerpdffileoperations-on-android"></a>Office.OfficeMobile.PdfViewer.PdfFileOperations (on Android)

Događaj se prikuplja za aplikaciju Office za sustav Android. On se bilježi kada se provede operacija otvaranja, zatvaranja ili spremanja datoteke .pdf i upotrebljava se za razumijevanje i određivanje prioriteta korisničkog iskustva na temelju podataka o radu datoteke .pdf. Događaj nam omogućuje da osiguramo da operacije otvaranja, zatvaranja i spremanja datoteke .pdf funkcioniraju na očekivani način te da poboljšamo učinkovitost operacija datoteke .pdf.

Prikupljaju se sljedeća polja:

- **Data_Doc_FileOpSessionID** – jedinstveni ID za sesiju dokumenta

- **Data_ErrorCode** – pogreška u slučaju neuspjelih otvaranja datoteka / neuspjelih preuzimanja / otkazanih preuzimanja

- **Data_ErrorMessage** – odgovarajući kôd na poruku o pogrešci

- **Data_FailureReason** – u slučaju neuspjelog otvaranja, ovi identifikatori definiraju razlog neuspjeha.

- **Data_FileGUID** – globalni identifikator za datoteku koja se nasumično generira

- **Data_FileLocation** – lokacija na kojoj se datoteka nalazi, npr.: Lokalno, ODSP, iCloud itd.

- **Data_FileOpenEntryPoint** – ulazno mjesto za otvaranje datoteke

- **Data_FileSize** – veličina datoteke na kojoj se operacija provodi

- **Data_NetworkRequestErrorResponse** – odgovor pogreške mreže koji odgovara kôdu pogreške.

- **Data_NetworkRequestStage** – faza pogreške u slučaju preuzimanja PDF datoteke iz oblaka.

- **Data_OpenMode** – u kojem se načinu rada PDF otvorio, npr.: 0: način rada Prikaz, 2: način rada Potpis

- **Data_PageCount** – broj stranica u PDF datoteci.

- **Data_PasswordProtected** – oznaka koja označava je li datoteka zaštićena lozinkom ili nije.

- **Data_ProviderApp** – aplikacija pružatelja usluga koji trenutno pruža usluge u slučaju isključive aktivacije datoteke 

- **Data_ReadOnly** – oznaka koja označava je li datoteka samo za čitanje ili nije.

- **Data_Result** – status operacije koja se izvršava, npr.: istinito:uspjeh, neistinito:neuspjeh

- **Data_Type** – vrsta operacije datoteke (otvaranje, zatvaranje ili spremanje) 

#### <a name="officeofficemobilepdfviewerpdffileoperations-on-ios"></a>Office.OfficeMobile.PdfViewer.PdfFileOperations (on iOS)

Događaj se prikuplja za aplikaciju Office za sustav iOS. On se bilježi kada se provede operacija otvaranja, zatvaranja ili spremanja datoteke .pdf i upotrebljava se za razumijevanje i određivanje prioriteta korisničkog iskustva na temelju podataka o radu datoteke .pdf. Događaj nam omogućuje da osiguramo da operacije otvaranja, zatvaranja i spremanja datoteke .pdf funkcioniraju na očekivani način te da poboljšamo učinkovitost operacija datoteke .pdf. 

- **Data_Doc_FileOpSessionID** – jedinstveni ID za sesiju dokumenta 

- **Data_ErrorCode** – pogreška u slučaju neuspjelih otvaranja datoteka / neuspjelih preuzimanja / otkazanih preuzimanja 

- **Data_ErrorMessage** – odgovarajući kôd na poruku o pogrešci 

- **Data_FailureReason** – u slučaju neuspjelog otvaranja, ovi identifikatori definiraju razlog neuspjeha. 

- **Data_FileGUID** – globalni identifikator za datoteku koja se nasumično generira

- **Data_FileLocation** – lokacija na kojoj se datoteka nalazi (Lokalno, ODSP, iCloud itd.) 

- **Data_FileOpenEntryPoint** – ulazno mjesto za otvaranje datoteke 

- **Data_FileSize** – veličina datoteke na kojoj se operacija provodi 

- **Data_OpenMode** – U kojem je načinu PDF otvoren (0: način prikaza 2: način potpisivanja) 

- **Data_PageCount** – broj stranica u PDF datoteci.

- **Data_PasswordProtected** – oznaka koja označava je li datoteka zaštićena lozinkom ili nije. 

- **Data_ProviderApp** – aplikacija pružatelja usluga koji trenutno pruža usluge u slučaju isključive aktivacije datoteke 

- **Data_ReadOnly** – oznaka koja označava je li datoteka samo za čitanje ili nije.

- **Data_Result** – status operacije koja se izvršava (istinito:uspjeh, neistinito:neuspjeh) 

- **Data_Type** – vrsta operacije datoteke (otvaranje, zatvaranje ili spremanje)


#### <a name="officeonenoteandroidappnavigationnavigationuistatechanged"></a>Office.OneNote.Android.App.Navigation.NavigationUIStateChanged

*[Ovaj je događaj prethodno imenovan OneNote.App.Navigation.NavigationUIStateChanged.]*

Ovaj događaj prikuplja ključni signal koji se koristi za osiguravanje da se korisnici aplikacije OneNote mogu uspješno kretati aplikacijom.  Telemetrija se koristi za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. 

Prikupljaju se sljedeća polja: 

- **IS_SPANNED** – označava je li aplikacija u rastegnutom načinu rada. To se posebno bilježi za sklopive uređaje.

- **NEW_STATE** – označava stanje aplikacije neposredno nakon navigacije

- **OLD_STATE** – označava stanje aplikacije neposredno prije navigacije

#### <a name="officeonenoteandroidcanvaspageopened"></a>Office.OneNote.Android.Canvas.PageOpened

*[Ovaj je događaj prethodno imenovan OneNote.Canvas.PageOpened.]*

Signal koji se koristi za snimanje prilikom otvaranja stranice.  Telemetrija se koristi za nadziranje, otkrivanje i ispravljanje problema tijekom otvaranja stranice u programu OneNote

Prikupljaju se sljedeća polja: 

- **JOT_ID** – objekt otvorene stranice

- **TIME_TAKEN_IN_MS** – vrijeme potrebno za otvaranje stranice

#### <a name="officeonenoteandroidcapturenewnotenewnotetaken"></a>Office.OneNote.Android.Capture.NewNote.NewNoteTaken

*[Ovaj je događaj prethodno imenovan OneNote.Capture.NewNote.NewNoteTaken.]*

Ovaj se signal koristi za osiguravanje da se, nakon što se korisnik prijavi u aplikaciju OneNote na platformi Android, bilježnice pravilno dodijele te da je korisnik uspješno kreirao novu bilješku.  To se upotrebljava za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge.

Prikupljaju se sljedeća polja:

- Nijedno

#### <a name="officeonenoteandroidlenssdkofficelenslaunched"></a>Office.OneNote.Android.LensSDK.OfficeLensLaunched

*[Ovaj je događaj prethodno imenovan OneNote.LensSDK.OfficeLensLaunched.]*

Ovaj događaj prikuplja ključne signale koji se koriste za osiguravanje pravilnog pokretanja aplikacije OfficeLens.  Telemetrija se koristi za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. 

Prikupljaju se sljedeća polja: 

- **CAPTURE_MODE** – označava način rada u kojem je aplikacija OfficeLens pokrenuta.  To može biti zadani način, način za uređivanje, brzo umetanje ili uvoz videozapisa.

- **ERROR_CODE** – kôd pogreške pri pokretanju u slučaju da je došlo do pogreške tijekom pokretanja.

- **IMAGE_COUNT** – označava broj snimljenih slika

- **LAUNCH_REASON** – označava protok pod kojim je aplikacija OfficeLens bila pokrenuta. To može biti putem zaključanog zaslona ili mogućnosti Kamera ili Galerija u aplikaciji StickyNotes ili putem aplikacije OneNote Canvas itd.

#### <a name="officeonenoteandroidmessagebarmessagebarclicked"></a>Office.OneNote.Android.MessageBar.MessageBarClicked

*[Ovaj je događaj prethodno imenovan OneNote.MessageBar.MessageBarClicked.]*

Signal koji se koristi za označavanje bilo kakvih problema tijekom korištenja trake s porukama.  Telemetrija se koristi za nadgledanje, otkrivanje i ispravljanje problema nastalih tijekom interakcije s trakom s porukama

Prikupljaju se sljedeća polja: 

- **Message_Bar_Type** – vraća ako korisnik koristi staru ili novu traku s porukama

- **Message_Type** – vraća ID poruke o pogrešci

#### <a name="officeonenoteandroidstickynotesnotecreated"></a>Office.OneNote.Android.StickyNotes.NoteCreated
 
Ključan signal koji se koristi za nadzor mogućnosti da korisnici aplikacije Ljepljive bilješke mogu stvarati bilješke u aplikaciji.   Telemetrija se koristi za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. Ako korisnici ne mogu stvoriti bilješku, time bi se izazvao incident visoke ozbiljnosti.

Prikupljaju se sljedeća polja:

- **IsExportable** – zastavica koja označava je li ovaj događaj bio rezultat radnje korisnika ili ne. Treba se postaviti na Istinito jer je NoteCreated radnja koju aktivira korisnik.

- **NoteLocalId** – prepoznatljiv jedinstveni identifikator dodijeljen bilješci u vrijeme kada korisnik stvori bilješku unutar aplikacije.

- **StickyNotes-SDKVersion** – broj verzije koji označava verziju aplikacije Sticky Notes koju korisnik koristi. Omogućuje prepoznavanje verzija proizvoda s kojima se pojavljuje problem kako bismo mogli ispravno odrediti njegov prioritet.


#### <a name="officeonenoteandroidstickynotesnoteviewed"></a>Office.OneNote.Android.StickyNotes.NoteViewed

Ključan signal koji se koristi za nadzor mogućnosti da korisnici aplikacije Ljepljive bilješke mogu prikazivati bilješke u aplikaciji.  Telemetrija se koristi za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. Ako korisnici ne mogu vidjeti svoje bilješke, time bi se izazvao incident visoke ozbiljnosti.

Prikupljaju se sljedeća polja:

- **HasImages** – zastavica koja označava jesu li u prikazanoj bilješci pohranjene slike.

- **IsExportable** – zastavica koja označava je li ovaj događaj bio rezultat radnje korisnika ili ne. Treba se postaviti na Istinito jer je NoteViewed radnja koju aktivira korisnik.

- **NoteLocalId** – prepoznatljiv jedinstveni identifikator dodijeljen bilješci u vrijeme kada korisnik stvori bilješku unutar aplikacije.

- **StickyNotes-SDKVersion** – broj verzije koji označava verziju aplikacije Sticky Notes koju korisnik koristi. Omogućuje prepoznavanje verzija proizvoda s kojima se pojavljuje problem kako bismo mogli ispravno odrediti njegov prioritet.


#### <a name="officeonenotecanvasinkinkstrokelogger"></a>Office.OneNote.Canvas.Ink.InkStrokeLogger 

Ovaj se događaj koristi za otkrivanje i dijagnosticiranje pogreške visoke frekvencije s kojom se korisnik susreće dok koristi značajku Rukopis.  To će se koristiti za određivanje najprikladnijeg načina otklanjanja ovog problema. 

Prikupljaju se sljedeća polja:

- **CurrentCanvasZoomFactor** – trenutni faktor zumiranja područja crtanja.

- **CurrentNotebook** – identifikator trenutne aktivne bilježnice.

- **CurrentPage** – identifikator trenutne aktivne stranice

- **CurrentSection** – identifikator trenutno aktivnog odjeljka.

- **DefaultCanvasZoomFactor** – zadani faktor zumiranja područja crtanja.

- **InkStrokeCount** – ukupan broj rukopisnih poteza od posljednje evidencije.

- **InkStrokeWithLayerInkEffect** – broj rukopisnih poteza s efektom sloja rukopisa od posljednje evidencije.

- **InkStrokeWithoutPressureCount** – broj rukopisnih poteza bez pritiska od posljednje evidencije.

- **InkStrokeWithPencilInkEffect** – broj rukopisnih poteza s efektom rukopisa olovkom od posljednje evidencije.

- **InkStrokeWithTilt** – broj rukopisnih poteza s naginjanjem od posljednje evidencije.

#### <a name="officeonenotenavigationcreatepage"></a>Office.OneNote.Navigation.CreatePage

Ključni signal korišten za nadzor mogućnosti korisnika OneNote za stvaranje stranica u aplikaciji OneNote.  Telemetrija korištena za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. Ako korisnici ne mogu stvoriti stranicu, time bi se izazvao incident visoke ozbiljnosti.

Prikupljaju se sljedeća polja:

- **IsAtSectionEnd** – označava je li nova stranica stvorena na kraju odjeljka ili nije.

- **IsBlank** – označava je li nova stranica prazna stranica ili je stvorena s predloškom.

- **IsRecentsView** – označava je li stranica stvorena iz nedavnih stavki ili nije.

- **NavView** – označava je li stranica stvorena iz navigacijskog prikaza ili nije.

- **NoteType** – označava vrstu (brza bilješka, popis ili fotografija) stranice.

- **QuickNoteType** – označava vrstu (brza bilješka, popis ili fotografija) stranice.

- **RailState** – označava stanje navigacijske trake aplikacije OneNote tijekom stvaranja stranice.

- **Trigger** – označava ulaznu točku na kojoj je radnja stvaranja stranice započeta.

- **TriggerInfo** – označava dodatne informacije povezane s okidačem.


#### <a name="officeonenotenavigationcreatesection"></a>Office.OneNote.Navigation.CreateSection

Ključni signal korišten za nadzor mogućnosti korisnika OneNote za stvaranje odjeljaka u aplikaciji OneNote.  Telemetrija korištena za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. Ako korisnici ne mogu stvoriti stranicu, time bi se izazvao incident visoke ozbiljnosti.

Prikupljaju se sljedeća polja

- **NotebookID** – jedinstveni identifikator bilježnice.

- **SectionID** – jedinstveni identifikator stvorenog odjeljka.

- **Trigger** – označava ulaznu točku na kojoj je radnja stvaranja odjeljka započeta.

- **TriggerInfo** – označava dodatne informacije povezane s okidačem.


#### <a name="officeonenotenavigationnavigate"></a>Office.OneNote.Navigation.Navigate

Ključni signal korišten za nadzor mogućnosti korisnika OneNote za prelazak između stranica u aplikaciji OneNote.  Telemetrija korištena za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. Ako korisnici ne mogu prelaziti, time bi se izazvao incident visoke ozbiljnosti.

Prikupljaju se sljedeća polja:

- **FromNotebook** – jedinstveni identifikator bilježnice.

- **FromPage** – jedinstveni identifikator stranice.

- **FromSection** – jedinstveni identifikator odjeljka.

- **FromSectionGroup** – jedinstveni identifikator grupe odjeljka.

- **IsCurrentUserEduStudent** – označava ima li trenutnu korisnik ulogu studenta u obrazovnoj bilježnici ili nema.

- **IsEduNotebook** – označava je li trenutna stranica obrazovna bilježnica ili nije.

- **IsEduNotebookReadOnlyPage** – označava je li trenutna stranica ujedno stranica samo za čitanje u obrazovnoj bilježnici ili nije.

- **ToNotebook** – jedinstveni identifikator bilježnice.

- **ToPage** – jedinstveni identifikator stranice.

- **ToSection** – jedinstveni identifikator odjeljka.

- **ToSectionGroup** – jedinstveni identifikator grupe odjeljka.


#### <a name="officeonenotenotebookmanagementcreatenotebook"></a>Office.OneNote.NotebookManagement.CreateNotebook

Ključni signal korišten za nadzor mogućnosti korisnika OneNote za stvaranje bilježnica u aplikaciji OneNote.  Telemetrija korištena za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. Ako korisnici ne mogu stvarati bilježnice, time bi se izazvao incident visoke ozbiljnosti.

Prikupljaju se sljedeća polja:
    
- **NotebookID** – jedinstveni identifikator bilježnice.


#### <a name="officeonenotenotebookmanagementopennotebook"></a>Office.OneNote.NotebookManagement.OpenNotebook

Ključni signal korišten za nadzor mogućnosti korisnika OneNote za otvaranje bilježnica u aplikaciji OneNote.  Telemetrija korištena za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. Ako korisnici ne mogu otvarati bilježnice, time bi se izazvao incident visoke ozbiljnosti.

Prikupljaju se sljedeća polja:

-  **NotebookID** – jedinstveni identifikator bilježnice.

    
#### <a name="officeonenotesearchsearch"></a>Office.OneNote.Search.Search

Ključni ID signala korišten za nadzor mogućnosti korisnika aplikacije OneNote za pronalazak informacija na diljem tisuća stranica i bilježnica.   Telemetrija korištena za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. Ako korisnici ne mogu pronaći informacije diljem bilježnica, time bi se izazvao incident visoke ozbiljnosti.

Prikupljaju se sljedeća polja:

- **PageSearchResultCount** – označava broj rezultata pretraživanja pronađenih u načinu rada pretraživanja stranice.

-  **PageTimeToFirstResultInMs** – označava vrijeme koje je aplikaciji OneNote potrebno za pronalazak prvog podudaranja u načinu rada za pretraživanje stranica.
    
-  **PageTimeToLastResultInMs** – označava vrijeme koje je aplikaciji OneNote potrebno za pronalazak posljednjeg podudaranja u načinu rada za pretraživanje stranica.

-  **PageTimeToMedianResultInMs** – označava srednje vrijeme koje je aplikaciji OneNote potrebno za pronalazak svih podudaranja u načinu rada za pretraživanje stranica.

-  **SearchResultCount** – označava broj pronađenih rezultata pretraživanja.

-  **TagSearchResultCount** – označava broj pronađenih rezultata pretraživanja u načinu rada za pretraživanje oznaka.

-  **TagTimeToFirstResultInMs** – označava vrijeme koje je aplikaciji OneNote potrebno za pronalazak prvog podudaranja u načinu rada za pretraživanje oznaka.

-  **TagTimeToLastResultInMs** – označava vrijeme koje je aplikaciji OneNote potrebno za pronalazak posljednjeg podudaranja u načinu rada za pretraživanje oznaka.

-  **TagTimeToMedianResultInMs** – označava srednje vrijeme koje je aplikaciji OneNote potrebno za pronalazak svih podudaranja u načinu rada za pretraživanje.

-  **TimeToFirstResultInMs** – označava vrijeme koje je aplikaciji OneNote potrebno za pronalazak prvog podudaranja.

-  **TimeToLastResultInMs** – označava vrijeme koje je aplikaciji OneNote potrebno za pronalazak zadnjeg podudaranja.

-  **TimeToMedianResultInMs** – označava srednje vrijeme koje je aplikaciji OneNote potrebno za pronalazak svih podudaranja.

### <a name="officeonenotesigscriticalerrorencountered"></a>Office.OneNote.SIGS.CriticalErrorEncountered

Ovim se događajem bilježi ključan signal koji se koristi za nadziranje stanja servisa Signal Ingestion Service (SIG) evidentiranjem svake kritične pogreške. Kritične pogreške mogu blokirati cijeli SIGS, a to će nam pomoći da vidimo svaki takav problem čim korisnici na njih naiđu. 

Bez toga ćemo ovisiti o korisnicima koji prijavljuju probleme s kojima se suočavaju. Odsutnost takve telemetrije mogla bi znatno povećati vrijeme rješavanja takvih problema.

Prikupljaju se sljedeća polja: 

- **ErrorCode** – kôd problema na koji je naišao korisnik.


#### <a name="officeonenotestickynotesnotecreated-on-ios-onenotestickynotesnotecreated-on-android"></a>Office.OneNote.StickyNotes.NoteCreated (u sustavu iOS), OneNote.StickyNotes.NoteCreated (u sustavu Android)

Ovo je ključan signal koji se koristi za nadzor mogućnosti da korisnici aplikacije Sticky Notes mogu stvarati bilješke u aplikaciji.  Telemetrija se koristi za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. Ako korisnici ne mogu stvoriti bilješku, time bi se izazvao incident visoke ozbiljnosti.

Prikupljaju se sljedeća polja:

- **NoteLocalId** – prepoznatljiv jedinstveni identifikator dodijeljen bilješci u vrijeme kada korisnik stvori bilješku unutar aplikacije.

- **IsExportable** – zastavica koja označava je li ovaj događaj bio rezultat radnje korisnika ili ne. Treba se postaviti na Istinito jer je NoteCreated radnja koju aktivira korisnik.

- **StickyNotes-SDKVersion** – broj verzije koji označava verziju aplikacije Sticky Notes koju korisnik koristi. Omogućuje prepoznavanje verzija proizvoda s kojima se pojavljuje problem kako bismo mogli ispravno odrediti njegov prioritet.


#### <a name="officeonenotestickynotesnoteviewed-on-ios-onenotestickynotesnoteviewed-on-android"></a>Office.OneNote.StickyNotes.NoteViewed (u sustavu iOS), OneNote.StickyNotes.NoteViewed (u sustavu Android)

Ovo je ključan signal koji se koristi za nadzor mogućnosti da korisnici aplikacije Sticky Notes mogu stvarati bilješke u aplikaciji.  Telemetrija se koristi za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. Ako korisnici ne mogu stvoriti bilješku, time bi se izazvao incident visoke ozbiljnosti.

Prikupljaju se sljedeća polja:

- **HasImages** – zastavica koja označava jesu li u prikazanoj bilješci pohranjene slike.

- **IsExportable** – zastavica koja označava je li ovaj događaj bio rezultat radnje korisnika ili ne. Treba se postaviti na Istinito jer je NoteViewed radnja koju aktivira korisnik.

- **NoteLocalId** – prepoznatljiv jedinstveni identifikator dodijeljen bilješci u vrijeme kada korisnik stvori bilješku unutar aplikacije.

- **StickyNotes-SDKVersion** – broj verzije koji označava verziju aplikacije Sticky Notes koju korisnik koristi. Omogućuje prepoznavanje verzija proizvoda s kojima se pojavljuje problem kako bismo mogli ispravno odrediti njegov prioritet.


#### <a name="officeonenotestoragenotebooksyncresult"></a>Office.OneNote.Storage.NotebookSyncResult
 
Ovaj događaj zapisuje rezultat sinkronizacije bilježnice. Koristi se za otkrivanje broja jedinstvenih ciljeva sinkronizacije tijekom izračuna rezultata sinkronizacije aplikacije OneNote.
 
Prikupljaju se sljedeća polja

- **CachedError_Code** – numerirani ili alfanumerički kod koji se koristi za određivanje prirode predmemorirane pogreške i/ili razloga pojave
    
- **CachedError_Description** – opis predmemorirane pogreške

- **CachedError_Tag** – označava mjesto na kojem se predmemorirana pogreška prikazuje u kodu

- **CachedError_Type** – vrsta predmemorirane pogreške, na primjer, Win32Error itd.

- **ExecutionTime** – vrijeme u milisekundama potrebno za repliciranje bilježnice

- **Gosid** – globalni ID prostora objekta

- **IdentityType** – vrsta identiteta, npr. Windows Live, Org ID itd.

- **InitialReplicationInSession** – označava je li ova replikacija prva replikacija bilježnice nakon otvaranja ili nije

- **IsBackgroundSync** – označava je li ovo sinkronizacija u pozadini ili nije

- **IsCachedErrorSuppressed** – označava je li predmemorirana pogreška potisnuta ili nije

- **IsCachedErrorUnexpected** – označava je li predmemorirana pogrešna neočekivana ili nije

- **IsNotebookErrorSuppressed** – označava je li pogreška sinkronizacije na razini bilježnice potisnuta ili nije

- **IsNotebookErrorUnexpected** – označava je li pogreška sinkronizacije na razini bilježnice neočekivana ili nije

- **IsSectionErrorSuppressed** – označava je li pogreška sinkronizacije odjeljka potisnuta ili nije

- **IsSectionErrorUnexpected** – označava je li pogreška sinkronizacije odjeljka neočekivana ili nije

- **IsUsingRealtimeSync** – označava koristi li sinkronizacija bilježnice suvremenu sinkronizaciju sadržaja stranice ili ne

- **LastAttemptedSync** – vremenska oznaka za trenutak kada se proveo zadnji pokušaj sinkronizacije bilježnice

- **LastBackgroundSync** – vremenska oznaka za trenutak kada se proveo posljednji pokušaj sinkronizacije u pozadini

- **LastNotebookViewedDate** – datum kada je bilježnica zadnji put prikazana

- **LastSuccessfulSync** – vremenska oznaka za trenutak kada se bilježnica uspješno prethodno sinkronizirala

- **NeedToRestartBecauseOfInconsistencies** – treba li se sinkronizacija ponovno pokrenuti zbog nedosljednosti ili ne

- **NotebookErrorCode** – kod pogreške sinkronizacije na razini bilježnice spremljen je na prostoru grafikona bilježnice

- **NotebookId** – ID bilježnice

- **NotebookType** – vrsta bilježnice

- **ReplicatingAgainBecauseOfInconsistencies** – pokreće li se sinkronizacija ponovno zbog nedosljednosti ili ne

- **SectionError_Code** – numerirani ili alfanumerički kod koji se koristi za određivanje prirode pogreške sinkronizacije odjeljka i/ili razloga pojave

- **SectionError_Description** – opis pogreške sinkronizacije odjeljka

- **SectionError_Tag** – označava mjesto na kojem se pogreška sinkronizacije odjeljka prikazuje u kodu

- **SectionError_Type** – vrsta pogreške sinkronizacije odjeljka, na primjer, Win32Error itd.

- **Success** – je li bilježnica uspješno sinkronizirana ili nije

- **SyncDestinationType** – vrsta odredišta sinkronizacije, npr. OneDrive ili SharePoint Online

- **SyncId** – broj jedinstven svakoj sinkronizaciji bilježnice

- **SyncWasFirstInSession** – označava je li ova sinkronizacija prva sinkronizacija u trenutnoj sesiji

- **SyncWasUserInitiated** – označava je li korisnik sinkronizacije pokrenut ili nije

- **TenantId** – ID klijenta sustava SharePoint

- **TimeSinceLastAttemptedSync** – vrijeme proteklo od posljednjeg pokušaja sinkronizacije bilježnice

- **TimeSinceLastSuccessfulSync** – vrijeme proteklo od posljednje uspješne sinkronizacije bilježnice


#### <a name="officeonenotesystemapplifecycleapplaunch"></a>Office.OneNote.System.AppLifeCycle.AppLaunch

Ključni signal koji se koristi za osiguravanje da korisnici aplikacije OneNote mogu uspješno pokrenuti aplikaciju. Telemetrija se koristi za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. Ako korisnici ne mogu pokrenuti aplikaciju u našem prozoru izvedbe, time bi se izazvao incident visoke ozbiljnosti.

Prikupljaju se sljedeća polja:     Nijedno

#### <a name="officeoutlookdesktopaccountconfigurationcreateaccountresult"></a>Office.Outlook.Desktop.AccountConfiguration.CreateAccountResult

Rezultat dodavanja računa za Outlook u novi profil, u prikazu Office Backstage ili iz dijaloškog okvira Postavke računa. Kako ne bi bilo porasta u pogreškama, podaci se aktivno nadziru. Također analiziramo podatke kako bismo pronašli područja poboljšanja. Trudimo se poboljšati stopu uspjeha sa svakim izdanjem.

Prikupljaju se sljedeća polja:

  - **AccountCreationResult** – rezultat (uspjeh, pogreška, otkazivanje itd.) dodavanja računa u Outlook.

  - **AccountCreationTime** – trajanje pokušaja stvaranja računa

  - **AccountInfoSource** – izvor postavki računa (npr. AutoDiscover, GuessSmart, AutoDetect itd.)

  - **AccountType** – vrsta računa koji se konfigurira.

  - **HashedEmailAddress** – raspršena adresa e-pošte

  - **ShowPasswordPageFlightEnabled** – pokazatelj je li omogućena međuverzija ShowPopImapPasswordPage

#### <a name="officeoutlookdesktopaccountconfigurationrepairaccountresult"></a>Office.Outlook.Desktop.AccountConfiguration.RepairAccountResult

Rezultat popravka računa ili promjene naprednih postavki računa. Kako ne bi bilo porasta u pogreškama, podaci se aktivno nadziru. Također analiziramo podatke kako bismo pronašli područja poboljšanja. S obzirom da je ovo novo (restrukturirano) okruženje, želimo biti sigurni da sve radi kako treba.

Prikupljaju se sljedeća polja:

  - **AccountInfoSource** – izvor informacija o računu za račun korišten za pokušaj popravka

  - **AccountType** – vrsta računa za koji je pokušan popravak računa

  - **HashedEmailAddress** – raspršena adresa e-pošte

  - **ManualRepairRequested** – pokazatelj je li zatražen ručni popravak

  - **Rezultat** – rezultat pokušaja popravka računa. Na primjer: „Uspjeh“ ili „Fail\_SaveChangesToAccount“

#### <a name="officeoutlookdesktopaccountconfigurationupdatepasswordresult"></a>Office.Outlook.Desktop.AccountConfiguration.UpdatePasswordResult

Rezultat ažuriranja lozinke za račun na padajućem izborniku Postavke računa. Kako ne bi bilo porasta u pogreškama, podaci se aktivno nadziru. Također analiziramo podatke kako bismo pronašli područja poboljšanja. S obzirom da je ovo novo (restrukturirano) okruženje, želimo biti sigurni da sve radi kako treba.

Prikupljaju se sljedeća polja:

  - **AccountType** – vrsta računa za koji je pokušano ažuriranje lozinke

  - **HashedEmailAddress** – raspršena adresa e-pošte

  - **Rezultat** – rezultat pokušaja ažuriranja lozinke. Na primjer: „Uspjeh“ ili „Fail\_AllowLessSecureAppsDisabled“


#### <a name="officeoutlookdesktopstorescreatenewstore"></a>Office.Outlook.Desktop.Stores.CreateNewStore

Prikuplja rezultat stvaranja nove trgovine (s vrstom i verzijom) i kôd rezultata. Aktivno pratimo taj događaj radi praćenja stanja korisnikove mogućnosti sinkroniziranja i pohrane pošte lokalno, arhiviranje poruka e-pošte (u PST) ili korištenje grupa.

Prikupljaju se sljedeća polja:

  - **Standardna HVA aktivnost** s prilagođenim opterećenjem

  - **StoreType** – vrsta trgovine koju stvara OST/PST/NST

  - **StoreVersion** – verzija trgovine koja stvara Small/Large/Tardis

#### <a name="officeoutlookmacaccountaddworkflow"></a>Office.Outlook.Mac.AccountAddWorkflow

Rezultat dodavanja računa u programu Outlook. Kako ne bi bilo porasta u pogreškama, podaci se nadziru. Također analiziramo podatke kako bismo pronašli područja poboljšanja. Trudimo se poboljšati stopu uspjeha sa svakim izdanjem. 

Prikupljaju se sljedeća polja:

- **AccountConfigMethod** – način konfiguracije računa

- **AccountType** – vrsta računa koji se konfigurira

- **AccountWorkflowSession** – sesija tijekom koje je proveden pokušaj tijeka rada računa

- **SessionDuration** – trajanje sesije 

- **ThreadId** – identifikator za niz


#### <a name="officeoutlookmacaccountonboardingflow"></a>Office.Outlook.Mac.AccountOnboardingFlow

Rezultat dodavanja računa u programu Outlook korištenjem novog iskustva konfiguracije računa. Kako ne bi bilo porasta u pogreškama, podaci se nadziru. Također analiziramo podatke kako bismo pronašli područja poboljšanja. Trudimo se poboljšati stopu uspjeha sa svakim izdanjem. 

Prikupljaju se sljedeća polja:

- **AccountConfigAutoSignIn** – automatska konfiguracija računa koju je postavio administrator

- **AccountConfigDomain** – domena navedena tijekom konfiguracije računa 

- **AccountConfigEntryPoint** – ulazna točka u kojoj je korisnik unio konfiguraciju računa 

- **AccountConfigErrorCode** – kod pogreške koji je nastupio tijekom konfiguracije računa 

- **AccountConfigErrorString** – pogreška koja je nastupila tijekom konfiguracije računa

- **AccountConfigMethod** – način konfiguracije računa

- **AccountConfigPhase** – trenutni korak tijeka rada konfiguracije računa

- **AccountConfigPhaseFrom** – početni korak tijeka rada konfiguracije računa 

- **AccountConfigPhaseTo** – zadnji korak tijeka rada konfiguracije računa 

- **AccountType** – vrsta računa koji se konfigurira

- **AccountWorkflowSession** – sesija tijekom koje je proveden pokušaj tijeka rada računa

- **SessionDuration** – trajanje sesije


#### <a name="officeoutlookmacdeleteaccountusage"></a>Office.Outlook.Mac.DeleteAccountUsage

Rezultat brisanja računa u programu Outlook. Kako ne bi bilo porasta u pogreškama, podaci se nadziru. Također analiziramo podatke kako bismo pronašli područja poboljšanja. Trudimo se poboljšati stopu uspjeha sa svakim izdanjem. 

Prikupljaju se sljedeća polja:

- **AccountType** – vrsta računa koji se konfigurira

- **AccountID** – identifikator računa

- **DeprovisionAccount** – označava je li račun uklonjen s poslužitelja

- **IsFastDelete** – označava je li račun izbrisan na niti u pozadini

#### <a name="officepowerpointdocoperationclose"></a>Office.PowerPoint.DocOperation.Close

Prikuplja se kada su zatvorene prezentacije programa PowerPoint. Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi u postupku zatvaranja koji obuhvaćaju održavanje i sinkroniziranje korisničkih podataka. Microsoft koristi te podatke da bi osigurao da zatvaranje funkcionira prema očekivanjima i da se korisnički sadržaj uspješno održava.

Prikupljaju se sljedeća polja:

  - **Data\_AddDocTelemetryResult:long –** ima li ova stavka zapisnika svu potrebnu telemetriju dokumenta (polja Data\_Doc\_\*)? Ako ne, zašto?

  - **Data\_AutoSaveDisabledReasons:string –** unaprijed definiran skup vrijednosti koji naznačuje zašto je automatsko spremanje onemogućeno na ovom dokumentu? (Pogreška spajanja, pogreška spremanja, pravilnik grupe itd.)

  - **Data\_CloseReason:long –** kako je izvršeno zatvaranje? Zatvaranje dokumenta? Zatvaranje aplikacije?

  - **Data\_CppUncaughtExceptionCount:long –** broj neobrađenih iznimki

  - **Data\_DetachedDuration:long –** vrijeme tijekom kojeg je aktivnost isključena/nije pokrenuta

  - **Data\_Doc\_AccessMode:long –** kako je dokument otvoren (samo za čitanje | samo za pisanje)

  - **Data\_Doc\_AssistedReadingReasons:long –** unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

  - **Data_Doc_AsyncOpenKind:long –** označava je li otvorena predmemorirana verzija dokumenta u oblaku i koja je logika za asinkrono osvježavanje korištena.

  - **Data\_Doc\_ChunkingType:long –** kako je dokument pohranjen u sustavu SharePoint

  - **Data\_Doc\_EdpState:long –** stanje dokumenta s obzirom na zaštitu korporativnih podataka

  - **Data\_Doc\_Ext:string –** nastavak dokumenta

  - **Data\_Doc\_Extension:string –** nastavak dokumenta

  - **Data\_Doc\_FileFormat:long –** unaprijed definirani skup vrijednosti oblika datoteke (precizniji od nastavka)

  - **Data\_Doc\_Fqdn:string –** mjesto pohrane dokumenta (SharePoint.com, live.net), dostupno samo za domene sustava Office 365

  - **Data\_Doc\_FqdnHash:string –** raspršivanje mjesta pohrane dokumenta

  - **Data\_Doc\_IdentityTelemetryId:string –** jedinstveni GUID korisnika

  - **Data\_Doc\_IdentityUniqueId:string –** jedinstveni identifikator identiteta korištenog za akciju zajedničkih dokumenata

  - **Data\_Doc\_IOFlags:long –** bit-maska za razne zastavice vezane uz ulaz i izlaz za određeni dokument

  - **Data\_Doc\_IrmRights:long –** unaprijed definiran skup vrijednosti za vrstu informacija koju upravljanje pravima na informacije primjenjuje na ovom dokumentu (proslijedi, odgovori, SecureReader, uređivanje itd.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool –** istinito ako je HTTP zaglavlje „IsCloudCollabEnabled“ već prihvaćeno iz zahtjeva MOGUĆNOSTI.

  - **Data\_Doc\_IsIncrementalOpen:bool –** je li dokument otvoren inkrementalno (nova značajka koja otvara dokument bez potrebe za preuzimanjem cijelog dokumenta)

  - **Data\_Doc\_IsOcsSupported:bool –** podržava li dokument suautorstvo pomoću novog servisa OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool –** provjerava otvara li se dokument iz lokalne predmemorije

  - **Data\_Doc\_IsSyncBacked:bool –** provjerava otvara li se dokument iz mape koja koristi aplikaciju OneDrive za povratnu sinkronizaciju

  - **Data\_Doc\_Location:long –** unaprijed definiran skup vrijednosti mjesta na kojima se dokument pohranjuje (lokalno, SharePoint, WOPI, mreža itd.)

  - **Data\_Doc\_LocationDetails:long –** unaprijed definiran skup vrijednosti detaljnijih lokacija (mapa Temp, mapa preuzimanja, dokumenti servisa One Drive, slike servisa One Drive itd.)

  - **Data\_Doc\_NumberCoAuthors:long –** broj suautora prilikom otvaranja dokumenta

  - **Data\_Doc\_PasswordFlags:long –** unaprijed definirani skup vrijednosti načina na koji je dokument šifriran pomoću lozinke (nema, lozinka za čitanje, lozinka za uređivanje)

  - **Data\_Doc\_ReadOnlyReasons:long –** unaprijed definirani skup vrijednosti koji naznačuje zašto je dokument označen samo za čitanje (zaključan na poslužitelju, konačni dokument, zaštićen lozinkom za uređivanje itd.)

  - **Data\_Doc\_ResourceIdHash:string –** raspršivanje identifikatora resursa za dokumente pohranjene u oblaku

  - **Data_Doc_RtcType –** označava kako je kanal u stvarnom vremenu (RTC) postavljen za trenutnu datoteku (onemogućen, nepodržan, na zahtjev, uvijek uključen itd.).

  - **Data\_Doc\_ServerDocId:string –** nepromjenjivi identifikator za dokumente pohranjene u oblaku

  - **Data\_Doc\_ServerProtocol:long –** unaprijed definirani skup vrijednosti o protokolu koji se koristi za komuniciranje s poslužiteljem (Http, Cobalt, WOPI itd.)

  - **Data\_Doc\_ServerType:long –** unaprijed definiran skup vrijednosti za vrstu poslužitelja (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long –** provjerava temelji li se poslužitelj na sustavu Office14, Office15 ili Office 16

  - **Data\_Doc\_SessionId:long –** generirani GUID koji identificira instancu dokumenta u sklopu iste sesije procesa

  - **Data\_Doc\_SharePointServiceContext:string –** neprozirni niz, obično GridManagerID.FarmID. Korisno za korelaciju klijentskih i poslužiteljskih zapisnika

  - **Data\_Doc\_SizeInBytes:long –** veličina dokumenta u bajtovima

  - **Data\_Doc\_SpecialChars:long –** bit-maska koja pokazuje posebne znakove u URL-u ili putu dokumenta

  - **Data\_Doc\_StorageProviderId:string –** niz koji određuje davatelja pohrane dokumenta, primjerice „DropBox“

  - **Data\_Doc\_StreamAvailability:long –** unaprijed definirani skup vrijednosti statusa toka dokumenta (dostupno, trajno onemogućeno, nije dostupno)

  - **Data\_Doc\_UrlHash:string –** raspršivanje punog URL-a dokumenata pohranjenih u oblaku

  - **Data\_Doc\_UsedWrsDataOnOpen:bool –** istinito ako je datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka na glavnom računalu

  - **Data\_Doc\_WopiServiceId:string –** identifikator WOPI servisa, na primjer, „Dropbox“

  - **Data\_DocHasStorage:bool –** ima li ovaj dokument lokalnu pohranu?

  - **Data\_fLifeguarded:bool –** je li dokument ikad popravljen pomoću značajke lifeguard (značajka za popravljanje pogrešaka dokumenta bez slanja upita korisniku)?

  - **Data\_IsDocAutoSaveable:bool –** može li se prezentacija automatski spremiti?

  - **Data\_IsDocDirty:bool –** ima li prezentacija promjene koje još nisu spremljene?

  - **Data\_IsNewDoc:bool –** radi li se o novom ili postojećem dokumentu

  - **Data\_IsRecoveredDoc:bool –** je li dokument oporavljen? (Ako je došlo do rušenja prethodne sesije, u sljedećoj sesiji prikazat ćemo okno za oporavak dokumenta)

  - **Data\_NewDocDiscarded:bool –** je li nova prezentacija odbačena bez spremanja

  - **Data\_OCSClosingDlgCanceled:bool –** ako prijenos čeka na OCS dok korisnik zatvara dokument, korisniku se prikazuje dijaloški okvir s porukom da pričeka. Koju je mogućnost korisnik odabrao?

  - **Data\_OCSClosingDlgExpired:bool –** je li dijaloški okvir istekao (nakon 1 minute)?

  - **Data\_OCSClosingStatus:long –** koji je konačni status OCS-a (u CSI-ju, Closable, u OCS prijelazu, u CSI prijelazu itd.)

  - **Data\_OCSClosingWaitDurationMS:long –** koliko je vremena korisnik čekao na prijenos OCS-a

  - **Data\_OCSHandleTransitionResult:long –** unaprijed definirani skup vrijednosti rezultata prijelaza izvedenog tijekom zatvaranja (već pokušano, nastavi zatvaranje itd.)

  - **Data\_ServerDocId:string –** GUID za jedinstveno identificiranje dokumenta

  - **Data\_StopwatchDuration:long –** ukupno vrijeme za aktivnost

  - **Data\_UserContinuedZRTClose:bool –** nakon prikazivanja dijaloškog okvira prilikom zatvaranja, je li korisnik odabrao „Nastavi” za zatvaranje?

#### <a name="officepowerpointdocoperationnewdocument"></a>Office.PowerPoint.DocOperation.NewDocument

Prikuplja se kada PowerPoint stvori novu prezentaciju.  Obuhvaća metriku uspjeha, neuspjeha i performansi.

Te se informacije upotrebljavaju da bismo uspješno stvorili datoteke bez smanjenih performansi.

Prikupljaju se sljedeća polja:

  - **NewDocumentType** – je li novi dokument stvoren iz predloška ili je stvoren kao prazan?

  - **FLifeguarded** – je li zaštićen životni vijek dokumenta (značajka koja vraća stanje oštećenog dokumenta bez slanja upita korisniku)

#### <a name="officepowerpointdocoperationopencompleteprotocol"></a>Office.PowerPoint.DocOperation.OpenCompleteProtocol

Prikuplja se kada PowerPoint otvara prezentacije. Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi u završnim fazama postupka otvaranja.

Microsoft koristi te podatke da bi značajka funkcionirala prema očekivanjima i kako ne bi bilo smanjenih performansi prilikom otvaranja prezentacija.

Prikupljaju se sljedeća polja:

  - **Data\_AntiVirusScanMethod:long –** unaprijed definirani skup vrijednosti vrste antivirusnog pregleda (IOAV, AMSI, Nema itd.)

  - **Data\_AntiVirusScanStatus:long –** unaprijed definirani skup vrijednosti antivirusnog pregleda za svaki otvoreni dokument (NoThreatsDetected, Failed, MalwareDetected itd.)

  - **Data\_CloseAndReopen:bool –** je li ovaj dokument zatvoren i ponovno otvoren?

  - **Data\_DetachedDuration:long –** vrijeme tijekom kojeg je aktivnost isključena/nije pokrenuta

  - **Data\_Doc\_AccessMode:long –** kako je dokument otvoren (samo za čitanje | samo za pisanje)

  - **Data\_Doc\_AssistedReadingReasons:long –** unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

  - **Data_Doc_AsyncOpenKind:long –** označava je li otvorena predmemorirana verzija dokumenta u oblaku i koja je logika za asinkrono osvježavanje korištena.

  - **Data\_Doc\_ChunkingType:long –** kako je dokument pohranjen u sustavu SharePoint

  - **Data\_Doc\_EdpState:long –** stanje dokumenta s obzirom na zaštitu korporativnih podataka

  - **Data\_Doc\_Ext:string –** nastavak dokumenta

  - **Data\_Doc\_Extension:string –** nastavak dokumenta

  - **Data\_Doc\_FileFormat:long –** unaprijed definirani skup vrijednosti oblika datoteke (precizniji od nastavka)

  - **Data\_Doc\_Fqdn:string –** mjesto pohrane dokumenta (SharePoint.com, live.net), dostupno samo za domene sustava Office 365

  - **Data\_Doc\_FqdnHash:string –** raspršivanje mjesta pohrane dokumenta

  - **Data\_Doc\_IdentityTelemetryId:string –** jedinstveni GUID korisnika

  - **Data\_Doc\_IdentityUniqueId:string –** jedinstveni identifikator identiteta korištenog za akciju zajedničkih dokumenata

  - **Data\_Doc\_IOFlags:long –** bit-maska za razne zastavice vezane uz ulaz i izlaz za određeni dokument

  - **Data\_Doc\_IrmRights:long –** unaprijed definiran skup vrijednosti za vrstu informacija koju upravljanje pravima na informacije primjenjuje na ovom dokumentu (proslijedi, odgovori, SecureReader, uređivanje itd.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool –** istinito ako je HTTP zaglavlje „IsCloudCollabEnabled“ već prihvaćeno iz zahtjeva MOGUĆNOSTI.

  - **Data\_Doc\_IsIncrementalOpen:bool –** je li dokument otvoren inkrementalno (nova značajka koja otvara dokument bez potrebe za preuzimanjem cijelog dokumenta)

  - **Data\_Doc\_IsOcsSupported:bool –** podržava li dokument suautorstvo pomoću novog servisa OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool –** otvara li se dokument iz lokalne predmemorije?

  - **Data\_Doc\_IsSyncBacked:bool –** otvara li se dokument iz mape koja koristi aplikaciju OneDrive za povratnu sinkronizaciju

  - **Data\_Doc\_Location:long –** unaprijed definiran skup vrijednosti mjesta na kojima se dokument pohranjuje (lokalno, SharePoint, WOPI, mreža itd.)

  - **Data\_Doc\_LocationDetails:long –** unaprijed definiran skup vrijednosti detaljnijih lokacija (mapa Temp, mapa preuzimanja, dokumenti servisa One Drive, slike servisa One Drive itd.)

  - **Data\_Doc\_NumberCoAuthors:long –** broj suautora prilikom otvaranja dokumenta

  - **Data\_Doc\_PasswordFlags:long –** unaprijed definirani skup vrijednosti načina na koji je dokument šifriran pomoću lozinke (nema, lozinka za čitanje, lozinka za uređivanje)

  - **Data\_Doc\_ReadOnlyReasons:long –** unaprijed definirani skup vrijednosti koji naznačuje zašto je dokument označen samo za čitanje (zaključan na poslužitelju, konačni dokument, zaštićen lozinkom za uređivanje itd.)

  - **Data\_Doc\_ResourceIdHash:string –** raspršivanje identifikatora resursa za dokumente pohranjene u oblaku

  - **Data_Doc_RtcType –** označava kako je kanal u stvarnom vremenu (RTC) postavljen za trenutnu datoteku (onemogućen, nepodržan, na zahtjev, uvijek uključen itd.).

  - **Data\_Doc\_ServerDocId:string –** nepromjenjivi identifikator za dokumente pohranjene u oblaku

  - **Data\_Doc\_ServerProtocol:long –** unaprijed definirani skup vrijednosti o protokolu koji se koristi za komuniciranje s poslužiteljem (Http, Cobalt, WOPI itd.)

  - **Data\_Doc\_ServerType:long –** unaprijed definiran skup vrijednosti za vrstu poslužitelja (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long –** provjerava temelji li se poslužitelj na sustavu Office14, Office15 ili Office 16

  - **Data\_Doc\_SessionId:long –** generirani GUID koji identificira instancu dokumenta u sklopu iste sesije procesa

  - **Data\_Doc\_SharePointServiceContext:string –** neprozirni niz, obično GridManagerID.FarmID. Korisno za korelaciju klijentskih i poslužiteljskih zapisnika

  - **Data\_Doc\_SizeInBytes:long –** veličina dokumenta u bajtovima

  - **Data\_Doc\_SpecialChars:long –** bit-maska koja pokazuje posebne znakove u URL-u ili putu dokumenta

  - **Data\_Doc\_StorageProviderId:string –** niz koji određuje davatelja pohrane dokumenta, primjerice „DropBox“

  - **Data\_Doc\_StreamAvailability:long –** unaprijed definirani skup vrijednosti statusa toka dokumenta (dostupno, trajno onemogućeno, nije dostupno)

  - **Data\_Doc\_UrlHash:string –** raspršivanje punog URL-a dokumenata pohranjenih u oblaku

  - **Data\_Doc\_UsedWrsDataOnOpen:bool –** istinito ako je datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka na glavnom računalu

  - **Data\_Doc\_WopiServiceId:string –** identifikator WOPI servisa, na primjer, „Dropbox“

  - **Data\_ExecutionCount:long –** koliko smo puta izvršili protokol IncOpen prije izvršavanja ovog protokola (OpenComplete)

  - **Data\_FailureComponent:long –** unaprijed definirani skup vrijednosti koji označava koja je komponenta uzrokovala neuspjeh ovog protokola? (Conflict, CSI, Internal itd.)

  - **Data\_FailureReason:long –** unaprijed definiran skup vrijednosti razloga neuspjeha (FileIsCorrupt, BlockedByAntivirus itd.)

  - **Data_FullDownloadRoundTripCount:long –** broj vraćanja poslužitelju provedenih za preuzimanje cijelog dokumenta.
  
  - **Data_IsProtocolRunInIncOpenMode:bool –** bio je protokol za inkrementalno preuzimanje, što je preuzimanje kod kojeg su dijelovi dokumenta preuzeti nakon što se prethodno prikazao korisniku.

  - **Data\_MethodId:long –** koji je redak koda interno zadnji izvršen

  - **Data\_StopwatchDuration:long –** ukupno vrijeme za aktivnost

  - **Data\_TimeToEdit:long –** vrijeme potrebno da bi se dokument mogao uređivati

  - **Data\_TimeToView:long –** vrijeme potrebno za prikazivanje prvog slajda dokumenta

  - **Data\_UnhandledException:bool –** ima li neobrađenih lokalnih iznimaka?

#### <a name="officepowerpointdocoperationsave"></a>Office.PowerPoint.DocOperation.Save

Prikuplja se svaki put kada PowerPoint izvodi spremanje pomoću modernog puta koda. Obuhvaća vrstu rezultata uspješno ili neuspješno metrike performansi spremanja i relevantnih metapodataka dokumenta.  Problemi sa spremanjem mogu uzrokovati gubitak podataka. Microsoft koristi te podatke da bi osigurao da značajka funkcionira prema očekivanjima i da se korisnički sadržaj uspješno održava.

Prikupljaju se sljedeća polja:

  - **Data\_AddDocTelemetryResult:long –** ima li ova stavka zapisnika svu potrebnu telemetriju dokumenta (polja Data\_Doc\_\*)? Ako ne, zašto?

  - **Data\_BeforeSaveEvent:long –** vrijeme potrebno za podizanje dokumenta prije događaja spremanja

  - **Data\_CheckDownRevSaveTimeMS:long –** vrijeme potrebno za provjeru revizije

  - **Data\_CheckMacroSaveTimeMS:long –** vrijeme potrebno za spremanje makronaredbi

  - **Data\_ClearAutoSaveTimeMS:long –** vrijeme potrebno za brisanje zastavice automatskog spremanja

  - **Data\_ClearDirtyFlagTimeMS:long –** vrijeme potrebno za brisanje zastavice prljavog dokumenta

  - **Data\_CloneDocumentTimeMS:long –** vrijeme potrebno za kloniranje dokumenta prije pokretanja spremanja

  - **Data\_CommitTransactionTimeMS:long –** vrijeme potrebno za izvršavanje transakcije spremanja

  - **Data\_CppUncaughtExceptionCount:long –** neuhvaćene lokalne iznimke dok je aktivnost pokrenuta

  - **Data\_DetachedDuration:long –** vrijeme tijekom kojeg je aktivnost isključena/nije pokrenuta

  - **Data\_Doc\_AccessMode:long –** kako je dokument otvoren (samo za čitanje | samo za pisanje)

  - **Data\_Doc\_AssistedReadingReasons:long –** unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

  - **Data_Doc_AsyncOpenKind:long –** označava je li otvorena predmemorirana verzija dokumenta u oblaku i koja je logika za asinkrono osvježavanje korištena.

  - **Data\_Doc\_ChunkingType:long –** kako je dokument pohranjen u sustavu SharePoint

  - **Data\_Doc\_EdpState:long –** stanje dokumenta s obzirom na zaštitu korporativnih podataka

  - **Data\_Doc\_Ext:string –** nastavak dokumenta

  - **Data\_Doc\_Extension:string –** nastavak dokumenta

  - **Data\_Doc\_FileFormat:long –** unaprijed definirani skup vrijednosti oblika datoteke (precizniji od nastavka)

  - **Data\_Doc\_Fqdn:string –** mjesto pohrane dokumenta (SharePoint.com, live.net), dostupno samo za domene sustava Office 365

  - **Data\_Doc\_FqdnHash:string –** raspršivanje mjesta pohrane dokumenta

  - **Data\_Doc\_IdentityTelemetryId:string –** jedinstveni GUID korisnika

  - **Data\_Doc\_IdentityUniqueId:string –** jedinstveni identifikator identiteta korištenog za akciju zajedničkih dokumenata

  - **Data\_Doc\_IOFlags:long –** bit-maska za razne zastavice vezane uz ulaz i izlaz za određeni dokument

  - **Data\_Doc\_IrmRights:long –** unaprijed definiran skup vrijednosti za vrstu informacija koju upravljanje pravima na informacije primjenjuje na ovom dokumentu (proslijedi, odgovori, SecureReader, uređivanje itd.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool –** istinito ako je HTTP zaglavlje „IsCloudCollabEnabled“ već prihvaćeno iz zahtjeva MOGUĆNOSTI.

  - **Data\_Doc\_IsIncrementalOpen:bool –** je li dokument otvoren inkrementalno (nova značajka koja otvara dokument bez potrebe za preuzimanjem cijelog dokumenta)

  - **Data\_Doc\_IsOcsSupported:bool –** podržava li dokument suautorstvo pomoću novog servisa OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool –** provjerava otvara li se dokument iz lokalne predmemorije

  - **Data\_Doc\_IsSyncBacked:bool –** otvara li se dokument iz mape koja koristi aplikaciju OneDrive za povratnu sinkronizaciju

  - **Data\_Doc\_Location:long –** unaprijed definiran skup vrijednosti mjesta na kojima se dokument pohranjuje (lokalno, SharePoint, WOPI, mreža itd.)

  - **Data\_Doc\_LocationDetails:long –** unaprijed definiran skup vrijednosti detaljnijih lokacija (mapa Temp, mapa preuzimanja, dokumenti servisa One Drive, slike servisa One Drive itd.)

  - **Data\_Doc\_NumberCoAuthors:long –** broj suautora prilikom otvaranja dokumenta

  - **Data\_Doc\_PasswordFlags:long –** unaprijed definirani skup vrijednosti načina na koji je dokument šifriran pomoću lozinke (nema, lozinka za čitanje, lozinka za uređivanje)

  - **Data\_Doc\_ReadOnlyReasons:long –** unaprijed definirani skup vrijednosti koji naznačuje zašto je dokument označen samo za čitanje (zaključan na poslužitelju, konačni dokument, zaštićen lozinkom za uređivanje itd.)

  - **Data\_Doc\_ResourceIdHash:string –** raspršivanje identifikatora resursa za dokumente pohranjene u oblaku

  - **Data_Doc_RtcType –** označava kako je kanal u stvarnom vremenu (RTC) postavljen za trenutnu datoteku (onemogućen, nepodržan, na zahtjev, uvijek uključen itd.).

  - **Data\_Doc\_ServerDocId:string –** nepromjenjivi identifikator za dokumente pohranjene u oblaku

  - **Data\_Doc\_ServerProtocol:long –** unaprijed definirani skup vrijednosti o protokolu koji se koristi za komuniciranje s poslužiteljem (Http, Cobalt, WOPI itd.)

  - **Data\_Doc\_ServerType:long –** unaprijed definiran skup vrijednosti za vrstu poslužitelja (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long –** provjerava temelji li se poslužitelj na sustavu Office14, Office15 ili Office 16

  - **Data\_Doc\_SessionId:long –** generirani GUID koji identificira instancu dokumenta u sklopu iste sesije procesa

  - **Data\_Doc\_SharePointServiceContext:string –** neprozirni niz, obično GridManagerID.FarmID. Korisno za korelaciju klijentskih i poslužiteljskih zapisnika

  - **Data\_Doc\_SizeInBytes:long –** veličina dokumenta u bajtovima

  - **Data\_Doc\_SpecialChars:long –** bit-maska koja pokazuje posebne znakove u URL-u ili putu dokumenta

  - **Data\_Doc\_StorageProviderId:string –** niz koji određuje davatelja pohrane dokumenta, primjerice „DropBox“

  - **Data\_Doc\_StreamAvailability:long –** unaprijed definirani skup vrijednosti statusa toka dokumenta (dostupno, trajno onemogućeno, nije dostupno)

  - **Data\_Doc\_UrlHash:string –** raspršivanje punog URL-a dokumenata pohranjenih u oblaku

  - **Data\_Doc\_UsedWrsDataOnOpen:bool –** istinito ako je datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka na glavnom računalu

  - **Data\_Doc\_WopiServiceId:string –** identifikator WOPI servisa, na primjer, „Dropbox“

  - **Data\_DurationUAEOnSaveStartedMs:long –** vrijeme potrebno za zatvaranje nepoznate aplikacije tijekom spremanja

  - **Data\_EnsureSaveTransactionTimeMS:long –** vrijeme potrebno za stvaranje transakcije spremanja ako već ne postoji

  - **Data\_FailureComponent:long–** unaprijed definirani skup vrijednosti koji označava koja je komponenta uzrokovala neuspjeh ovog protokola? (Conflict, CSI, Internal itd.)

  - **Data\_FailureReason:long –** unaprijed definiran skup vrijednosti razloga neuspjeha (FileIsCorrupt, BlockedByAntivirus itd.)

  - **Data\_fLifeguarded:bool –** je li dokument ikad popravljen pomoću značajke lifeguard (značajka za popravljanje pogrešaka dokumenta bez slanja upita korisniku)?

  - **Data\_HandleEnsureContentType:long –** vrijeme potrebno da bi se osiguralo da su sve vrste sadržaja ispravne

  - **Data\_HandleEnsureContentTypeTimeMS:long –** vrijeme potrebno da bi se osiguralo da su sve vrste sadržaja ispravne

  - **Data\_HasEmbeddedFont:bool –** ima li ovaj dokument ugrađene fontove?

  - **Data\_InitializeSaveTimeMS:long –** vrijeme potrebno za pokretanje spremanja sadržaja dokumenta

  - **Data\_InOCSTransition:bool –** izvršava li se ovo spremanje za prijelaz na OCS

  - **Data\_IsSavingWithEmbeddedFont:bool –** ima li ovaj dokument ugrađene fontove?

  - **Data\_MethodId:long –** koji je redak koda interno zadnji izvršen

  - **Data\_PerformEmbedFontsTimeMS:long –** vrijeme potrebno za serijaliziranje ugrađenih fontova

  - **Data\_PerformModernSaveTimeMS:long –** vrijeme potrebno za izvođenje modernog spremanja (novi kod)

  - **Data\_PerformPostSaveTimeMS:long –** vrijeme potrebno za izvođenje funkcija nakon spremanja (obavijesti, poništavanje unosa)

  - **Data\_PrepareForSaveTimeMS:long –** vrijeme potrebno za pokretanje spremanja

  - **Data\_RaiseDocumentBeforeSaveEventTimeMS:long –** vrijeme potrebno za podizanje događaja BeforeSave

  - **Data\_ReflectDocumentChangeTimeMS:long –** vrijeme potrebno za odražavanje spremljenih promjena u korisničko sučelje (ponovno popunjavanje minijatura itd.)

  - **Data\_ReportStartTimeMS:long –** vrijeme potrebno da bi se dovršilo pokretanje telemetrije za spremanje

  - **Data\_ReportSuccessTimeMS:long –** vrijeme potrebno da bi se dovršilo izvješćivanje o uspješnom spremanju

  - **Data\_ResetDirtyFlagOnErrorTimeMS:long –** vrijeme potrebno za ponovno postavljanje zastavice o pogrešci prljavog dokumenta

  - **Data\_SaveReason:long –** unaprijed definirani skup vrijednosti koji označava zašto je izvršeno spremanje? (AutoSave, ToOCSTransitionSave, ToCSITransitionSave itd.)

  - **Data\_SaveType:long –** unaprijed definirani skup vrijednosti o vrsti spremanja (SaveAs, Publish, Manual, OMSave itd.)

  - **Data\_SavingWithFont:bool–** spremamo li dokument s novim ugrađenim fontovima?

  - **Data\_ScrubClonedDocumentTimeMS:long –** vrijeme potrebno za uklanjanje osobnih podataka na kloniranoj kopiji dokumenta

  - **Data\_StopwatchDuration:long –** ukupno vrijeme za aktivnost

  - **Data\_TransactionType:long –** je li transakcija Spremi ili Spoji i spremi?

#### <a name="officepowerpointdocoperationsaveas"></a>Office.PowerPoint.DocOperation.SaveAs

Prikuplja se svaki put kada PowerPoint izvodi Spremi u obliku. Obuhvaća vrstu rezultata uspješno ili neuspješno metrike performansi spremanja i relevantnih metapodataka dokumenta. Problemi sa spremanjem mogu uzrokovati gubitak podataka.  Microsoft koristi te podatke da bi osigurao da značajka funkcionira prema očekivanjima i da se korisnički sadržaj uspješno održava.

Prikupljaju se sljedeća polja:

- **Data_AddDocTelemetryResult:long** – ima li ovaj unos u zapisnik svu potrebnu telemetriju dokumenta (polja Data_Doc_*)? Ako ne, zašto?

- **Data_CppUncaughtExceptionCount:long** – neuhvaćene lokalne iznimke dok se aktivnost izvršavala

- **Data_DetachedDuration:long** – vrijeme tijekom kojeg je aktivnost bila odvojena ili se nije izvršavala

- **Data_DstDoc_AccessMode:long** – kako je dokument otvoren (samo za čitanje | čitanje i pisanje)

- **Data_DstDoc_AssistedReadingReasons:long** – unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

- **Data_DstDoc_AsyncOpenKind:long –** označava je li otvorena predmemorirana verzija dokumenta u novom oblaku i koja je logika za asinkrono osvježavanje korištena.

- **Data_DstDoc_ChunkingType:long** – kako je dokument pohranjen u sustavu SharePoint

- **Data_DstDoc_EdpState:long** – stanje dokumenta s obzirom na zaštitu korporativnih podataka

- **Data_DstDoc_Ext:string** – nastavak dokumenta

- **Data_DstDoc_Extension:string** – nastavak dokumenta

- **Data_DstDoc_FileFormat:long** – unaprijed definirani skup vrijednosti oblika datoteke (precizniji od nastavka)

- **Data_DstDoc_Fqdn:string** – mjesto pohrane dokumenta (SharePoint.com, live.net), dostupno samo za domene sustava Office 365
    
- **Data_DstDoc_FqdnHash:string** – raspršivanje mjesta pohrane dokumenta

- **Data_DstDoc_IdentityTelemetryId:string** – jedinstveni GUID korisnika

- **Data_DstDoc_IdentityUniqueId:string** – jedinstveni identifikator identiteta korišten za akciju zajedničkih dokumenata

- **Data_DstDoc_IOFlags:long** – bit-maska za razne zastavice vezane uz ulaz i izlaz za određeni dokument

- **Data_DstDoc_IrmRights:long** – unaprijed definirani skup vrijednosti za vrstu informacija koju upravljanje pravima primjenjuje na ovom dokumentu (proslijedi, odgovori, SecureReader, uređivanje itd.)
    
- **Data_DstDoc_IsCloudCollabEnabled:bool** – istinito ako je HTTP zaglavlje „IsCloudCollabEnabled” već prihvaćeno iz zahtjeva MOGUĆNOSTI.

- **Data_DstDoc_IsIncrementalOpen:bool** – je li dokument otvoren inkrementalno (nova značajka koja otvara dokument bez potrebe za preuzimanjem cijelog dokumenta)

- **Data_DstDoc_IsOcsSupported:bool** – podržava li dokument suautorstvo pomoću novog servisa OCS

- **Data_DstDoc_IsOpeningOfflineCopy:bool** – provjerava otvara li se dokument iz lokalne predmemorije

- **Data_DstDoc_IsSyncBacked:bool** – otvara li se dokument iz mape koja koristi aplikaciju OneDrive za povratnu sinkronizaciju
    
- **Data_DstDoc_Location:long** – unaprijed definiran skup vrijednosti mjesta na kojima se dokument pohranjuje (lokalno, SharePoint, WOPI, mreža itd.)

- **Data_DstDoc_LocationDetails:long** – unaprijed definiran skup vrijednosti detaljnijih lokacija (mapa Temp, mapa preuzimanja, dokumenti servisa One Drive, slike servisa One Drive itd.)

- **Data_DstDoc_NumberCoAuthors:long** – broj suautora prilikom otvaranja dokumenta

- **Data_DstDoc_PasswordFlags:long** – unaprijed definirani skup vrijednosti načina na koji je dokument šifriran pomoću lozinke (nema, lozinka za čitanje, lozinka za uređivanje)

- **Data_DstDoc_ReadOnlyReasons:long** – unaprijed definirani skup vrijednosti koji naznačuje zašto je dokument označen samo za čitanje (zaključan na poslužitelju, konačni dokument, zaštićen lozinkom za uređivanje itd.)

- **Data_DstDoc_ResourceIdHash:string** – raspršivanje identifikatora resursa za dokumente pohranjene u oblaku

- **Data_DstDoc_ServerDocId:string** – nepromjenjivi identifikator za dokumente pohranjene u oblaku

- **Data_DstDoc_ServerProtocol:long** – unaprijed definirani skup vrijednosti o protokolu koji se koristi za komuniciranje s poslužiteljem (Http, Cobalt, WOPI itd.)

- **Data_DstDoc_ServerType:long** – unaprijed definirani skup vrijednosti o vrsti poslužitelja (SharePoint, DropBox, WOPI)

- **Data_DstDoc_ServerVersion:long** – provjerava temelji li se poslužitelj na sustavu Office14, Office15 ili Office 16

- **Data_DstDoc_SessionId:long** – generirani GUID koji identificira instancu dokumenta u sklopu iste sesije procesa

- **Data_DstDoc_SharePointServiceContext:string** – neprozirni niz, obično GridManagerID.FarmID. Korisno za korelaciju klijentskih i poslužiteljskih zapisnika

- **Data_DstDoc_SizeInBytes:long** – veličina dokumenta u bajtovima

- **Data_DstDoc_SpecialChars:long** – bit-maska koja pokazuje posebne znakove u URL-u ili putu dokumenta

- **Data_DstDoc_StorageProviderId:string** – niz koji određuje davatelja pohrane dokumenta, primjerice „DropBox”

- **Data_DstDoc_StreamAvailability:long** – unaprijed definirani skup vrijednosti statusa toka dokumenta (dostupno, trajno onemogućeno, nije dostupno)

- **Data_DstDoc_UrlHash:string** – raspršivanje punog URL-a dokumenata pohranjenih u oblaku

- **Data_DstDoc_UsedWrsDataOnOpen:bool** – istinito ako je datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka na glavnom računalu

- **Data_DstDoc_WopiServiceId:string** – identifikator WOPI servisa, npr. „Dropbox”

- **Data_FileType:long** – unaprijed definirani skup vrijednosti interne vrste datoteke

- **Data_fLifeguarded:bool** – je li dokument ikad popravljen pomoću značajke lifeguard (značajka za popravljanje pogrešaka dokumenta bez slanja upita korisniku)?

- **Data_FWebCreated:bool** – ima li ovaj dokument zastavicu WebCreator?

- **Data_SaveReason:long** – unaprijed definirani skup vrijednosti koji označava zašto je izvršeno spremanje? (AutoSave, ToOCSTransitionSave, ToCSITransitionSave itd.)

- **Data_SaveType:long** – unaprijed definirani skup vrijednosti o vrsti spremanja (SaveAs, Publish, Manual, OMSave itd.) 

- **Data_SrcDoc_AccessMode:long** – kako je dokument otvoren (samo za čitanje | čitanje i pisanje)

- **Data_SrcDoc_AssistedReadingReasons:long** – unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

- **Data_SrcDoc_AsyncOpenKind:long –** označava je li otvorena predmemorirana verzija dokumenta u izvornom oblaku i koja je logika za asinkrono osvježavanje korištena.

- **Data_SrcDoc_ChunkingType:long** – kako je dokument pohranjen u sustavu SharePoint 

- **Data_SrcDoc_EdpState:long** – stanje dokumenta s obzirom na zaštitu korporativnih podataka

- **Data_SrcDoc_Ext:string** – nastavak dokumenta

- **Data_SrcDoc_Extension:string** – nastavak dokumenta

- **Data_SrcDoc_FileFormat:long** – unaprijed definirani skup vrijednosti oblika datoteke (precizniji od nastavka)

- **Data_SrcDoc_Fqdn:string** – mjesto pohrane dokumenta (SharePoint.com, live.net), dostupno samo za domene sustava Office 365

- **Data_SrcDoc_FqdnHash:string** – raspršivanje mjesta pohrane dokumenta

- **Data_SrcDoc_IdentityTelemetryId:string** – jedinstveni GUID korisnika

- **Data_SrcDoc_IdentityUniqueId:string** – jedinstveni identifikator identiteta korišten za akciju zajedničkih dokumenata

- **Data_SrcDoc_IOFlags:long** – bit-maska za razne zastavice vezane uz ulaz i izlaz za određeni dokument

- **Data_SrcDoc_IrmRights:long** – unaprijed definirani skup vrijednosti za vrstu informacija koju upravljanje pravima primjenjuje na ovom dokumentu (proslijedi, odgovori, SecureReader, uređivanje itd.)

- **Data_SrcDoc_IsCloudCollabEnabled:bool** – istinito ako je HTTP zaglavlje „IsCloudCollabEnabled” već prihvaćeno iz zahtjeva MOGUĆNOSTI.

- **Data_SrcDoc_IsIncrementalOpen:bool** – je li dokument otvoren inkrementalno (nova značajka koja otvara dokument bez potrebe za preuzimanjem cijelog dokumenta)

- **Data_SrcDoc_IsOcsSupported:bool** – podržava li dokument suautorstvo pomoću novog servisa OCS

- **Data_SrcDoc_IsOpeningOfflineCopy:bool** – provjerava otvara li se dokument iz lokalne predmemorije

- **Data_SrcDoc_IsSyncBacked:bool** – otvara li se dokument iz mape koja koristi aplikaciju OneDrive za povratnu sinkronizaciju

- **Data_SrcDoc_Location:long** – unaprijed definiran skup vrijednosti mjesta na kojima se dokument pohranjuje (lokalno, SharePoint, WOPI, mreža itd.)

- **Data_SrcDoc_LocationDetails:long** – unaprijed definiran skup vrijednosti detaljnijih lokacija (mapa Temp, mapa preuzimanja, dokumenti servisa One Drive, slike servisa One Drive itd.)

- **Data_SrcDoc_NumberCoAuthors:long** – broj suautora prilikom otvaranja dokumenta

- **Data_SrcDoc_PasswordFlags:long** – unaprijed definirani skup vrijednosti načina na koji je dokument šifriran pomoću lozinke (nema, lozinka za čitanje, lozinka za uređivanje)

- **Data_SrcDoc_ReadOnlyReasons:long** – unaprijed definirani skup vrijednosti koji naznačuje zašto je dokument označen samo za čitanje (zaključan na poslužitelju, konačni dokument, zaštićen lozinkom za uređivanje itd.)

- **Data_SrcDoc_ResourceIdHash:string** – raspršivanje identifikatora resursa za dokumente pohranjene u oblaku

- **Data_SrcDoc_ServerDocId:string** – nepromjenjivi identifikator za dokumente pohranjene u oblaku

- **Data_SrcDoc_ServerProtocol:long** – unaprijed definirani skup vrijednosti o protokolu koji se koristi za komuniciranje s poslužiteljem (Http, Cobalt, WOPI itd.)

- **Data_SrcDoc_ServerType:long** – unaprijed definirani skup vrijednosti o vrsti poslužitelja (SharePoint, DropBox, WOPI)

- **Data_SrcDoc_ServerVersion:long** – provjerava temelji li se poslužitelj na sustavu Office14, Office15 ili Office 16

- **Data_SrcDoc_SessionId:long** – generirani GUID koji označava instancu dokumenta u sklopu iste sesije procesa

- **Data_SrcDoc_SharePointServiceContext:string** – neprozirni niz, obično GridManagerID.FarmID. Korisno za korelaciju klijentskih i poslužiteljskih zapisnika

- **Data_SrcDoc_SizeInBytes:long** – veličina dokumenta u bajtovima

- **Data_SrcDoc_SpecialChars:long** – bit-maska koja pokazuje posebne znakove u URL-u ili putu dokumenta

- **Data_SrcDoc_StorageProviderId:string** – niz koji određuje davatelja pohrane dokumenta, primjerice „DropBox”

- **Data_SrcDoc_StreamAvailability:long** – unaprijed definirani skup vrijednosti statusa toka dokumenta (dostupno, trajno onemogućeno, nije dostupno)

- **Data_SrcDoc_UrlHash:string** – raspršivanje punog URL-a dokumenata pohranjenih u oblaku

- **Data_SrcDoc_UsedWrsDataOnOpen:bool** – istinito ako je datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka na glavnom računalu

- **Data_SrcDoc_WopiServiceId:string** – identifikator WOPI servisa, npr. „Dropbox”

- **Data_StopwatchDuration:long** – ukupno vrijeme za aktivnost

- **Data_TypeOfSaveDialog:long** – unaprijed definirani skup vrijednosti dijaloškog okvira (RUN_SAVEAS_DLG,RUN_SAVEMEDIA_DLG, RUN_SAVEAS_VIDEO_DLG itd.)

- **Data_WaitForSaveOrMergeSuccess: bool** – SaveAs je uspio nakon čekanja na spremanje ili spajanje u pozadini.
 
- **Data_WaitForSaveOrMergeTimeout: long** – isteklo je vrijeme čekanja na SaveAs za vrijeme čekanja na spremanje ili spajanje u pozadini.

- **DstDoc** – nova lokacija dokumenta 

- **SrcDoc** – izvorna lokacija dokumenta


#### <a name="officepowerpointdocoperationsavelegacy"></a>Office.PowerPoint.DocOperation.SaveLegacy

Prikuplja se svaki put kada PowerPoint izvodi spremanje pomoću naslijeđenog puta koda. Obuhvaća vrstu rezultata uspješno ili neuspješno metrike performansi spremanja i relevantnih metapodataka dokumenta.  Problemi sa spremanjem mogu uzrokovati gubitak podataka.  Microsoft koristi te podatke da bi osigurao da značajka funkcionira prema očekivanjima i da se korisnički sadržaj uspješno održava.

Prikupljaju se sljedeća polja:

- **Data_AddDocTelemetryResult:long** – ima li ovaj unos u zapisnik svu potrebnu telemetriju dokumenta (polja Data_Doc_*)? Ako ne, zašto?

- **Data_CppUncaughtExceptionCount:long** – neuhvaćene lokalne iznimke dok se aktivnost izvršavala

- **Data_DetachedDuration:long** – vrijeme tijekom kojeg je aktivnost bila odvojena ili se nije izvršavala

- **Data_Doc_AccessMode:long** – kako je dokument otvoren (samo za čitanje | čitanje i pisanje)

- **Data_Doc_AssistedReadingReasons:long** – unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

- **Data_Doc_AsyncOpenKind:long –** označava je li otvorena predmemorirana verzija dokumenta u oblaku i koja je logika za asinkrono osvježavanje korištena.

- **Data_Doc_ChunkingType:long** – kako je dokument pohranjen u sustavu SharePoint

- **Data_Doc_EdpState:long** – stanje dokumenta s obzirom na zaštitu korporativnih podataka

- **Data_Doc_Ext:string** – nastavak dokumenta

- **Data_Doc_Extension:string** – nastavak dokumenta

- **Data_Doc_FileFormat:long** – unaprijed definirani skup vrijednosti oblika datoteke (precizniji od nastavka)

- **Data_Doc_Fqdn:string** – mjesto pohrane dokumenta (SharePoint.com, live.net), dostupno samo za domene sustava Office 365

- **Data_Doc_FqdnHash:string** – raspršivanje mjesta pohrane dokumenta

- **Data_Doc_IdentityTelemetryId:string** – jedinstveni GUID korisnika

- **Data_Doc_IdentityUniqueId:string** – jedinstveni identifikator identiteta korišten za akciju zajedničkih dokumenata

- **Data_Doc_IOFlags:long** – bit-maska za razne zastavice vezane uz ulaz i izlaz za određeni dokument

- **Data_Doc_IrmRights:long** – unaprijed definirani skup vrijednosti za vrstu informacija koju upravljanje pravima primjenjuje na ovom dokumentu (proslijedi, odgovori, SecureReader, uređivanje itd.)

- **Data_Doc_IsCloudCollabEnabled:bool** – istinito ako je HTTP zaglavlje „IsCloudCollabEnabled” već prihvaćeno iz zahtjeva MOGUĆNOSTI.

- **Data_Doc_IsIncrementalOpen:bool** – je li dokument otvoren inkrementalno (nova značajka koja otvara dokument bez potrebe za preuzimanjem cijelog dokumenta)

- **Data_Doc_IsOcsSupported:bool** – podržava li dokument suautorstvo pomoću novog servisa OCS

- **Data_Doc_IsOpeningOfflineCopy:bool** – provjerava otvara li se dokument iz lokalne predmemorije

- **Data_Doc_IsSyncBacked:bool** – otvara li se dokument iz mape koja koristi aplikaciju OneDrive za povratnu sinkronizaciju

- **Data_Doc_Location:long** – unaprijed definiran skup vrijednosti mjesta na kojima se dokument pohranjuje (lokalno, SharePoint, WOPI, mreža itd.)

- **Data_Doc_LocationDetails:long** – unaprijed definiran skup vrijednosti detaljnijih lokacija (mapa Temp, mapa preuzimanja, dokumenti servisa One Drive, slike servisa One Drive itd.)

- **Data_Doc_NumberCoAuthors:long** – broj suautora prilikom otvaranja dokumenta

- **Data_Doc_PasswordFlags:long** – unaprijed definirani skup vrijednosti načina na koji je dokument šifriran pomoću lozinke (nema, lozinka za čitanje, lozinka za uređivanje)

- **Data_Doc_ReadOnlyReasons:long** – unaprijed definirani skup vrijednosti koji naznačuje zašto je dokument označen samo za čitanje (zaključan na poslužitelju, konačni dokument, zaštićen lozinkom za uređivanje itd.)

- **Data_Doc_ResourceIdHash:string** – raspršivanje identifikatora resursa za dokumente pohranjene u oblaku

- **Data_Doc_RtcType** – označava kako je postavljen kanal u stvarnom vremenu (RTC) za trenutnu datoteku (Onemogućeno, nepodržano, na zahtjev, uvijek uključeno itd.).

- **Data_Doc_ServerDocId:string** – nepromjenjivi identifikator za dokumente pohranjene u oblaku

- **Data_Doc_ServerProtocol:long** – unaprijed definirani skup vrijednosti o protokolu koji se koristi za komuniciranje s poslužiteljem (Http, Cobalt, WOPI itd.)

- **Data_Doc_ServerType:long** – unaprijed definirani skup vrijednosti o vrsti poslužitelja (SharePoint, DropBox, WOPI) 

- **Data_Doc_ServerVersion:long** – provjerava temelji li se poslužitelj na sustavu Office14, Office15 ili Office 16

- **Data_Doc_SessionId:long** – generirani GUID koji identificira instancu dokumenta u sklopu iste sesije procesa

- **Data_Doc_SharePointServiceContext:string** – neprozirni niz, obično GridManagerID.FarmID. Korisno za korelaciju klijentskih i poslužiteljskih zapisnika

- **Data_Doc_SizeInBytes:long** – veličina dokumenta u bajtovima

- **Data_Doc_SpecialChars:long** – bit-maska koja pokazuje posebne znakove u URL-u ili putu dokumenta

- **Data_Doc_StorageProviderId:string** – niz koji određuje davatelja pohrane dokumenta, primjerice „DropBox”

- **Data_Doc_StreamAvailability:long** – unaprijed definirani skup vrijednosti statusa toka dokumenta (dostupno, trajno onemogućeno, nije dostupno)

- **Data_Doc_UrlHash:string** – raspršivanje punog URL-a dokumenata pohranjenih u oblaku

- **Data_Doc_UsedWrsDataOnOpen:bool** – istinito ako je datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka na glavnom računalu

- **Data_Doc_WopiServiceId:string** – identifikator WOPI servisa, na primjer, „Dropbox”

- **Data_DstDoc_AccessMode:long** – kako je dokument otvoren (samo za čitanje | čitanje i pisanje)

- **Data_DstDoc_AssistedReadingReasons:long** – unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

- **Data_DstDoc_AsyncOpenKind:long –** označava je li otvorena predmemorirana verzija dokumenta u novom oblaku i koja je logika za asinkrono osvježavanje korištena.

- **Data_DstDoc_ChunkingType:long** – kako je dokument pohranjen u sustavu SharePoint

- **Data_DstDoc_EdpState:long** – stanje dokumenta s obzirom na zaštitu korporativnih podataka

- **Data_DstDoc_Ext:string** – nastavak dokumenta

- **Data_DstDoc_Extension:string** – nastavak dokumenta

- **Data_DstDoc_FileFormat:long** – unaprijed definirani skup vrijednosti oblika datoteke (precizniji od nastavka)

- **Data_DstDoc_Fqdn:string** – mjesto pohrane dokumenta (SharePoint.com, live.net), dostupno samo za domene sustava Office 365
    
- **Data_DstDoc_FqdnHash:string** – raspršivanje mjesta pohrane dokumenta

- **Data_DstDoc_IdentityTelemetryId:string** – jedinstveni GUID korisnika

- **Data_DstDoc_IdentityUniqueId:string** – jedinstveni identifikator identiteta korišten za akciju zajedničkih dokumenata

- **Data_DstDoc_IOFlags:long** – bit-maska za razne zastavice vezane uz ulaz i izlaz za određeni dokument

- **Data_DstDoc_IrmRights:long** – unaprijed definirani skup vrijednosti za vrstu informacija koju upravljanje pravima primjenjuje na ovom dokumentu (proslijedi, odgovori, SecureReader, uređivanje itd.)

- **Data_DstDoc_IsCloudCollabEnabled:bool** – istinito ako je HTTP zaglavlje „IsCloudCollabEnabled” već prihvaćeno iz zahtjeva MOGUĆNOSTI.

- **Data_DstDoc_IsIncrementalOpen:bool** – je li dokument otvoren inkrementalno (nova značajka koja otvara dokument bez potrebe za preuzimanjem cijelog dokumenta)

- **Data_DstDoc_IsOcsSupported:bool** – podržava li dokument suautorstvo pomoću novog servisa OCS

- **Data_DstDoc_IsOpeningOfflineCopy:bool** – provjerava otvara li se dokument iz lokalne predmemorije

- **Data_DstDoc_IsSyncBacked:bool** – otvara li se dokument iz mape koja koristi aplikaciju OneDrive za povratnu sinkronizaciju

- **Data_DstDoc_Location:long** – unaprijed definiran skup vrijednosti mjesta na kojima se dokument pohranjuje (lokalno, SharePoint, WOPI, mreža itd.)

- **Data_DstDoc_LocationDetails:long** – unaprijed definiran skup vrijednosti detaljnijih lokacija (mapa Temp, mapa preuzimanja, dokumenti servisa One Drive, slike servisa One Drive itd.)

- **Data_DstDoc_NumberCoAuthors:long** – broj suautora prilikom otvaranja dokumenta

- **Data_DstDoc_PasswordFlags:long** – unaprijed definirani skup vrijednosti načina na koji je dokument šifriran pomoću lozinke (nema, lozinka za čitanje, lozinka za uređivanje)

- **Data_DstDoc_ReadOnlyReasons:long** – unaprijed definirani skup vrijednosti koji naznačuje zašto je dokument označen samo za čitanje (zaključan na poslužitelju, konačni dokument, zaštićen lozinkom za uređivanje itd.)

- **Data_DstDoc_ResourceIdHash:string** – raspršivanje identifikatora resursa za dokumente pohranjene u oblaku

- **Data_DstDoc_ServerDocId:string** – nepromjenjivi identifikator za dokumente pohranjene u oblaku

- **Data_DstDoc_ServerProtocol:long** – unaprijed definirani skup vrijednosti o protokolu koji se koristi za komuniciranje s poslužiteljem (Http, Cobalt, WOPI itd.)

- **Data_DstDoc_ServerType:long** – unaprijed definirani skup vrijednosti o vrsti poslužitelja (SharePoint, DropBox, WOPI)

- **Data_DstDoc_ServerVersion:long** – provjerava temelji li se poslužitelj na sustavu Office14, Office15 ili Office 16

- **Data_DstDoc_SessionId:long** – generirani GUID koji identificira instancu dokumenta u sklopu iste sesije procesa

- **Data_DstDoc_SharePointServiceContext:string** – neprozirni niz, obično GridManagerID.FarmID. Korisno za korelaciju klijentskih i poslužiteljskih zapisnika

- **Data_DstDoc_SizeInBytes:long** – veličina dokumenta u bajtovima

- **Data_DstDoc_SpecialChars:long** – bit-maska koja pokazuje posebne znakove u URL-u ili putu dokumenta

- **Data_DstDoc_StorageProviderId:string** – niz koji određuje davatelja pohrane dokumenta, primjerice „DropBox”

- **Data_DstDoc_StreamAvailability:long** – unaprijed definirani skup vrijednosti statusa toka dokumenta (dostupno, trajno onemogućeno, nije dostupno)

- **Data_DstDoc_UrlHash:string** – raspršivanje punog URL-a dokumenata pohranjenih u oblaku

- **Data_DstDoc_UsedWrsDataOnOpen:bool** – istinito ako je datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka na glavnom računalu

- **Data_DstDoc_WopiServiceId:string** – identifikator WOPI servisa, npr. „Dropbox”

- **Data_FileType:long** – unaprijed definirani skup vrijednosti interne vrste datoteke

- **Data_fLifeguarded:bool** – je li dokument ikad popravljen pomoću značajke lifeguard (značajka za popravljanje pogrešaka dokumenta bez slanja upita korisniku)?

- **Data_SaveReason:long** – unaprijed definirani skup vrijednosti koji označava zašto je izvršeno spremanje? (AutoSave, ToOCSTransitionSave, ToCSITransitionSave itd.)

- **Data_SaveType:long** – unaprijed definirani skup vrijednosti o vrsti spremanja (SaveAs, Publish, Manual, OMSave itd.)

- **Data_SrcDoc_AccessMode:long** – kako je dokument otvoren (samo za čitanje | čitanje i pisanje)

- **Data_SrcDoc_AssistedReadingReasons:long** – unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

- **Data_SrcDoc_AsyncOpenKind:long –** označava je li otvorena predmemorirana verzija dokumenta u izvornom oblaku i koja je logika za asinkrono osvježavanje korištena.

- **Data_SrcDoc_ChunkingType:long** – kako je dokument pohranjen u sustavu SharePoint

- **Data_SrcDoc_EdpState:long** – stanje dokumenta s obzirom na zaštitu korporativnih podataka

- **Data_SrcDoc_Ext:string** – nastavak dokumenta

- **Data_SrcDoc_Extension:string** – nastavak dokumenta

- **Data_SrcDoc_FileFormat:long** – unaprijed definirani skup vrijednosti oblika datoteke (precizniji od nastavka)

- **Data_SrcDoc_Fqdn:string** – mjesto pohrane dokumenta (SharePoint.com, live.net), dostupno samo za domene sustava Office 365

- **Data_SrcDoc_FqdnHash:string** – raspršivanje mjesta pohrane dokumenta 

- **Data_SrcDoc_IdentityTelemetryId:string** – jedinstveni GUID korisnika

- **Data_SrcDoc_IdentityUniqueId:string** – jedinstveni identifikator identiteta korišten za akciju zajedničkih dokumenata

- **Data_SrcDoc_IOFlags:long** – bit-maska za razne zastavice vezane uz ulaz i izlaz za određeni dokument

- **Data_SrcDoc_IrmRights:long** – unaprijed definirani skup vrijednosti za vrstu informacija koju upravljanje pravima primjenjuje na ovom dokumentu (proslijedi, odgovori, SecureReader, uređivanje itd.)
    
- **Data_SrcDoc_IsCloudCollabEnabled:bool** – istinito ako je HTTP zaglavlje „IsCloudCollabEnabled” već prihvaćeno iz zahtjeva MOGUĆNOSTI.

- **Data_SrcDoc_IsIncrementalOpen:bool** – je li dokument otvoren inkrementalno (nova značajka koja otvara dokument bez potrebe za preuzimanjem cijelog dokumenta)

- **Data_SrcDoc_IsOcsSupported:bool** – podržava li dokument suautorstvo pomoću novog servisa OCS

- **Data_SrcDoc_IsOpeningOfflineCopy:bool** – provjerava otvara li se dokument iz lokalne predmemorije

- **Data_SrcDoc_IsSyncBacked:bool** – otvara li se dokument iz mape koja koristi aplikaciju OneDrive za povratnu sinkronizaciju

- **Data_SrcDoc_Location:long** – unaprijed definiran skup vrijednosti mjesta na kojima se dokument pohranjuje (lokalno, SharePoint, WOPI, mreža itd.)

- **Data_SrcDoc_LocationDetails:long** – unaprijed definiran skup vrijednosti detaljnijih lokacija (mapa Temp, mapa preuzimanja, dokumenti servisa One Drive, slike servisa One Drive itd.)

- **Data_SrcDoc_NumberCoAuthors:long** – broj suautora prilikom otvaranja dokumenta

- **Data_SrcDoc_PasswordFlags:long** – unaprijed definirani skup vrijednosti načina na koji je dokument šifriran pomoću lozinke (nema, lozinka za čitanje, lozinka za uređivanje)

- **Data_SrcDoc_ReadOnlyReasons:long** – unaprijed definirani skup vrijednosti koji naznačuje zašto je dokument označen samo za čitanje (zaključan na poslužitelju, konačni dokument, zaštićen lozinkom za uređivanje itd.)

- **Data_SrcDoc_ResourceIdHash:string** – raspršivanje identifikatora resursa za dokumente pohranjene u oblaku

- **Data_SrcDoc_ServerDocId:string** – nepromjenjivi identifikator za dokumente pohranjene u oblaku

- **Data_SrcDoc_ServerProtocol:long** – unaprijed definirani skup vrijednosti o protokolu koji se koristi za komuniciranje s poslužiteljem (Http, Cobalt, WOPI itd.)

- **Data_SrcDoc_ServerType:long** – unaprijed definirani skup vrijednosti o vrsti poslužitelja (SharePoint, DropBox, WOPI)

- **Data_SrcDoc_ServerVersion:long** – provjerava temelji li se poslužitelj na sustavu Office14, Office15 ili Office 16

- **Data_SrcDoc_SessionId:long** – generirani GUID koji identificira instancu dokumenta u sklopu iste sesije procesa

- **Data_SrcDoc_SharePointServiceContext:string** – neprozirni niz, obično GridManagerID.FarmID. Korisno za korelaciju klijentskih i poslužiteljskih zapisnika

- **Data_SrcDoc_SizeInBytes:long** – veličina dokumenta u bajtovima

- **Data_SrcDoc_SpecialChars:long** – bit-maska koja pokazuje posebne znakove u URL-u ili putu dokumenta

- **Data_SrcDoc_StorageProviderId:string** – niz koji određuje davatelja pohrane dokumenta, primjerice „DropBox”

- **Data_SrcDoc_StreamAvailability:long** – unaprijed definirani skup vrijednosti statusa toka dokumenta (dostupno, trajno onemogućeno, nije dostupno)

- **Data_SrcDoc_UrlHash:string** – raspršivanje punog URL-a dokumenata pohranjenih u oblaku

- **Data_SrcDoc_UsedWrsDataOnOpen:bool** – istinito ako je datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka na glavnom računalu

- **Data_SrcDoc_WopiServiceId:string** – identifikator WOPI servisa, npr. „Dropbox”

- **Data_StopwatchDuration:long** – ukupno vrijeme za aktivnost

- **Data_TypeOfSaveDialog:long** – unaprijed definirani skup vrijednosti dijaloškog okvira (RUN_SAVEAS_DLG, RUN_SAVEMEDIA_DLG, RUN_SAVEAS_VIDEO_DLG itd.)

- **Doc** – trenutni dokument za spremanje

- **DstDoc** – nova lokacija dokumenta (u slučaju SaveAs)

- **SrcDoc** – izvorna lokacija dokumenta (u slučaju SaveAs)


#### <a name="officepowerpointpptiosrehearseview"></a>Office.PowerPoint.PPT.IOS.RehearseView 

Ovaj događaj označava da je korisnik prekinuo sesiju probe. Podaci se koriste u kombinaciji s Office.PowerPoint.PPT.Android.RehearseView.StartSession kao prvi indikator bilo kojeg zaustavljanja ili pogreški s kojima se korisnik suočava.  
 
Prikupljaju se sljedeća polja:

- **ConnectionCreationTime** – vrijeme potrebno za stvaranje veza na strani poslužitelja.

- **CountDownAlertTime** – vrijeme za koje je prikazano upozorenje za odbrojavanje.

- **CountdownInitTime –** vrijeme između dovršetka učitavanja dijaprojekcije i početka odbrojavanja.

- **CritiqueSummary** – sažetak onoga što će svi korisnici-kritičari vidjeti na svojim brojačima.

- **ExitEventCode** – kôd za prepoznavanje u kojem scenariju korisnik izlazi iz sesije vježbanja, bez obzira na to je li riječ o scenariju pogreške ili uspješnom izlazu.

- **FRETime** – Vrijeme između početka prikazivanja zaslona s početnim sučeljem i vremena dok ga korisnik nije odbacio.

- **MikrophonePermissionTime** – vrijeme tijekom kojeg je prikazano upozorenje o dozvolama mikrofona dok korisnik ne odabere jednu od mogućnosti.

- **PauseRehearsingCount** – koliko je puta korisnik kliknuo na pauziranje probe

- **RehearsalInitTime** vrijeme koje je probi bilo potrebno da se pokrene

- **ResumeRehearsingCount** – koliko je puta korisnik kliknuo na nastavak probe.

- **Sessionid** – to je ID sjednice govornog ulaza.  Koristi se za ispravljanje pogrešaka u zapisnicima servisa.

- **SlideshowViewLoadTime** – vrijeme učitavanja dijaprojekcije.


#### <a name="officepowerpointpptiosrehearseviewrehearsalsummarypage"></a>Office.PowerPoint.PPT.IOS.RehearseView.RehearsalSummaryPage

Događaj se aktivira kada stranica sažetka dovrši učitavanje. Taj nam događaj pomaže pri snimanju izvedbe stranice sažetka. Govori nam koliko je vremena potrebno da se stranica usluge sažetka probe učita na klijenta. Potrebno je održavati performanse značajke.  

Prikupljaju se sljedeća polja: 

- **PayloadCreationTime** – vrijeme koje je potrebno u milisekundama za stvaranje opterećenja.  

- **PostUrlCallTime** – vrijeme koje je potrebno u milisekundama za slanje naknadnog URL poziva. 

- **RehearseSessionId** – to je ID sesije ulaznih vrata govora. Može se koristiti za ispravljanje pogrešaka u zapisnicima servisa.  

- **SummaryPageErrorReceived** – to je Booleova vrijednost koja pokazuje je li primljena stranica sažetka ili je došlo do pogreške.

- **SummaryPageHtmlLoadTime** – to je vrijeme u milisekundama koje je potrebno za učitavanje summarypageHtml. 

- **SummaryPageLoadStartTime** – to je vrijeme u milisekundama za primanje prvog odgovora s poslužitelja. 

- **SummaryPageLoadTime** – Vrijeme potrebno za učitavanje stranice sažetka. To obuhvaća vrijeme stvaranja opterećenja. 

- **ThumbnailsCount** – to je ukupan broj minijatura koje će biti dio stranice sažetka. 


#### <a name="officepowerpointpptiosrehearseviewstartsession"></a>Office.PowerPoint.PPT.IOS.RehearseView.StartSession 
 
Događaj se aktivira kada korisnik klikne na početak sesije. Ovaj nam događaj pomaže utvrditi koliko korisnika koristi značajku Instruktor za izlaganje na uređaju sa sustavu iOS. U kombinaciji s Office.PowerPoint.PPT.iOS.RehearseView reći će nam koliko je korisnika uspješno dovršilo sesiju probe i koliko ih nije moglo to napraviti. To je naš prvi indikator rušenja ili pogrešaka u značajci.

Prikupljaju se sljedeća polja:

- Nijedno

#### <a name="officepowerpointpptmacshellprintinfo"></a>Office.PowerPoint.PPT.Mac.Shell.PrintInfo

Prikuplja se svaki put kada se dovrši radnja izvoza PDF-a te sadrži informacije o uspjehu radnje. Ove su informacije ključne za identifikaciju uspjeha radnji izvoza PDF-a u aplikaciji.

Prikupljaju se sljedeća polja:

- **Data_ExportAsPDFSucceed** – Booleova vrijednost koja označava je li izvoz u obliku PDF-a bio uspješan.

#### <a name="officepowerpointpptsharedrehearseviewrehearseclicked"></a>Office.PowerPoint.PPT.Shared.RehearseView.RehearseClicked

Taj događaj bilježi kada se pritisne RehearseWithCoach.   Taj se događaj koristi za analizu viđenog-pokušanog-zadržavanog lijevka značajke. Ovaj događaj zajedno s isprobanim i zadržanim događajem pomaže nam da shvatimo da li korisnici odustaju od lijevka. To nam pomaže održavati stanje značajke.

Prikupljaju se sljedeća polja:

- Nijedno


#### <a name="officepowerpointpptsharedslideshowfailure"></a>Office.PowerPoint.PPT.Shared.SlideShow.Failure

Prikupljanje neuspješnih pokušaja tijekom dijaprojekcije kao ključne značajke za PowerPoint. Microsoft prikuplja kada se poruka pojavljuje tijekom dijaprojekcije za poboljšanje korisničkog iskustva na dijaprojekciji. Microsoft koristi te podatke za dobivanje dijagnostičkih informacija o mjestu pojavljivanja pogreške dok korisnik koristi dijaprojekciju.

Prikupljaju se sljedeća polja:

- **CountOArtErrors** – ukupan broj OArt pogrešaka

- **CountOtherErrors** – ukupan broj drugih pogrešaka

- **CountPPTErrors** – ukupan broj PPT pogrešaka

- **CountSlideShowErrors** – ukupan broj pogrešaka dijaprojekcije

- **FirstOArtError** – prva pogreška dogodila se u OArt-u

- **FirstOtherError** – prva pogreška dogodila se u drugom području

- **FirstPPTError** – prva pogreška dogodila se u PPT-u

- **FirstSlideShowError** – prva pogreška dogodila se u dijaprojekciji

    
#### <a name="officepowerpointrunprintoperation"></a>Office.PowerPoint.RunPrintOperation

Prikuplja se svaki put kada se dovrši radnja ispisivanja PDF-a te sadrži informacije o vrsti izgleda, korištenju brojeva slajdova i uspjehu radnje. Ove su informacije ključne za identifikaciju uspjeha radnji ispisivanja PDF-a u aplikaciji.

Prikupljaju se sljedeća polja:

- **Data_PrintWithSlideNumbers** – Booleova vrijednost koja označava ispisuje li korisnik s brojevima slajdova.

- **Data_SavePrintLayoutType** – vrsta izgleda ispisa u trenutku početka postupka ispisivanja ili izvoza.

- **Data_Success** – Booleova vrijednost koja označava je li ispisivanje bilo uspješno.


#### <a name="officeprojectprojectfilesave"></a>Office.Project.ProjectFileSave

Project sprema datoteku. Taj događaj označava spremanje u programu Project. Omogućuje Microsoftu mjerenje uspjeha spremanja datoteke programa Project što je važno za sprječavanje gubitka podataka dokumenta.

Prikupljaju se sljedeća polja:

  - **Data\_TriggerTime** – vrijeme spremanja

  - **Data\_FileType** – vrsta datoteke u koju se sprema projekt
 
#### <a name="officesessionactivitystart"></a>Office.Session.Activity.Start

Omogućuje nam da znamo kada je pokrenuta sesija dodatka Data streamer.  Koristi se za stanje i nadzor značajke. Taj je događaj generirao dodatak Microsoft Data Streamer za Excel.

Prikupljaju se sljedeća polja:

- **Activity_Name** – naziv aktivnosti „Sesija”

- **Activity_CV** – ID za povezivanje događaja u sesiji povezivanja

- **Activity_StartStopType** – početak

- **Activity_DateTimeTicks** – vrijeme podataka za aktivnost

#### <a name="officesessionactivitystop"></a>Office.Session.Activity.Stop

Omogućuje nam da znamo kada je sesija dodatka Data streamer zaustavljena. Koristi se za stanje i nadzor značajke. Taj je događaj generirao dodatak Microsoft Data Streamer za Excel.

Prikupljaju se sljedeća polja:

- **Activity_Name** – naziv aktivnosti „Sesija”

- **Activity_CV** – ID za povezivanje događaja u sesiji povezivanja

- **Activity_StartStopType** – zaustavljanje

- **Activity_DateTimeTicks** – vrijeme podataka za aktivnost

#### <a name="officestreamdeviceactivitystart"></a>Office.StreamDevice.Activity.Start

Omogućuje nam da znamo je li početak strujanja izvora podataka uspješan.   Koristi se za stanje i nadzor značajke. Taj je događaj generirao dodatak Microsoft Data Streamer za Excel.

Prikupljaju se sljedeća polja:

- **Datasource_Type** – informacije o serijskom uređaju ili servisu aplikacije

- **DataSource_Name** – naziv povezanog izvora podataka

- **Activity_Name** – naziv aktivnosti „StreamDeviceData” ili „StreamFileData”

- **Activity_CV** – ID za povezivanje događaja u sesiji povezivanja

- **Activity_StartStopType** – početak

- **Activity_DateTimeTicks** – vrijeme podataka za aktivnost

#### <a name="officestreamdeviceactivitystop"></a>Office.StreamDevice.Activity.Stop

Omogućuje nam da znamo je li zaustavljanje strujanja izvora podataka uspješno.   Koristi se za stanje i nadzor značajke. Taj je događaj generirao dodatak Microsoft Data Streamer za Excel.

Prikupljaju se sljedeća polja:

- **Datasource_Type** – informacije o serijskom uređaju ili servisu aplikacije

- **DataSource_Name** – naziv povezanog izvora podataka

- **Activity_Name** – naziv aktivnosti „StreamDeviceData” ili „StreamFileData”

- **Activity_CV** – ID za povezivanje događaja u sesiji povezivanja

- **Activity_StartStopType** – zaustavljanje

- **Activity_DateTimeTicks** – vrijeme podataka za aktivnost

#### <a name="officetargetedmessagingabexperimentmessagetrigger"></a>Office.TargetedMessaging.ABExperimentMessageTrigger

Prati broj korisnika koji primaju poruke servisa BizBar i Dynamic Canvas iz značajke TargetedMessagingService (TMS). Ti su podaci ključni da bi se razumjelo koje poruke korisnici primaju i na kojoj površini kako bismo osigurali da ne propuste nijednu poruku koja može biti ključna za njihovo daljnje korištenje proizvoda. Također su potrebni za točno mjerenje uspjeha naših eksperimenata i kampanja pokrenutih putem TMS-a.

Prikupljaju se sljedeća polja:

  - **Data\_Surface** – naziv površine kojoj se isporučuje ova poruka putem servisa

  - **Data\_Flight** – identifikator ECS/CT međuverzije koji je korišten za isporuku poruke

  - **Data\_CampaignId** – identifikator kampanje koje je ova poruka dio

  - **Data\_MessageId** – identifikator ove poruke koju je isporučio servis

  - **Data\_TransactionId** – identifikator ove transakcije sa servisom

  - **Data\_TriggerPoint** – korak u kojem je ovaj događaj zapisan (poruka primljena i poruka prikazana)

#### <a name="officetextfontpickerfontselectedwin32"></a>Office.Text.FontPickerFontSelected.Win32

Taj događaj označava je li preuzeti font pravilno prikazan. Koristi se za označavanje uspjeha ili neuspjeha preuzimanja fonta.

Prikupljaju se sljedeća polja:

  - **Naziv fonta (Data\_Font)** – naziv fonta odabranog u biraču fontova

  - **Klik korisnika (Data\_FClick)** – je li korisnik odabrao stavku pomoću miša

#### <a name="officetextresourceclientrequestresourceinternal"></a>Office.Text.ResourceClient.RequestResourceInternal

Taj događaj označava je li font pravilno preuzet. Koristi se za označavanje uspjeha ili neuspjeha prikazivanja preuzetog fonta.

Prikupljaju se sljedeća polja:

  - **Data\_FontToken** – naziv datoteke resursa spremit će se kao

  - **Data\_HTTPResult** – rezultat HTTP zahtjeva

  - **Data\_HTTPStatusCode** – HTTP kod vraćen iz HTTP zahtjeva

  - **Data\_isInternetOn** – jesmo li imali vezu prilikom pokušaja dohvaćanja resursa

  - **Data\_RequestUrl** – URL resursa CDN kojeg pokušavamo dohvatiti



#### <a name="officetranslatordocumenttranslated"></a>Office.Translator.DocumentTranslated

Prikuplja uspjeh ili neuspjeh prijevoda cijelog dokumenta koji korisnik pokreće u servisu Translator SDX. To je vrlo važno zbog procjene stanja značajke prijevoda i reagiranja na kvarove koji se mogu dogoditi. Nadzor stanja scenarija „Prijevod dokumenta“ u programu Word.

Prikupljaju se sljedeća polja:

- **Data.actionSource** – kako je pokrenut prijevod odabira

- **Data.bodyBackgroundColor** – pozadinska boja spremnika teme sustava Office

- **Data.bodyForegroundColor** – boja prednjeg plana spremnika teme sustava Office

- **Data.browserLang** – trenutni jezik prikaza preglednika

- **Data.browserOnline** – zastarjelo

- **Data.browserPlatform** – platforma preglednika

- **Data.browserUserAgent** – korisnički agent preglednika

- **Data.colorDepth** – dubina boje sustava

- **Data.contentLanguage** – otkriveni jezik sadržaja za prijevod

- **Data.controlBackgroundColor** – pozadinska boja kontrole teme sustava Office

- **Data.controlForegroundColor** – boja prednjeg plana kontrole teme sustava Office

- **Data.correlationId** – jedinstveni identifikator zahtjeva poslanog servisu

- **Data.crossSessionId** – jedinstveni identifikator korisnika

- **Data.crossSessionStartTime** – vremenska oznaka UTC-a kada se pokrene sesija prijevoda

- **Data.currentTime** – vremenska oznaka UTC-a kada se pošalje ova telemetrijska poruka

- **Data.displayLanguage** – jezik prikaza sustava Office

- **Data.documentSourceLang** – jezik sadržaja dokumenta

- **Data.documentTargetLang** – jezik na koji će dokument biti preveden

- **Data.environment** – okruženje servisa kojem je zahtjev poslan

- **Data.errorMessage** – poruka o pogrešci koju je servis prijavio

- **Data.eventActionType** – vrsta telemetrijskog događaja

- **Data.eventTagId** – jedinstveni identifikator retka koda koji je stvorio ovu telemetrijsku poruku.

- **Data.flights** – omogućene međuverzije

- **Data.fileSize** – veličina datoteke programa Word za prijevod

- **Data.fileSource** – gdje je hostirana datoteka programa Word (izvanmrežno, na mreži)

- **Data.fileType** – nastavak datoteke programa Word

- **Data.innerHeight"** – visina spremnika bočnog okna

- **Data.innerWidth"** – širina spremnika bočnog okna

- **Data.lookupSourceLang** – ne koristi se za prijevod dokumenta

- **Data.lookupTargetLang** – ne koristi se za prijevod dokumenta

- **Data.officeHost** – aplikacija sustava Office koja hostira bočno okno

- **Data.officeLocale** – jezik korisnika sustava Office

- **Data.officeMachineId** – jedinstveni identifikator uređaja

- **Data.officePlatform** – platforma uređaja

- **Data.officeSessionId** – identifikator sesije sustava Office

- **Data.officeUserId** – jedinstveni identifikator korisnika sustava Office

- **Data.officeVersion** – verzija sustava Office

- **Data.pageXOffset** – položaj vodoravnog klizača u bočnom oknu s lijeve strane okna

- **Data.pageYOffset** – položaj okomitog klizača u bočnom oknu s gornje strane okna

- **Data.pixelDepth** – razlučivost boje zaslona

- **Data.responseCode** – kod odgovora na zahtjev iz servisa

- **Data.responseTime** – proteklo vrijeme zahtjeva 

- **Data.resultType** – rezultat zahtjeva

- **Data.screenHeight** – visina zaslona u pikselima

- **Data.screenLeft** – vodoravna koordinata prozora u odnosu prema zaslonu

- **Data.screenTop** – okomita koordinata prozora u odnosu prema zaslonu

- **Data.screenWidth** – širina zaslona u pikselima

- **Data.selectedTab** – koja je kartica odabrana, Odabir ili Dokument

- **Data.serverUrl** – URL servisa za prevođenje

- **Data.sessionId** – identifikator sesije u bočnom oknu

- **Data.sessionStartTime** – vremenska oznaka UTC-a kada se pokrene sesija prijevoda

- **Data.sourceTextHash** – raspršivanje teksta za prijevod

- **Data.sourceTextLength** – duljina teksta za prijevod

- **Data.sourceTextWords** – broj riječi u tekstu za prijevod

- **Data.warningMessage** – poruka s upozorenjem koju je prijavio servis


#### <a name="officetranslatortexttranslated"></a>Office.Translator.TextTranslated

Prikuplja uspjeh ili neuspjeh prijevoda odabira koji korisnik pokreće u servisu Translator SDX. To je vrlo važno zbog procjene stanja značajke prijevoda i reagiranja na kvarove koji se mogu dogoditi. Koristi se za praćenje stanja scenarija „Prijevod odabira“ u programima Excel, PowerPoint i Word.

Prikupljaju se sljedeća polja:

- **Data.actionSource** – kako je pokrenut prijevod odabira

- **Data.bodyBackgroundColor** – pozadinska boja spremnika teme sustava Office

- **Data.bodyForegroundColor** – boja prednjeg plana spremnika teme sustava Office

- **Data.browserLang** – trenutni jezik prikaza preglednika

- **Data.browserOnline** – zastarjelo

- **Data.browserPlatform** – platforma preglednika

- **Data.browserUserAgent** – korisnički agent preglednika

- **Data.colorDepth** – dubina boje sustava

- **Data.contentLanguage** – otkriveni jezik sadržaja za prijevod

- **Data.controlBackgroundColor** – pozadinska boja kontrole teme sustava Office

- **Data.controlForegroundColor** – boja prednjeg plana kontrole teme sustava Office

- **Data.correlationId** – jedinstveni identifikator zahtjeva poslanog servisu

- **Data.crossSessionId** – jedinstveni identifikator korisnika

- **Data.crossSessionStartTime** – vremenska oznaka UTC-a kada se pokrene sesija prijevoda

- **Data.currentTime** – vremenska oznaka UTC-a kada se pošalje ova telemetrijska poruka

- **Data.displayLanguage** – jezik prikaza sustava Office

- **Data.documentSourceLang** – ne koristi se za odabir

- **Data.documentTargetLang** – ne koristi se za odabir prijevoda

- **Data.environment** – okruženje servisa kojem je zahtjev poslan

- **Data.errorMessage** – poruka o pogrešci koju je servis prijavio

- **Data.eventActionType** – vrsta telemetrijskog događaja

- **Data.eventTagId"** – jedinstveni identifikator retka koda koji je stvorio ovu telemetrijsku poruku

- **Data.flights** – omogućene međuverzije

- **Data.innerHeight** – visina spremnika bočnog okna

- **Data.innerWidth** – širina spremnika bočnog okna

- **Data.lookupSourceLang** – jezik trenutno odabranog teksta

- **Data.lookupTargetLang** – jezik na koji će trenutno odabrani tekst biti preveden

- **Data.officeHost** – aplikacija sustava Office koja hostira bočno okno

- **Data.officeLocale** – jezik korisnika sustava Office

- **Data.officeMachineId** – jedinstveni identifikator uređaja

- **Data.officePlatform** – platforma uređaja

- **Data.officeSessionId** – identifikator sesije sustava Office

- **Data.officeUserId** – jedinstveni identifikator korisnika sustava Office

- **Data.officeVersion** – verzija sustava Office

- **Data.pageXOffset** – položaj vodoravnog klizača u bočnom oknu s lijeve strane okna

- **Data.pageYOffset** – položaj okomitog klizača u bočnom oknu s gornje strane okna

- **Data.pixelDepth** – razlučivost boje zaslona

- **Data.responseCode** – kod odgovora na zahtjev iz servisa

- **Data.responseTime** – proteklo vrijeme zahtjeva

- **Data.resultType** – rezultat zahtjeva

- **Data.screenHeight** – visina zaslona u pikselima

- **Data.screenLeft** – vodoravna koordinata prozora u odnosu prema zaslonu

- **Data.screenTop** – okomita koordinata prozora u odnosu prema zaslonu

- **Data.screenWidth** – širina zaslona u pikselima

- **Data.selectedTab** – koja je kartica odabrana, Odabir ili Dokument

- **Data.serverUrl** – URL servisa za prevođenje

- **Data.sessionId** – identifikator sesije u bočnom oknu

- **Data.sessionStartTime** – vremenska oznaka UTC-a kada se pokrene sesija prijevoda

- **Data.sourceTextHash** – raspršivanje teksta za prijevod

- **Data.sourceTextLength** – duljina teksta za prijevod

- **Data.sourceTextWords** – broj riječi u tekstu za prijevod

- **Data.warningMessage** – poruka s upozorenjem koju je prijavio servis


#### <a name="officeuxacccheckeracccheckerfinalviolationcountperrule"></a>Office.UX.AccChecker.AccCheckerFinalViolationCountPerRule

Ovaj se događaj aktivira kada se prijave problemi s pristupačnošću za trenutačno otvoreni dokument. Ovaj događaj predstavlja povrede pristupačnosti (pogreške, upozorenja i savjete) koja postoje za svako pravilo, za otvoreni dokument pri početku i kraju sesije.  Ovaj događaj upotrebljava se za evidenciju broja povreda pristupačnosti (pogreške, upozorenja i savjete) za svako pravilo, za otvoreni dokument pri početku i kraju sesije.

Pojedinosti o brojevima povreda za svako pravilo pomažu Microsoftu pri prepoznavanju koji su problemi s pristupačnošću najčešći u dokumentima sustava Office. To pomaže pri njihovu otklanjanju te potiče stvaranje inkluzivnog okruženja na radnom mjestu i u učionici za osobe s invaliditetom.

Prikupljaju se sljedeća polja:

- **Data_FinalCount_RuleID_0** – broj povreda ID-a pravila = n koji ostaje od zadnjeg puta kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_FinalCount_RuleID_1** – broj povreda ID-a pravila = n koji ostaje od zadnjeg puta kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_FinalCount_RuleID_2** – broj povreda ID-a pravila = n koji ostaje od zadnjeg puta kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_FinalCount_RuleID_3** – broj povreda ID-a pravila = n koji ostaje od zadnjeg puta kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_FinalCount_RuleID_4** – broj povreda ID-a pravila = n koji ostaje od zadnjeg puta kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_FinalCount_RuleID_5** – broj povreda ID-a pravila = n koji ostaje od zadnjeg puta kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_FinalCount_RuleID_6** – broj povreda ID-a pravila = n koji ostaje od zadnjeg puta kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_FinalCount_RuleID_7** – broj povreda ID-a pravila = n koji ostaje od zadnjeg puta kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_FinalCount_RuleID_8** – broj povreda ID-a pravila = n koji ostaje od zadnjeg puta kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_FinalCount_RuleID_9** – broj povreda ID-a pravila = n koji ostaje od zadnjeg puta kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_FinalCount_RuleID_10** – broj povreda ID-a pravila = n koji ostaje od zadnjeg puta kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_FinalCount_RuleID_11** – broj povreda ID-a pravila = n koji ostaje od zadnjeg puta kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_FinalCount_RuleID_12** – broj povreda ID-a pravila = n koji ostaje od zadnjeg puta kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_FinalCount_RuleID_13** – broj povreda ID-a pravila = n koji ostaje od zadnjeg puta kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_FinalCount_RuleID_14** – broj povreda ID-a pravila = n koji ostaje od zadnjeg puta kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_FinalCount_RuleID_15** – broj povreda ID-a pravila = n koji ostaje od zadnjeg puta kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_FinalCount_RuleID_16** – broj povreda ID-a pravila = n koji ostaje od zadnjeg puta kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_FinalCount_RuleID_17** – broj povreda ID-a pravila = n koji ostaje od zadnjeg puta kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_InitialCount_RuleID_0** – broj povreda ID-a pravila = n koji je pronađen prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_InitialCount_RuleID_1** – broj povreda ID-a pravila = n koji je pronađen prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_InitialCount_RuleID_2** – broj povreda ID-a pravila = n koji je pronađen prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_InitialCount_RuleID_3** – broj povreda ID-a pravila = n koji je pronađen prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_InitialCount_RuleID_4** – broj povreda ID-a pravila = n koji je pronađen prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_InitialCount_RuleID_5** – broj povreda ID-a pravila = n koji je pronađen prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_InitialCount_RuleID_6** – broj povreda ID-a pravila = n koji je pronađen prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_InitialCount_RuleID_7** – broj povreda ID-a pravila = n koji je pronađen prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_InitialCount_RuleID_8** – broj povreda ID-a pravila = n koji je pronađen prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_InitialCount_RuleID_9** – broj povreda ID-a pravila = n koji je pronađen prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_InitialCount_RuleID_10** – broj povreda ID-a pravila = n koji je pronađen prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_InitialCount_RuleID_11** – broj povreda ID-a pravila = n koji je pronađen prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_InitialCount_RuleID_12** – broj povreda ID-a pravila = n koji je pronađen prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_InitialCount_RuleID_13** – broj povreda ID-a pravila = n koji je pronađen prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_InitialCount_RuleID_14** – broj povreda ID-a pravila = n koji je pronađen prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_InitialCount_RuleID_15** – broj povreda ID-a pravila = n koji je pronađen prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_InitialCount_RuleID_16** – broj povreda ID-a pravila = n koji je pronađen prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **Data_InitialCount_RuleID_17** – broj povreda ID-a pravila = n koji je pronađen prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **FinalDocID** – konačni ID dokumenta skeniranog dokumenta

- **FinalDocUrlHash** – konačni URL raspršivanja dokumenta skeniranog dokumenta
    
- **InitialDocID** – početni ID dokumenta skeniranog dokumenta

- **InitialDocUrlHash** – početni URL raspršivanja dokumenta skeniranog dokumenta

- **PaneOpened** – Booleova vrijednost koja prati je li okno Provjere pristupačnosti bilo otvoreno

- **ServerDocID** – ID dokumenta poslužitelja za dokument koji je skenirala Provjera pristupačnosti


#### <a name="officeuxacccheckeracccheckerviolationinformation"></a>Office.UX.AccChecker.AccCheckerViolationInformation

Ovaj se događaj aktivira kada se prijave problemi s pristupačnošću za trenutačno otvoreni dokument. On predstavlja zbirni broj povreda (pogreške, upozorenja i savjete) koja postoje za svako pravilo, za otvoreni dokument pri početku i kraju sesije. Ovaj događaj upotrebljava se za evidenciju zbirnog broja povreda pristupačnosti (pogreške, upozorenja i savjete) za otvoreni dokument pri početku i kraju sesije. Znanje stečeno iz upotrebe Provjere pristupačnosti Microsoftu omogućuje poboljšanje kako bi doživljaji njegove aplikacije bili inkluzivniji za osobe s invaliditetom u scenarijima upotrebe sustava Office za radno mjesto i učionicu.

Prikupljaju se sljedeća polja:
    
- **FinalDocID** – konačni ID dokumenta skeniranog dokumenta

- **FinalDocUrlHash** – konačni URL raspršivanja dokumenta skeniranog dokumenta

- **FinalErrorCount** – konačan broj pogrešaka koje je Provjera pristupačnosti prijavila za dokument

- **FinalIntelligentServiceCount** – konačan broj problema s pametnim servisima koje je Provjera pristupačnosti prijavila za dokument

- **FinalTipCount** – konačan broj savjeta koje je Provjera pristupačnosti prijavila za dokument

- **FinalViolationCount** – konačan broj povreda koje je Provjera pristupačnosti prijavila za dokument

- **FinalWarningCount** – konačan broj upozorenja koje je Provjera pristupačnosti prijavila za dokument

- **InitialDocID** – početni ID dokumenta skeniranog dokumenta

- **InitialDocUrlHash** – početni URL raspršivanja dokumenta skeniranog dokumenta

- **InitialErrorCount** – broj svih povreda vrste Pogreška koje su pronađene prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **InitialIntelligentServicesCount** – broj svih povreda vrste Pametna usluga koje su pronađene prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **InitialTipCount** – broj svih povreda vrste Savjet koje su pronađene prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **InitialUrlHash** – broj svih povreda vrste Pogreška koje su pronađene prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **InitialViolationCount** – broj svih povreda koje su pronađene prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **InitialWarningCount** – broj svih povreda vrste Upozorenje koje su pronađene prvi put kada je Provjera pristupačnosti bila pokrenuta u sesiji.

- **PaneOpened** – Booleova vrijednost koja prati je li okno Provjere pristupačnosti dokumenta bilo otvoreno

- **ServerDocID** – ID dokumenta poslužitelja za dokument koji je skenirala Provjera pristupačnosti


#### <a name="officeuxacccheckerbackgroundacccheckerenabledstate"></a>Office.UX.AccChecker.BackgroundAccCheckerEnabledState

Ovaj se događaj aktivira kada je korisnik ili IT administrator omogućio pozadinski alat za provjeru pristupačnosti za korisnika sustava Office. Ovaj se događaj upotrebljava za razumijevanje slučajeva kada je pozadinski alat za provjeru pristupačnosti omogućen za korisnike sustava Office. Omogućeno stanje pozadinskog alata za provjeru pristupačnosti omogućuje Microsoftu utvrditi mogu li se dokumenti automatski skenirati u pozadini. Time se stvara inkluzivnije okruženje na radnom mjesto i u učionici za osobe s invaliditetom.

Prikupljaju se sljedeća polja:

- **BackgroundAccCheckerEnabled** – Booleova vrijednost za praćenje stanja Omogućeno/Onemogućen pozadinskog alata za provjeru pristupačnosti


#### <a name="officeuxacccheckerbackgroundscanningcheckboxclicked"></a>Office.UX.AccChecker.BackgroundScanningCheckboxClicked

Ovaj se događaj aktivira kada korisnik omogući pozadinski alat za provjeru pristupačnosti iz okna zadatka Provjere pristupačnosti.  Ovaj se događaj upotrebljava za razumijevanje slučajeva kada je pozadinski alat za provjeru pristupačnosti omogućen za dokumente sustava Office. Omogućeno stanje pozadinskog alata za provjeru pristupačnosti omogućuje Microsoftu utvrditi mogu li se dokumenti automatski skenirati u pozadini. Time se stvara inkluzivnije okruženje na radnom mjesto i u učionici za osobe s invaliditetom.

Prikupljaju se sljedeća polja:
    
- **FinalBackgroundScanningState** – početno stanje potvrdnog okvira koji omogućuje pozadinsko skeniranje

- **InitialBackgroundScanningState** – početno stanje potvrdnog okvira koji omogućuje pozadinsko skeniranje


#### <a name="officeuxacccheckerdisabledresults"></a>Office.UX.AccChecker.DisabledResults

Ovaj se događaj aktivira kada se Provjera pristupačnosti onemogući za otvoreni dokument. Ovaj se događaj upotrebljava za razumijevanje slučajeva kada se alat za provjeru pristupačnosti sustava Office onemogući zbog starije ili nepodržane verzije dokumenta sustava Office. Onemogućeno stanje Provjere pristupačnosti omogućuje Microsoftu utvrđivanje koliko se često dokument ne može skenirati te pomaže korisnicima pri dopuštanju skeniranja takvih dokumenata – pretvaranjem dokumenta u suvremeni oblik datoteke. Time se stvara inkluzivnije okruženje na radnom mjesto i u učionici za osobe s invaliditetom.

Prikupljaju se sljedeća polja:
    
- **Data_Disabled_ID** – ID onemogućene pogreške

- **Data_Disabled_Reason** – razlog za onemogućivanje Provjere pristupačnosti

- **Data_IsUpConvertEnabled** – prati je li dostupna mogućnost pretvaranja dokumenta u suvremen oblik datoteke


#### <a name="officeuxacccheckershowtaskpane"></a>Office.UX.AccChecker.ShowTaskPane

Ovaj se događaj aktivira kada se okno zadatka Provjere pristupačnosti pokrene za trenutačno otvoreni dokument.  Ovaj se događaj upotrebljava za razumijevanje upotrebe Provjere pristupačnosti sustava Office. Provjera pristupačnosti upotrebljava se za prepoznavanje i popravak problema s pristupačnošću u dokumentima sustava Office. Znanje stečeno iz upotrebe Provjere pristupačnosti Microsoftu omogućuje poboljšanje kako bi doživljaji njegove aplikacije bili inkluzivniji za osobe s invaliditetom u scenarijima upotrebe sustava Office za radno mjesto i učionicu.

Prikupljaju se sljedeća polja:

- **BackgroundScanCheckboxEnabled** – prati je li omogućen pozadinski alat za provjeru pristupačnosti
    
- **Column** – svrha

- **DocUrlHash** – jedinstveno raspršivanje ID-a dokumenta koji je bio skeniran

- **HasAccessibilityViolations** – prati sadrži li dokument ikakve povrede pristupačnosti u trenutku otvaranja okna

- **IsPaneDisabled** – prati je li okno Provjere pristupačnosti otvoreno u onemogućenom stanju (stara ili nepodržana verzija dokumenta)

- **PaneOpenedBefore** – prati je li okno Provjere pristupačnost već bilo otvoreno

- **WAC_ServerDocId** – ID dokumenta poslužitelja za dokument koji je bio skeniran


#### <a name="officevisiosharedfeatureexperimentation"></a>Office.Visio.Shared.FeatureExperimentation

Značajka prati isporuku testnih verzija korisnicima. Taj nam događaj pomaže odrediti uspješnost ili neuspješnost isporuke testnih verzija.

Prikupljaju se sljedeća polja:

  - **Data\_Enable:bool**– vrijednost „istinito” označava da je značajka omogućena za trenutnog korisnika

  - **Data\_Feature:string** – naziv značajke

  - **Data\_Flighted:bool** – vrijednost „istinito” označava da je značajka omogućena

  - **Data\_Licensed:bool** – vrijednost „istinito” označava da je značajka u postupku provjere licence

  - **Data\_Subscriber:bool** – vrijednost „istinito” označava da korisnik ima licencu za pretplatu

#### <a name="officevisiosharedrefreshsmartdiagram"></a>Office.Visio.Shared.RefreshSmartDiagram

Bilježi neuspjela osvježavanja dijagrama kada je datoteka stvorena putem DV-a. To nam olakšava ispravljanje pogrešaka i problema pri osvježavanju podataka u DV dijagramu.

Prikupljaju se sljedeća polja:

  - **Data\_ConnectorsBasedOnSequence:bool** – istinito ako je osvježeni dijagram izvorno stvoren korištenjem poveznika koji se temelji na mogućnosti „niz”

  - **Data\_DialogError**:**string** – pogreška tijekom osvježavanja pametnog dijagrama

  - **Data\_FileError:string** – niz pogreške kada povezana datoteka programa Excel nije valjana

  - **Data\_OverwriteSelected**:**bool** – istinito ako je korisnik odabrao mogućnost koja prebriše dijagram tijekom osvježavanja

  - **Data\_WarningShown**:**bool** – istinito ako se korisniku tijekom osvježavanja podataka prikazalo bilo kakvo upozorenje

#### <a name="officevisiosharedwritebacktoexcel"></a>Office.Visio.Shared.WritebackToExcel

Bilježi neuspjela povratna zapisivanja u Excel kada je datoteka stvorena putem DV-a. To nam olakšava ispravljanje pogrešaka i problema pri povratnom zapisivanju u Excel u DV dijagramu.

Prikupljaju se sljedeća polja:

  - **Data\_ConnectorsBasedOnSequence:bool** – vrijednost „istinito” znači da se poveznici stvaraju na temelju postavki niza

  - **Data\_DataSourceType:string** – to polje označava je li osnova za stvaranje dijagrama „Table” ili „CustomRange”

  - **Data\_DialogError:string** – prilagođena vrsta pogreške prilikom stvaranja pametnog dijagrama putem programa Excel

  - **Data\_NoOfShapesAdded:int** – broj oblika dodanih tijekom funkcije povratnog zapisivanja u Excel

  - **Data\_NoOfShapesDeleted:int** – broj oblika izbrisanih tijekom funkcije povratnog zapisivanja u Excel

  - **Data\_OverwriteSelected:bool** – vrijednost „istinito” označava da je korisnik odabrao mogućnost koja prebriše podatke

  - **Data\_SourceDataModified:bool** – vrijednost „istinito” označava da su izvorni podaci izmijenjeni

  - **Data\_WarningShown:bool** – vrijednost „istinito” označava da se korisniku prikazalo upozorenje o ažuriranju podataka

  - **Data\_WarningShownBecauseOfPresenceOfFormula:bool** – vrijednost „istinito” označava da se korisniku prikazalo upozorenje zbog prisutnosti formule u programu Excel

  - **Data\_WarningShownToAddNextStepID:bool** – vrijednost „istinito” označava da se korisniku prikazalo upozorenje zbog odsutnosti identifikatora sljedećeg koraka u programu Excel

  - **Data\_WarningShownToConvertToTable:bool** – vrijednost „istinito” označava da se korisniku prikazalo upozorenje da pretvori podatke programa Excel u tablični oblik


#### <a name="officewordfilenewcreatenewfile"></a>Office.Word.FileNew.CreateNewFile

Taj događaj označava da je novi dokument stvoren u programu Office Word i prati uspjeh ili neuspjeh operacije. Događaj se koristi za praćenje radi li stvaranje novog dokumenta prema očekivanjima. Koristi se i za izračunavanje broja mjesečnih aktivnih korisnika/uređaja i metriku pouzdanosti oblaka.

Prikupljaju se sljedeća polja:

  - **Data\_DirtyState** – je li dokument stvoren u prljavom stanju (s promjenama koje treba spremiti)

  - **Data\_ErrorID** – identifikator pogreške u slučaju pogreške operacije

  - **Data\_MainPdod –** identifikator dokumenta tijekom ove sesije postupka

  - **Data\_UsesCustomTemplate** – označava je li dokument stvoren iz prilagođenog predloška

#### <a name="officewordfileopenuserinitiatedopen"></a>Office.Word.FileOpen.UserInitiatedOpen 

Ovaj događaj označava da je aplikacija Office Word otvorila dokument na zahtjev korisnika umjesto programski putem aplikacije Office Word. Sadrži i ključne podatke o performansama otvaranja datoteka, a iz perspektive korisnika predstavlja događaj pokretanja aplikacije.  Događaj nadzire funkcionira li otvaranje datoteka prema očekivanjima. Koristi se i za izračunavanje broja mjesečnih aktivnih korisnika/uređaja i metriku pouzdanosti oblaka. 
 
Prikupljaju se sljedeća polja:

- **Data_AddDocTelemRes** – Izvještava jesmo li u slučaju uspjeli pravilno popuniti druge vrijednosti povezane s telemetrijom dokumenta. Koristi se za dijagnostiku kvalitete podataka. 

- **Data_BytesAsynchronous** – broj (sažetih) bajtova za koje vjerujemo da možemo otvoriti datoteku bez njih ako ih dobijemo prije nego što korisnik poželi početi uređivati ili možda spremati. 

- **Data_BytesAsynchronousWithWork** – broj (sažetih) bajtova bez kojih bismo možda mogli otvoriti datoteku, ali bi to zahtijevalo značajna ulaganja u kod 

- **Data_BytesSynchronous** – broj (sažetih) bajtova koje moramo imati prije nego što možemo početi otvarati datoteku 

- **Data_BytesUnknown** – broj bajtova u dijelovima dokumenta koje ne očekujemo pronaći. 

- **Data_Doc_AccessMode** – dokument je samo za čitanje/uređivanje 

- **Data_Doc_AssistedReadingReasons** – unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju 

- **Data_Doc_ChunkingType** – jedinice koje se koriste za inkrementalno otvaranje dokumenta 

- **Data_Doc_EdpState** – postavka zaštite elektroničkih podataka za dokument 

- **Data_Doc_Ext** – nastavak dokumenta (docx/xlsb/pptx itd.) 

- **Data_Doc_FileFormat** – verzija protokola oblika datoteke 

- **Data_Doc_Fqdn** – naziv domene servisa OneDrive ili sustava SharePoint Online 

- **Data_Doc_FqdnHash** – jednosmjerno raspršivanje naziva domene koji identificira korisnika 

- **Data_Doc_IdentityTelemetryId** – jednosmjerno raspršivanje korisničkog identiteta kojim se izvršava otvaranje 

- **Data_Doc_InitializationScenario** – bilježi način otvaranja dokumenta 

- **Data_Doc_IOFlags** – izvješćuje o predmemoriranim zastavicama za postavljanje mogućnosti zahtjeva 

- **Data_Doc_IrmRights** – radnje koje dopuštaju pravila zaštite elektroničkih podataka koja su primijenjena na dokument/korisnika 

- **Data_Doc_IsIncrementalOpen** – zastavica koja označava da je dokument inkrementalno otvoren 

- **Data_Doc_IsOcsSupported** – zastavica koja označava da je dokument podržan u servisu za suradnju 

- **Data_Doc_IsOpeningOfflineCopy** – zastavica koja označava da je otvorena izvanmrežna kopija dokumenta 

- **Data_Doc_IsSyncBacked** – zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta 

- **Data_Doc_Location** – označava koji je servis pružio dokument (OneDrive, File Server, SharePoint) 

- **Data_Doc_LocationDetails** – označava koja je poznata mapa pružila lokalno pohranjeni dokument 

- **Data_Doc_NumberCoAuthors** – broj drugih korisnika u sesiji zajedničkog uređivanja 

- **Data_Doc_PasswordFlags** – označava postavljene zastavice za čitanje/pisanje lozinke 

- **Data_Doc_ReadOnlyReasons** – razlozi zbog kojih je dokument otvoren samo za čitanje 

- **Data_Doc_ResourceIdHash** – anonimizirani identifikator dokumenta za dijagnosticiranje problema 

- **Data_Doc_ServerDocId** – nepromjenjivi anonimizirani identifikator dokumenta za dijagnosticiranje problema 

- **Data_Doc_ServerProtocol** – verzija protokola za komuniciranje sa servisom 

- **Data_Doc_ServerType** – vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.) 

- **Data_Doc_ServerVersion** – verzija poslužitelja koji pruža servis 

- **Data_Doc_SessionId** – verzija poslužitelja koji pruža servis 

- **Data_Doc_SharePointServiceContext** – dijagnostičke informacije iz zahtjeva sustava SharePoint Online 

- **Data_Doc_SizeInBytes** – pokazatelj veličine dokumenta 

- **Data_Doc_SpecialChars** – pokazatelj posebnih znakova u URL-u ili putu dokumenta 

- **Data_Doc_StreamAvailability** – pokazatelj je li niz dokumenata dostupan/onemogućen 

- **Data_Doc_SyncBackedType** – pokazatelj vrste dokumenta (lokalni ili na servisu) 

- **Data_Doc_UrlHash** – jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta 

- **Data_Doc_WopiServiceId** – sadrži jedinstveni identifikator davatelja usluga WOPI 

- **Data_EditorDisablingRename** – identifikator prvog uređivača koji je uzrokovao onemogućivanje preimenovanja 

- **Data_EditorsCount** – broj uređivača dokumenta 

- **Data_ForceReadWriteReason** – cijeli broj koji predstavlja razlog zbog kojeg je datoteka prisilno prebačena u način rada za čitanje/pisanje 

- **Data_FSucceededAfterRecoverableFailure** – označava da je otvaranje uspjelo nakon popravljanja neuspjelog otvaranja dokumenta 

- **Data_LastLoggedTag** – jedinstvena oznaka mjesta pozivanja koda, koja se koristi za identifikaciju dvokratnog neuspjelog pokušaja otvaranja (koristi se za dijagnostiku kvalitete podataka) 

- **Data_LinkStyles** – označava povezujemo li se sa stilovima predloška 

- **Data_MainPdod** – identifikator dokumenta u sklopu procesa Office Word 

- **Data_Measurements** – šifrirani niz koji sadrži analizu trajanja različitih dijelova otvaranja. Koristi se za dijagnosticiranje performansi otvaranja. 

- **Data_MoveDisabledReason** – pogreška koja onemogućuje premještanje dokumenta 

- **Data_MoveFlightEnabled** – je li omogućena testna verzija za značajku premještanja 

- **Data_OpenInitiateKind** – vrsta scenarija u kojem su korisnici pokrenuli ovu operaciju otvaranja datoteka. 

- **Data_PartsUnknown** – broj dijelova dokumenta za koje nismo mogli pribaviti podatke 

- **Data_RecoverableFailureInitiationLocationTag** – jedinstvena oznaka mjesta pozivanja koda, koja se koristi za identifikaciju mjesta na kojem pokušavamo popraviti datoteku prije otvaranja 

- **Data_RenameDisabledReason** – pogreška koja uzrokuje onemogućivanje preimenovanja za taj dokument 

- **Data_RenameFlightEnabled** – je li omogućena testna verzija za značajku preimenovanja 

- **Data_SecondaryTag** – jedinstvena oznaka mjesta pozivanja koda, koja se koristi za dodavanje dodatnih podataka o neuspjelom otvaranju. 

- **Data_TemplateFormat** – oblik datoteke predloška na kojem se dokument temelji. 

- **Data_UsesNormal** – označava temelji li se otvoreni dokument na predlošku Normal. 

- **Data_VerboseMeasurements** – šifrirani niz koji sadrži detaljnu analizu trajanja različitih dijelova otvaranja.  Koristi se za mjerenje učinkovitosti, a omogućeno je samo za interne krugove. 



#### <a name="officewordfilesaveactcmdgosubsaveas"></a>Office.Word.FileSave.ActCmdGosubSaveAs

Taj događaj označava da korisnik sprema promjene u novom dokumentu. Događaj nadzire funkcionira li spremanje u novom dokumentu prema očekivanjima. Koristi se i za izračunavanje broja mjesečnih aktivnih korisnika/uređaja i metriku pouzdanosti oblaka.

Prikupljaju se sljedeća polja:

- **Data_AddDocTelemRes** – Izvještava jesmo li u slučaju uspjeli pravilno popuniti druge vrijednosti povezane s telemetrijom dokumenta. Koristi se za dijagnostiku kvalitete podataka.

- **Data_DetachedDuration** – koliko je dugo aktivnost bila odvojena od niti

- **Data_Doc_AccessMode** – dokument je samo za čitanje/uređivanje

- **Data_Doc_AssistedReadingReasons** – unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

- **Data_Doc_AsyncOpenKind –** označava je li otvorena predmemorirana verzija dokumenta u oblaku i koja je logika za asinkrono osvježavanje korištena.

- **Data_Doc_ChunkingType** – jedinice koje se koriste za inkrementalno otvaranje dokumenta

- **Data_Doc_EdpState** – postavka zaštite elektroničkih podataka za dokument

- **Data_Doc_Ext** – nastavak dokumenta (docx/xlsb/pptx itd.)

- **Data_Doc_FileFormat** – verzija protokola oblika datoteke

- **Data_Doc_Fqdn** – naziv domene servisa OneDrive ili sustava SharePoint Online

- **Data_Doc_FqdnHash** – jednosmjerno raspršivanje naziva domene koji identificira korisnika

- **Data_Doc_IdentityTelemetryId** – jednosmjerno raspršivanje korisničkog identiteta kojim se izvršava otvaranje

- **Data_Doc_InitializationScenario** – bilježi način otvaranja dokumenta

- **Data_Doc_IOFlags** – izvješćuje o predmemoriranim zastavicama za postavljanje mogućnosti zahtjeva

- **Data_Doc_IrmRights** – radnje koje dopuštaju pravila zaštite elektroničkih podataka koja su primijenjena na dokument/korisnika
    
- **Data_Doc_IsIncrementalOpen** – zastavica koja označava da je dokument inkrementalno otvoren

- **Data_Doc_IsOcsSupported** – zastavica koja označava da je dokument podržan u servisu za suradnju
    
- **Data_Doc_IsOpeningOfflineCopy** – zastavica koja označava da je otvorena izvanmrežna kopija dokumenta

- **Data_Doc_IsSyncBacked** – zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

- **Data_Doc_Location** – označava koji je servis pružio dokument (OneDrive, File Server, SharePoint itd.)

- **Data_Doc_LocationDetails** – označava koja je poznata mapa pružila lokalno pohranjeni dokument

- **Data_Doc_NumberCoAuthors** – broj drugih korisnika u sesiji zajedničkog uređivanja

- **Data_Doc_PasswordFlags** – označava postavljene zastavice za čitanje/pisanje lozinke

- **Data_Doc_ReadOnlyReasons** – razlozi zbog kojih je dokument otvoren samo za čitanje

- **Data_Doc_ResourceIdHash** – anonimizirani identifikator dokumenta za dijagnosticiranje problema

- **Data_Doc_RtcType** – označava kako je postavljen kanal u stvarnom vremenu (RTC) za trenutnu datoteku (Onemogućeno, nepodržano, na zahtjev, uvijek uključeno itd.).

- **Data_Doc_ServerDocId** – nepromjenjivi anonimizirani identifikator dokumenta za dijagnosticiranje problema

- **Data_Doc_ServerProtocol** – verzija protokola za komuniciranje sa servisom

- **Data_Doc_ServerType** – vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.)

- **Data_Doc_ServerVersion** – verzija poslužitelja koji pruža servis

- **Data_Doc_SessionId** – označava određenu sesiju uređivanja dokumenta u cijeloj sesiji

- **Data_Doc_SharePointServiceContext** – dijagnostičke informacije iz zahtjeva sustava SharePoint Online

- **Data_Doc_SizeInBytes** – pokazatelj veličine dokumenta

- **Data_Doc_SpecialChars** – pokazatelj posebnih znakova u URL-u ili putu dokumenta

- **Data_Doc_StreamAvailability** – pokazatelj je li niz dokumenata dostupan/onemogućen

- **Data_Doc_SyncBackedType** – pokazatelj vrste dokumenta (lokalni ili na servisu)

- **Data_Doc_UrlHash** – jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta

- **Data_EditorDisablingRename** – identifikator prvog uređivača koji je uzrokovao onemogućivanje preimenovanja

- **Data_EditorsCount** – broj uređivača dokumenta

- **Data_LastLoggedTag** – jedinstvena oznaka mjesta pozivanja koda, koja se koristi za identifikaciju dvokratnog neuspjelog pokušaja spremanja (koristi se za dijagnostiku kvalitete podataka)

- **Data_MoveDisabledReason** – pogreška koja onemogućuje premještanje dokumenta

- **Data_MoveFlightEnabled** – je li omogućena testna verzija za značajku premještanja

- **Data_RenameDisabledReason** – pogreška koja uzrokuje onemogućivanje preimenovanja za dokument

- **Data_RenameFlightEnabled** – je li omogućena testna verzija za značajku preimenovanja

    

#### <a name="officewordfilesaveactfconfirmsavedoccorequerysave"></a>Office.Word.FileSave.ActFConfirmSaveDocCoreQuerySave

Taj događaj označava da Office Word traži od korisnika da spremi promjene kada pokuša zatvoriti dokument. To omogućuje Microsoftu praćenje radi li spremanje pri zatvaranju prema očekivanjima kako bi se spriječio gubitak podataka. Događaj nadzire funkcionira li spremanje pri zatvaranju prema očekivanjima. Koristi se i za izračunavanje broja mjesečnih aktivnih korisnika/uređaja i metriku pouzdanosti oblaka.

Prikupljaju se sljedeća polja:

- **Data_AddDocTelemRes** – Izvještava jesmo li u slučaju uspjeli pravilno popuniti druge vrijednosti povezane s telemetrijom dokumenta. Koristi se za dijagnostiku kvalitete podataka.

- **Data_DetachedDuration** – koliko je dugo aktivnost bila odvojena od niti

- **Data_Doc_AccessMode** – dokument je samo za čitanje/uređivanje

- **Data_Doc_AssistedReadingReasons** – unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

- **Data_Doc_AsyncOpenKind –** označava je li otvorena predmemorirana verzija dokumenta u oblaku i koja je logika za asinkrono osvježavanje korištena.

- **Data_Doc_ChunkingType** – jedinice koje se koriste za inkrementalno otvaranje dokumenta

- **Data_Doc_EdpState** – postavka zaštite elektroničkih podataka za dokument

- **Data_Doc_Ext** – nastavak dokumenta (docx/xlsb/pptx itd.)

- **Data_Doc_FileFormat** – verzija protokola oblika datoteke

- **Data_Doc_Fqdn** – naziv domene servisa OneDrive ili sustava SharePoint Online

- **Data_Doc_FqdnHash** – jednosmjerno raspršivanje naziva domene koji identificira korisnika

- **Data_Doc_IdentityTelemetryId** – jednosmjerno raspršivanje korisničkog identiteta kojim se izvršava otvaranje

- **Data_Doc_InitializationScenario** – bilježi način otvaranja dokumenta

- **Data_Doc_IOFlags** – izvješćuje o predmemoriranim zastavicama za postavljanje mogućnosti zahtjeva

- **Data_Doc_IrmRights** – radnje koje dopuštaju pravila zaštite elektroničkih podataka koja su primijenjena na dokument/korisnika

- **Data_Doc_IsIncrementalOpen** – zastavica koja označava da je dokument inkrementalno otvoren

- **Data_Doc_IsOcsSupported** – zastavica koja označava da je dokument podržan u servisu za suradnju
    
- **Data_Doc_IsOpeningOfflineCopy** – zastavica koja označava da je otvorena izvanmrežna kopija dokumenta

- **Data_Doc_IsSyncBacked** – zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

- **Data_Doc_Location** – označava koji je servis pružio dokument (OneDrive, File Server, SharePoint itd.)

- **Data_Doc_LocationDetails** – označava koja je poznata mapa pružila lokalno pohranjeni dokument

- **Data_Doc_NumberCoAuthors** – broj drugih korisnika u sesiji zajedničkog uređivanja

- **Data_Doc_PasswordFlags** – označava postavljene zastavice za čitanje/pisanje lozinke

- **Data_Doc_ReadOnlyReasons** – razlozi zbog kojih je dokument otvoren samo za čitanje

- **Data_Doc_ResourceIdHash** – anonimizirani identifikator dokumenta za dijagnosticiranje problema

- **Data_Doc_RtcType** – označava kako je postavljen kanal u stvarnom vremenu (RTC) za trenutnu datoteku (Onemogućeno, nepodržano, na zahtjev, uvijek uključeno itd.).

- **Data_Doc_ServerDocId** – nepromjenjivi anonimizirani identifikator dokumenta za dijagnosticiranje problema

- **Data_Doc_ServerProtocol** – verzija protokola za komuniciranje sa servisom

- **Data_Doc_ServerType** – vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.)

- **Data_Doc_ServerVersion** – verzija poslužitelja koji pruža servis

- **Data_Doc_SessionId** – označava određenu sesiju uređivanja dokumenta u cijeloj sesiji

- **Data_Doc_SharePointServiceContext** – dijagnostičke informacije iz zahtjeva sustava SharePoint Online

- **Data_Doc_SizeInBytes** – pokazatelj veličine dokumenta

- **Data_Doc_SpecialChars** – pokazatelj posebnih znakova u URL-u ili putu dokumenta

- **Data_Doc_StreamAvailability** – pokazatelj je li niz dokumenata dostupan/onemogućen

- **Data_Doc_SyncBackedType** – pokazatelj vrste dokumenta (lokalni ili na servisu)

- **Data_Doc_UrlHash** – jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta

- **Data_Doc_WopiServiceId** – sadrži jedinstveni identifikator davatelja usluga WOPI

- **Data_DstDoc_AccessMode** – odredišni je dokument samo za čitanje ili za uređivanje

- **Data_DstDoc_EdpState** – postavka zaštite elektroničkih podataka za odredišni dokument

- **Data_DstDoc_Ext** – nastavak dokumenta (docx/xlsb/pptx itd.) za odredišni dokument

- **Data_DstDoc_FileFormat** – verzija protokola za oblik datoteke za odredišni dokument

- **Data_DstDoc_Location** – označava koji će servis pružiti pohranu odredišnog dokumenta (OneDrive, File Server, SharePoint itd.)

- **Data_DstDoc_LocationDetails** – označava koja je lokalna poznata mapa pohranila odredišni dokument

- **Data_DstDoc_SessionId** – označava određenu sesiju uređivanja dokumenta u cijeloj sesiji

- **Data_DstDoc_UrlHash** – jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta za odredišni dokument

- **Data_FailureClass** – cijeli broj koji predstavlja klasu neuspjeha za neuspjehe OCS tranzicije

- **Data_LocationPickerSaveStatus** – cjelobrojna vrijednost koja označava akciju koja je aktivirala spremanje iz dijaloškog okvira za spremanje prilikom izlaska

- **Data_MainPdod** – identifikator dokumenta u sklopu procesa Office Word.

- **Data_MoveFlightEnabled** – je li omogućena testna verzija za značajku premještanja

- **Data_OCSSyncbackSaveStarted** – zastavica koja označava da je to spremanje povezano sa spremanjem radi povratne sinkronizacije 

- **Data_RenameDisabledReason** – pogreška koja uzrokuje onemogućivanje preimenovanja za taj dokument

- **Data_RenameFlightEnabled** – je li omogućena testna verzija za značajku preimenovanja

- **Data_SaveInitiateKind** – cijeli broj koji označava kako je pokrenuto spremanje

- **Data_SrcDocIsUnnamedOrNew** – označava je li dokument koji spremamo nov


#### <a name="officewordfilesavesaveassavefile"></a>Office.Word.FileSave.SaveAsSaveFile

Taj događaj označava da Office Word sprema dokument u novi dokument. On Microsoftu omogućuje otkrivanje pogrešaka pri izvođenju naredbe Spremi kao, što je važno za izbjegavanje gubitka podataka iz dokumenta. Događaj nadzire funkcionira li naredba Spremi kao prema očekivanjima. Koristi se i izračunavanje broja mjesečnih aktivnih korisnika/uređaja i metriku pouzdanosti oblaka.

Prikupljaju se sljedeća polja:

- **Data_AddDocTelemRes** – Izvještava jesmo li u slučaju uspjeli pravilno popuniti druge vrijednosti povezane s telemetrijom dokumenta. Koristi se za dijagnostiku kvalitete podataka.

- **Data_AddDocTelemResDst** – izvješćuje jesmo li mogli pravilno popuniti ostale vrijednosti vezane uz telemetriju dokumenta u sklopu događaja za odredišni dokument. Koristi se za dijagnostiku kvalitete podataka.

- **Data_AddDocTelemResSrc** – izvješćuje jesmo li mogli pravilno popuniti ostale vrijednosti vezane uz telemetriju dokumenta u sklopu događaja za izvorni dokument. Koristi se za dijagnostiku kvalitete podataka.

- **Data_DetachedDuration** – koliko je dugo aktivnost bila odvojena od niti

- **Data_Doc_AccessMode** – dokument je samo za čitanje/uređivanje

- **Data_Doc_AssistedReadingReasons** – unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

- **Data_Doc_AsyncOpenKind –** označava je li otvorena predmemorirana verzija dokumenta u oblaku i koja je logika za asinkrono osvježavanje korištena.

- **Data_Doc_ChunkingType** – jedinice koje se koriste za inkrementalno otvaranje dokumenta

- **Data_Doc_EdpState** – postavka zaštite elektroničkih podataka za dokument

- **Data_Doc_Ext** – nastavak dokumenta (docx/xlsb/pptx itd.)

- **Data_Doc_FileFormat** – verzija protokola oblika datoteke

- **Data_Doc_Fqdn** – naziv domene servisa OneDrive ili sustava SharePoint Online

- **Data_Doc_FqdnHash** – jednosmjerno raspršivanje naziva domene koji identificira korisnika

- **Data_Doc_IdentityTelemetryId** – jednosmjerno raspršivanje korisničkog identiteta kojim se izvršava otvaranje

- **Data_Doc_IOFlags** – izvješćuje o predmemoriranim zastavicama za postavljanje mogućnosti zahtjeva

- **Data_Doc_IrmRights** – radnje koje dopuštaju pravila zaštite elektroničkih podataka koja su primijenjena na dokument/korisnika

- **Data_Doc_IsIncrementalOpen** – zastavica koja označava da je dokument inkrementalno otvoren

- **Data_Doc_IsOcsSupported** – zastavica koja označava da je dokument podržan u servisu za suradnju

- **Data_Doc_IsOpeningOfflineCopy** – zastavica koja označava da je otvorena izvanmrežna kopija dokumenta

- **Data_Doc_IsSyncBacked** – zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

- **Data_Doc_Location** – označava koji je servis pružio dokument (OneDrive, File Server, SharePoint itd.)

- **Data_Doc_LocationDetails** – označava koja je poznata mapa pružila lokalno pohranjeni dokument

- **Data_Doc_NumberCoAuthors** – broj drugih korisnika u sesiji zajedničkog uređivanja

- **Data_Doc_ReadOnlyReasons** – razlozi zbog kojih je dokument otvoren samo za čitanje

- **Data_Doc_ResourceIdHash** – anonimizirani identifikator dokumenta za dijagnosticiranje problema

- **Data_Doc_RtcType** – označava kako je postavljen kanal u stvarnom vremenu (RTC) za trenutnu datoteku (Onemogućeno, nepodržano, na zahtjev, uvijek uključeno itd.).

- **Data_Doc_ServerDocId** – nepromjenjivi anonimizirani identifikator dokumenta za dijagnosticiranje problema

- **Data_Doc_ServerProtocol** – verzija protokola za komuniciranje sa servisom

- **Data_Doc_ServerType** – vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.)

- **Data_Doc_ServerVersion** – verzija poslužitelja koji pruža servis

- **Data_Doc_SessionId** – označava određenu sesiju uređivanja dokumenta u cijeloj sesiji

- **Data_Doc_SharePointServiceContext** – dijagnostičke informacije iz zahtjeva sustava SharePoint Online

- **Data_Doc_SizeInBytes** – pokazatelj veličine dokumenta

- **Data_Doc_SpecialChars** – pokazatelj posebnih znakova u URL-u ili putu dokumenta

- **Data_Doc_StreamAvailability** – pokazatelj je li niz dokumenata dostupan/onemogućen

- **Data_Doc_UrlHash** – jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta

- **Data_DstDoc_AccessMode** – odredišni je dokument samo za čitanje ili za uređivanje

- **Data_DstDoc_AssistedReadingReasons** – unaprijed definiran skup vrijednosti razloga zbog kojih se odredišni dokument otvorio u načinu za pomoć pri čitanju

- **Data_DstDoc_AsyncOpenKind –** označava je li otvorena predmemorirana verzija dokumenta u novom oblaku i koja je logika za asinkrono osvježavanje korištena.
    
- **Data_DstDoc_ChunkingType** – jedinice koje se koriste za inkrementalno otvaranje dokumenta

- **Data_DstDoc_EdpState** – postavka zaštite elektroničkih podataka za odredišni dokument

- **Data_DstDoc_Ext** – nastavak dokumenta (docx/xlsb/pptx itd.)

- **Data_DstDoc_FileFormat** – verzija protokola oblika datoteke

- **Data_DstDoc_Fqdn** – naziv domene servisa OneDrive ili sustava SharePoint Online za odredišni dokument

- **Data_DstDoc_FqdnHash** – jednosmjerno raspršivanje naziva domene koji identificira korisnika za odredišni dokument

- **Data_DstDoc_IdentityTelemetryId** – jednosmjerno raspršivanje korisničkog identiteta kojim se izvršava otvaranje

- **Data_DstDoc_InitializationScenario** – bilježi način otvaranja dokumenta

- **Data_DstDoc_IOFlags** – izvješćuje o predmemoriranim zastavicama korištenima za postavljanje mogućnosti otvorenog zahtjeva za odredišni dokument
    
- **Data_DstDoc_IrmRights** – radnje dopuštene pravilima zaštite elektroničkih podataka primijenjenima na odredišni dokument ili odredišnog korisnika

- **Data_DstDoc_IsIncrementalOpen** – zastavica koja označava da je dokument inkrementalno otvoren

- **Data_DstDoc_IsOcsSupported** – zastavica koja označava da je dokument podržan u servisu za suradnju

- **Data_DstDoc_IsOpeningOfflineCopy** – zastavica koja označava da je otvorena izvanmrežna kopija dokumenta

- **Data_DstDoc_IsSyncBacked** – zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

- **Data_DstDoc_Location** – označava koji je servis pružio pohranu odredišnog dokumenta (OneDrive, File Server, SharePoint itd.)

- **Data_DstDoc_LocationDetails** – označava koja je poznata mapa pružila lokalno pohranjeni dokument

- **Data_DstDoc_NumberCoAuthors** – broj drugih korisnika u sesiji zajedničkog uređivanja

- **Data_DstDoc_PasswordFlags** – označava zastavice za čitanje ili čitanje i pisanje lozinke postavljene za odredišni dokument

- **Data_DstDoc_ReadOnlyReasons** – razlozi zbog kojih je odredišni dokument otvoren samo za čitanje 

- **Data_DstDoc_ResourceIdHash** – anonimizirani identifikator dokumenta za dijagnosticiranje problema

- **Data_DstDoc_ServerDocId** – nepromjenjivi anonimizirani identifikator dokumenta za dijagnosticiranje problema

- **Data_DstDoc_ServerProtocol** – verzija protokola za komuniciranje sa servisom

- **Data_DstDoc_ServerType** – vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.)
    
- **Data_DstDoc_ServerVersion** – verzija poslužitelja koji pruža servis

- **Data_DstDoc_SessionId** – označava određenu sesiju uređivanja dokumenta u cijeloj sesiji

- **Data_DstDoc_SharePointServiceContext** – dijagnostičke informacije iz zahtjeva sustava SharePoint Online

- **Data_DstDoc_SizeInBytes** – pokazatelj veličine dokumenta

- **Data_DstDoc_SpecialChars** – pokazatelj posebnih znakova u URL-u ili putu dokumenta

- **Data_DstDoc_StreamAvailability** – pokazatelj je li niz dokumenata dostupan/onemogućen

- **Data_DstDoc_SyncBackedType** – pokazatelj vrste dokumenta (lokalni ili na servisu)

- **Data_DstDoc_UrlHash** – jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta za odredišni dokument
    
- **Data_DstDoc_WopiServiceId** – sadrži jedinstveni identifikator davatelja usluga WOPI

- **Data_FailureClass** – cijeli broj koji predstavlja klasu neuspjeha za neuspjehe OCS tranzicije

- **Data_LocationPickerPropagateToSaveTime,spLapsedMsec** – u milisekundama mjeri vrijeme potrebno da se pokrene spremanje nakon dobivanja rezultata od birača lokacije

- **Data_LocationPickerSaveStatus** – status koji je birač lokacije vratio

- **Data_MainPdod** – identifikator dokumenta u sklopu procesa Office Word

- **Data_MoveDisabledReason** – pogreška koja onemogućuje premještanje dokumenta

- **Data_MoveFlightEnabled** – je li omogućena testna verzija za značajku premještanja

- **Data_RenameDisabledReason** – pogreška koja uzrokuje onemogućivanje preimenovanja za taj dokument

- **Data_RenameFlightEnabled** – je li omogućena testna verzija za značajku preimenovanja

- **Data_SaveInitiateKind** – cijeli broj koji označava kako je pokrenuto spremanje

- **Data_SrcDoc_AccessMode** – izvorni je dokument samo za čitanje ili za uređivanje

- **Data_SrcDoc_AssistedReadingReasons** – unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

- **Data_SrcDoc_AsyncOpenKind –** označava je li otvorena predmemorirana verzija dokumenta u izvornom oblaku i koja je logika za asinkrono osvježavanje korištena.

- **Data_SrcDoc_ChunkingType** – jedinice koje se koriste za inkrementalno otvaranje dokumenta

- **Data_SrcDoc_EdpState** – postavka zaštite elektroničkih podataka za izvorni dokument

- **Data_SrcDoc_Ext** – nastavak dokumenta za izvorni dokument (docx/xlsb/pptx itd.)

- **Data_SrcDoc_FileFormat** – verzija protokola za oblik datoteke za izvorni dokument

- **Data_SrcDoc_Fqdn** – naziv domene servisa OneDrive ili sustava SharePoint Online za izvorni dokument

- **Data_SrcDoc_FqdnHash** – jednosmjerno raspršivanje naziva domene koji identificira korisnika za izvorni dokument

- **Data_SrcDoc_IdentityTelemetryId** – jednosmjerno raspršivanje korisničkog identiteta kojim se izvršava otvaranje

- **Data_SrcDoc_InitializationScenario** – bilježi način otvaranja dokumenta

- **Data_SrcDoc_IOFlags** – izvješćuje o predmemoriranim zastavicama za postavljanje mogućnosti zahtjeva

- **Data_SrcDoc_IrmRights** – radnje koje dopuštaju pravila zaštite elektroničkih podataka koja su primijenjena na dokument/korisnika

- **Data_SrcDoc_IsIncrementalOpen** – zastavica koja označava da je dokument inkrementalno otvoren

- **Data_SrcDoc_IsOcsSupported** – zastavica koja označava da je dokument podržan u servisu za suradnju

- **Data_SrcDoc_IsOpeningOfflineCopy** – zastavica koja označava da je otvorena izvanmrežna kopija dokumenta

- **Data_SrcDoc_IsSyncBacked** – zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta
    
- **Data_SrcDoc_Location** – označava koji je servis dobavio izvorni dokument (OneDrive, File Server, SharePoint itd.)

- **Data_SrcDoc_LocationDetails** – označava koja je poznata mapa pružila lokalno pohranjeni dokument

- **Data_SrcDoc_NumberCoAuthors** – broj drugih korisnika u sesiji zajedničkog uređivanja

- **Data_SrcDoc_PasswordFlags** – označava postavljene zastavice za čitanje/pisanje lozinke

- **Data_SrcDoc_ReadOnlyReasons** – razlozi zbog kojih je dokument otvoren samo za čitanje

- **Data_SrcDoc_ResourceIdHash** – anonimizirani identifikator dokumenta za dijagnosticiranje problema

- **Data_SrcDoc_ServerDocId** – nepromjenjivi anonimizirani identifikator dokumenta za dijagnosticiranje problema

- **Data_SrcDoc_ServerProtocol** – verzija protokola za komuniciranje sa servisom

- **Data_SrcDoc_ServerType** – vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.)

- **Data_SrcDoc_ServerVersion** – verzija poslužitelja koji pruža servis

- **Data_SrcDoc_SessionId** – označava određenu sesiju uređivanja dokumenta u cijeloj sesiji

- **Data_SrcDoc_SharePointServiceContext** – dijagnostičke informacije iz zahtjeva sustava SharePoint Online

- **Data_SrcDoc_SizeInBytes** – pokazatelj veličine dokumenta

- **Data_SrcDoc_SpecialChars** – pokazatelj posebnih znakova u URL-u ili putu dokumenta

- **Data_SrcDoc_StreamAvailability** – pokazatelj je li niz dokumenata dostupan/onemogućen

- **Data_SrcDoc_SyncBackedType** – pokazatelj vrste dokumenta (lokalni ili na servisu)

- **Data_SrcDoc_UrlHash** – jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta

- **Data_SrcDoc_WopiServiceId** – sadrži jedinstveni identifikator davatelja usluga WOPI

- **Data_SrcDocIsUnnamedOrNew** – označava je li dokument koji spremamo nov


#### <a name="officewordworddocumentdirtyflagchanged"></a>Office.Word.Word.DocumentDirtyFlagChanged

Ovaj događaj označava da Office Word uređuje dokument koji mijenja interno stanje dokumenta u „prljavo”. On Microsoftu omogućuje procjenu stanja značajke uređivanja dokumenta. Taj je događaj impuls korisničkog uređivanja. Koristi se i izračunavanje broja mjesečnih aktivnih korisnika/uređaja.

Prikupljaju se sljedeća polja:

  - **Data\_CollectionTime–** vremenska oznaka događaja

  - **Data\_DocumentLocation–** vrsta mjesta dokumenta

  - **Data\_DocumentLocationDetails–** podvrsta mjesta dokumenta

  - **Data\_FAlwaysSaveEnabled–** označava je li omogućeno spremanje u bilo kojem trenutku

  - **Data\_FirstEditTime–** vremenska oznaka prvog uređivanja

  - **Data\_NumberCoAuthors–** broj koautora koji uređuju dokument tijekom sesije

  - **Data\_NumberOfTimesDocumentDirtied–** broj izmjena u dokumentu

  - **Data\_Pdod–** identifikator dokumenta u sklopu procesa Office Word

  - **Data\_UrlHash–** raspršivanje puta dokumenta

  - **Data\_ViewKind–** vrsta prikaza u programu Word



#### <a name="onenoteappnavigationratingreminderdialogshown"></a>OneNote.App.Navigation.RatingReminderDialogShown

Ključni signal koji se upotrebljava za mjerenje djelotvornosti logike okidača za podsjetnik za ocjenjivanje. Ovaj se dijaloški okvir prikazuje kada korisnik ispuni sve uvjete za prikaz podsjetnika za ocjenjivanje (br. aktivnih dana, prethodno je ocjenjivao ili nije itd.). To se upotrebljava za osiguravanje funkcije logike okidača za podsjetnika za ocjenjivanje. Ako korisnici vide ovaj dijaloški okvir, to će nam pružiti načine za primanje povratnih informacija od korisnika u pravo vrijeme te poboljšanje stanja aplikacije.

Prikupljaju se sljedeća polja:

- Nijedno

#### <a name="parselicenseop"></a>ParseLicenseOp

Prikuplja se kada korisnik pokuša otvoriti dokument zaštićen IRM-om ili primijeniti zaštite IRM-a.  Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada se provodi operacija raščlanjivanja licenca. 

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere

- **AppInfo.Name** – naziv aplikacije

- **AppInfo.Version** – verzija aplikacije

- **iKey** – identifikacijski broj poslužitelja zapisnika

- **RMS.ApplicationScenarioId** – identifikacijski broj scenarija koji pruža aplikacija

- **RMS.Duration** – ukupno vrijeme potrebno za dovršavanje operacije

- **RMS.DurationWithoutExternalOps** – ukupno vrijeme umanjeno za potrošene vanjske operacije poput latencije mreže.

- **RMS.ErrorCode** – kod pogreške koji, ako postoji, vraća operacija

- **RMS.HttpCall** – označava postoji li operacija HTTP-a

- **RMS.LicenseFormat** – format licence: Xrml ili Json

- **RMS.Result** – uspjeh ili neuspjeh operacije

- **RMS.ScenarioId** – identifikacijski broj scenarija koji definira klijent usluge upravljanja pravima

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

- **RMS.ServerType** – vrsta poslužitelja usluge upravljanja pravima 

- **RMS.StatusCode** – kod statusa rezultata operacije

- **RMS.VerifyCertChainDuration** – vrijeme trajanja za provjeru lanca certifikata

- **RMS.VerifySignatureDuration** – vrijeme trajanja za provjeru potpisa

#### <a name="readconversation"></a>read.conversation

Koristi se za nadzor mogućeg negativnog utjecaja na stanje i funkciju prikazivanja poruke e-pošte

Prikupljaju se sljedeća polja: 

- **above_40fps** – broj prikazanih okvira iznad 40 fps
 
- **above_50fps** – broj prikazanih okvira iznad 50 fps
 
- **above_55fps** – broj prikazanih okvira iznad 55 fps

- **adal_id** – ID provjere autentičnosti aktivnog direktorija računa, jedinstveni identifikator u sustavu za provjere autentičnosti tvrtke Microsoft 

- **component_name** – naziv komponente/prikaza koji je aktivan tijekom filtriranja

- **event_mode** – mjesto u aplikaciji na kojem je korisnik ušao u razgovor (grupni ili drugi)

- **internet_message_id** – ID praćenja za najnoviju poruku u razgovoru
      
- **orientation** – orijentacija ekrana u trenutku događaja (okomito ili vodoravno)

- **recent_message_id** – ID najnovije poruke u razgovoru

- **suggested_reply_state** – stanje predloženih odgovora za ovaj razgovor (nedostupno, dostupno, prikazano, korišteno ili odbačeno)

- **suggested_reply_types** – označava vrstu i broj predloženog odgovora prikazanog/korištenog za taj razgovor. To je rječnik. Na primjer, {text: 2, send_avail: 1}.
  
- **total_count** – ukupan broj okvira koji komponenta prikazuje
 
- **view_duration** – koliko je dugo korisnik pregledavao komponentu

#### <a name="saveattempt"></a>save.attempt

Omogućuje utvrđivanje utjecaja problema uzrokovanih korisnicima koji pokušavaju spremiti datoteku procjenom broja zahvaćenih sesija te postoje li zajedničke značajke tih sesija.

Prikupljaju se sljedeća polja: 

- **file_type** – vrsta datoteke koju je korisnik pokušao spremiti (primjerice .doc)

- **origin** – odakle pokušaj spremanja potječe (primjerice iz poruke e-pošte) kako bismo mogli prepoznati probleme u vezi sa spremanjem datoteke s određenog mjesta u aplikaciji

- **token_type** – vrsta tokena korištenog za provjeru autentičnosti radi spremanja datoteka koji nam pomaže prepoznati probleme s provjerom autentičnosti u vezi sa spremanjem datoteke

#### <a name="searchsubtabselected"></a>search.subtab.selected

Događaj prikuplja točke podrijetla za razlog što je odabrana podkartica za pretraživanje. Podkartice se nalaze ispod primarne trake za pretraživanje aplikacije radi filtriranja podataka. Ovaj nam događaj omogućuje praćenje pilula vrste entiteta (sve, pošta, kontakti i kalendar) koje korisnici koriste kada provode pretraživanja kako bismo mogli osigurati da mehanizmi filtara pretraživanja propisno funkcioniraju.

Prikupljaju se sljedeća polja:

- **properties_general** – opća svojstva koja prikupljaju svi događaji Aria

- **selected_reason** – uzrok vrste pilule koja se odabire, a koja može biti jedna od ovih vrijednost (glif je ikona)i: tap_on_header, tap_on_see_all, enter_search_mode, mail_glyph, calendar_glyph.

- **subtab_type** – vrsta pilule koja je odabrana, a koja može biti jedna od ove četiri vrijednosti: sve, pošta, kontakt, događaj.

#### <a name="sendmessage"></a>send.message

Koristi se za nadzor mogućeg negativnog utjecaja na funkciju i stanje slanja poruka e-pošte.

Prikupljaju se sljedeća polja:
  
- **account** – prati račun koji je proveo radnju

- **compose_duration** – prati ukupno vrijeme koje je korisniku bilo potrebno za sastavljanje poruke uključujući sesiju s više skica

- **draft_message_id** – prati ID sastavljanja poruke koja se šalje

- **event_mode** – prati način događaja ako se odnosi na poruku, („grupni” ili „ostalo”)

- **has_attachment** – označava ima li poruka privitke

- **has_mip_label** – označava je li poruka označena oznakom MIP ili nije

- **is_group_escalation** – označava je li ovo eskalirana grupna poruka, „eskalirana poruka” jest poruka koja je poslana u ulaznu poštu korisnika zbog eskalacije (pretplata na grupu)

- **is_groups** – prati je li poslana poruka grupna poruka ili nije

- **key_stroke_count** – prati broj pritisaka tipki za poruku koja se šalje

- **message_id** – prati ID poruke koja se odgovorila/proslijedila

- **origin** – označava gdje je sastavljanje pokrenuto, npr. novo, odgovor, brzi odgovor itd.

- **send_draft_origin** – označava gdje je slanje pokrenuto, tj. sastavljanje ili brzi odgovor

- **smart_compose_model_version** – prati koja se verzija modela pametnog sastavljanja upotrebljava

- **source_inbox** – označava vrstu izvorne ulazne pošte za referentnu poruku, 

- **suggested_reply_state** – utvrđuje predloženo stanje odgovora, tj. nedostupno, dostupno, prikazano, korišteno ili odbačeno za ovu poslanu poštu

- **suggested_reply_types** – označava vrstu i broj predloženog odgovora prikazanog/korištenog za tu poslanu poruku e-pošte. To je rječnik. Na primjer, {text: 2, send_avail: 1}.

- **suggestions_requested** – označava koliko ste modela pametnog sastavljanja tražili

- **suggestions_results** – rezultat prijedloga pametnog sastavljanja, tj. prihvaćeno, odbijeno

- **suggestions_returned** – označava koliko je prijedloga pametnog sastavljanja vraćeno s poslužitelja

- **suggestions_shown** – označava koliko je prijedloga pametnog sastavljanja prikazano korisniku

- **thread_id** – označava ID niti razgovora na koji se odgovara/prosljeđuje

#### <a name="session"></a>session

Omogućuje nam prepoznavanje i rješavanje situacija u kojima se vaša baterija previše troši te nam pomaže utvrditi što bi mogao biti uzrok.

Prikupljaju se sljedeća polja: 

- **battery_level** – govori nam razinu napunjenosti baterije uređaja kako bi nam pomogao prepoznati kada naša aplikacija ima negativan utjecaj na razinu napunjenosti baterije vašeg uređaja

- **has_hx** – govori nam da račun koristi naš novi servis sinkronizacije kako bi nam pomogao prepoznati probleme uzrokovane našim servisom sinkronizacije

- **Session.Duration** – duljina sesije u sekundama

- **Session.DurationBucket** – vremensko razdoblje dužine trajanja *[Ovo je polje uklonjeno iz trenutnih verzija sustava Office, ali se i dalje može pojaviti u starijim verzijama.]*

- **Session.FirstLaunchTime** – prvo snimljeno vrijeme pokretanja aplikacije *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

- **Session.State** – pokazatelj je li to početak ili kraj sesije

#### <a name="settingsaction"></a>settings.action

Ovaj događaj prikuplja informacije o konfiguraciji u postavkama. Podaci nam omogućuju prepoznavanje situacija u kojima može doći do negativnog utjecaja na sposobnost korisnika za konfiguriranje postavki aplikacije, primjerice postavki obavijesti, primarnog računa pošte i konfiguriranja potpisa e-pošte.

Prikupljaju se sljedeća polja: 

- **account_order_changed** – da biste provjerili jeste li promijenili redoslijed računa kako biste osigurali da ova konfiguracija pravilno funkcionira 

- **action** – moguće radnje provedene u postavkama, primjerice brisanje računa kako bi nam pomogao dijagnosticirati probleme i osigurati da nema negativnog utjecaja

- **auth_type** – vrsta provjere autentičnosti koju račun koristi kako bismo mogli razumjeti koji sloj sinkronizacije u pozadini koristimo kako bismo mogli dijagnosticirati probleme 

- **changed_folder** – utvrđuje je li mapa promijenjena kako bi nam pomogao dijagnosticirati probleme. 

- **delete_scope** – tijekom brisanja računa, jeste li izbrisali račun s ovog uređaja ili sa svih uređaja s programom Outlook.  

- **enabled_state** – utvrđuje jesu li vaše postavke za automatski odgovor, spremanje kontakata i blokiranje vanjskih slika ispravno konfigurirane  

- **notification_action** – služi provjeri jeste li konfigurirali ikakve radnje obavijesti za razvrstavanje poruka e-pošte kako bismo mogli provjeriti funkcionira li ova postavka ispravno 

- **notification_action_number** – da biste provjerili jesu li radnje obavijesti (radnja jedan ili radnja dva) ispravno konfigurirane

- **server_type** – slično događaju auth_type, govori nam koju vrstu računa imate kako bi nam pomogao u boljem dijagnosticiranju problema.  Primjeri: Office365, Gmail, Outlook

- **setting_properties** – prati odnos svojstava prema radnji postavljanja detaljno u nastavku: 
   - **alternate_app_icon_setting** – odabrana ikona zamjenske aplikacije (svijetla, tamna)
   - **auth_type** – označava vrstu provjere autentičnosti u pozadini koja nam omogućava da saznamo postoji li problem s određenom vrstom računa
   - **badge_count_state** – označava koju vrstu broja znački je korisnik tražio, odnosno nema znački, samo fokusirana poštanska pošta itd. 
   - **changed_folder** – utvrđuje je li ova radnja bila arhivirana, zakazana ili je postojala druga radnja.
   - **delete_scope** – prati je li ova radnja bila povezana s brisanjem nekoga samo na ovom uređaju ili na svim uređajima, ako je primjenjivo. 
  - **enabled_state** – utvrđuje je li stanje povezano s radnjom omogućeno
  - **in_app_language** – odabrani jezik u aplikaciji, vrsta niza (zadano, en-US, fa, ru itd.)
  - **notification_action_setting** – označava pojedinosti o, ako je primjenjivo, postavkama radnje obavijesti povezanim s ovom radnjom
    - **notification_action** – označava što je korisnik pokušavao učiniti, odnosno, označiti zastavicom, izbrisati, arhivirati, omogućuje nam utvrditi koju radnju poruke je korisnik želio izvršiti na obavijesti te je li radnja bila neuspješna ili ne. 
    - **notification_action_number** – označava kojem je broju radnji (dvije od tri radnje su prilagodljive) dodijeljena radnja obavijesti, odnosno, radnja jedan, radnja dva. To nam omogućuje utvrditi postoji li problem s određenom radnjom.
   - **notification_state** – označava koju je vrstu značke korisnik zatražio, tj. nema značke, samo za fokusiranu ulaznu poštu itd.
   - **server_type** – označava vrstu poslužitelja u pozadini koja nam omogućava da saznamo postoji li problem s određenom vrstom poslužitelja
   - **source** – označava koji je izvor obavijesti, ako je primjenjivo, iz postavki ili postavke ne ometaj
   - **swipe_setting** – označava pojedinosti o, ako je primjenjivo, postavkama prelaska prstom povezanim s ovom radnjom
     - **swipe_action** – označava što je korisnik pokušavao učiniti, odnosno, označiti zastavicom, izbrisati, arhivirati, omogućuje nam utvrditi koju je radnju korisnik želio provesti te je li radnja bila neuspješna ili nije. 
     - **swipe_direction** – označava za koji je smjer korisnik postavio prelazak prstom, tj. slijeva udesno ili zdesna ulijevo. To nam omogućuje utvrditi postoji li problem s određenim smjerom prelaska prstom.
   - **temperature_unit_setting** – odabrana jedinica temperature koja će se upotrebljavati za vrijeme 
   - **theme_color_setting** – prilagođena tematska boja aplikacije koju je odabrao korisnik 
   - **ui_mode_setting** – odabrani način korisničkog sučelja (tamno, svijetlo, zadane postavke sustava, niska razina baterije, itd.)
   - **signature_setting** – označava je li postavka bila primijenjena na sve račune ili na pojedini račun

- **state_changed_to** – služi provjeri je li vaša postavka uključivanja/isključivanja fokusirane ulazne pošte pravilno konfigurirana 

- **swipe_action** – služi provjeri jeste li konfigurirali ikakve radnje prelaska prstom za razvrstavanje poruka e-pošte kako bismo mogli provjeriti funkcionira li ova postavka ispravno 

- **swipe_direction** – služi provjeri jesu li vaši smjerovi prelaska prstom (ulijevo ili udesno) ispravno konfigurirani


#### <a name="sidebaraction"></a>sidebar.action

Omogućuje nam prepoznavanje situacija u kojima može doći do negativnog utjecaja na vašu mogućnost konfiguriranja postavki aplikacije, primjerice vaših postavki obavijesti, vašeg primarnog računa pošte i konfiguriranja vašeg potpisa e-pošte.

Polja podataka koja su uobičajena za Outlook Mobile za ovaj događaj na operacijskim sustavima iOS i Android:

- **Account** – prati račun i njegove podatke povezane s događajem, vrijednosti praćene u okviru ovih podataka nalaze se u polju zajedničke dokumentacije *[Ovo je polje uklonjeno iz trenutnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

- **action** – prati vrstu provedene radnje bočne trake, tj. odbačeno, odabir gumba za pomoć, bočna traka pošte itd., 

- **from_favorites** – prati potječe li radnja iz stavke ili iz favorita 

- **mail_folder_type** – vrsta mape koja je odabrana tijekom radnje bočne trake, ako postoji.

- **sidebar_type** – prati vrstu bočne trake povezane s ovim događajem, odnosno, pošta ili kalendar, kako bi nam pomogao osigurati da navigacija iz postavke favorita pravilno funkcionira

Prikupljaju se sljedeća polja: 

- **account_type** – označava koju vrstu provjere autentičnosti račun ima, tj. Gmail, Outlook itd. 

- **account_has_groups** – pomaže nam provjeriti ima li račun grupe te jesu li one ispravno konfigurirane

- **calendar_accounts_count** – broj računa kalendara koje imate kako bismo mogli osigurati da su računi kalendara ispravno konfigurirani 

- **calendar_apps_count** – broj aplikacija kalendara koje imate kako bismo mogli osigurati da su vaše aplikacije zanimljivih kalendara ispravno konfigurirani 

- **calendar_type** – vrsta kalendara koji imate (primarni kalendar, grupni kalendar itd.) 

- **has_favorite_folders** – pomaže nam osigurati pravilan način konfiguriranja omiljenih mapa 

- **has_favorite_people** – pomaže nam osigurati pravilan način konfiguriranja omiljenih osoba/kontakata 

- **has_group_calendar** – pomaže nam osigurati pravilan način konfiguriranja grupnih kalendara ako ih imate 

- **has_group_calendar_account** – pomaže nam osigurati pravilan način konfiguriranja grupnih kalendara ako ih imate 

- **has_group_toggled** – pomaže nam osigurati pravilan način konfiguriranja postavki uključenih/isključenih grupnih kalendara 

- **interesting_calendars_accounts_count** – broj računa zanimljivih kalendara koje imate kako bismo mogli osigurati da su računi zanimljivih kalendara ispravno konfigurirani 

- **mail_accounts_count** – ukupan broj računa pošte na bočnoj traci kako bismo osigurali da je to ispravno konfigurirano 

- **mail_folder_type** – vrsta mape koju je korisnik dodirnuo kako bismo osigurali da je ispravno konfigurirana. To može uključivati Izbrisanu mapu, Neželjenu poštu ili vašu mapu Poslana pošta. 

- **mail_inbox_unread_count** – pomaže nam osigurati da je količina nepročitanih poruka prikazana i ispravno konfigurirana 

- **mail_subfolder_depth** – pomaže nam osigurati da možemo uspješno prikazivati konfiguracije korisnikove podmape pošte

#### <a name="storeop"></a>StoreOp

Prikuplja se kada korisnik pokuša otvoriti dokument zaštićen IRM-om ili primijeniti zaštite IRM-a.  Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada se provodi operacija pohranjivanja licence usluge upravljanja pravima. 

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere

- **AppInfo.Name** – naziv aplikacije.

- **AppInfo.Version** – verzija aplikacije

- **iKey** – identifikacijski broj poslužitelja pružatelja usluge zapisivanja

- **RMS.ApplicationScenarioId** – identifikacijski broj scenarija koji pruža aplikacija

- **RMS.ContentId** – identifikacijski broj sadržaja u licenci krajnjeg korisnika

- **RMS.Duration** – ukupno vrijeme potrebno za dovršavanje poziva API-ja

- **RMS.DurationWithoutExternalOps** – ukupno vrijeme umanjeno za potrošene vanjske operacije poput latencije mreže.

- **RMS.ErrorCode** – kod pogreške koji, ako postoji, vraća operacija

- **RMS.HttpCall** – označava postoji li operacija HTTP-a

- **RMS.LicenseFormat** – format licence: Xrml ili Json

- **RMS.OperationName** – naziv operacije

- **RMS.Result** – uspjeh ili neuspjeh operacije

- **RMS.ScenarioId** – identifikacijski broj scenarija koji definira klijent usluge upravljanja pravima

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

- **RMS.ServerType** – vrsta poslužitelja usluge upravljanja pravima 

- **RMS.StatusCode** – kod statusa rezultata operacije

- **RMS.Url** – URL poslužitelja usluge upravljanja pravima

#### <a name="watchappv2"></a>watchAppV2

Ovaj nam događa omogućuje otkrivanje i rješavanje mogućih problema s mogućnostima na uređaju Apple Watch kao što su primanje obavijesti i odgovaranje na poruke e-pošte.

Prikupljaju se sljedeća polja: 

- **app_action** – govori nam vrste radnji koje je korisnik proveo na uređaju Apple Watch, primjerice „archive_message”, kako bi nam pomogao prepoznati probleme u vezi s određenom radnjom, primjerice nemogućnost uspješnog arhiviranja poruka na uređaju Apple Watch

- **is_watch_app_installed** – govori nam je li korisnik instalirao našu aplikaciju Apple Watch na svom uređaju

- **is_complication_enabled** – govori nam je li korisnik dodao program Outlook na ekran uređaja Apple Watch kako bismo mogli prepoznati probleme u vezi s ekranima uređaja Apple Watch

- **watch_os** – govori nam verziju operacijskog sustava uređaja Apple Watch koja je instalirana kako bismo mogli prepoznati probleme u vezi s određenim verzijama operacijskog sustava uređaja Apple Watch


### <a name="application-status-and-boot-subtype"></a>*Podvrsta stanja i pokretanja aplikacije*

Utvrđivanje je li došlo do određenih događaja povezanih sa značajkama, poput pokretanja ili zaustavljanja, te je li značajka pokrenuta.

#### <a name="appstartup"></a>app.startup

Ovaj nam događaj omogućava prepoznavanje i popravljanje problema kada se Outlook pokreće sporo ili nepotpuno, zbog čega korisnici imaju probleme s korištenjem naše aplikacije.  To uključuje informacije o konkretnim značajkama koje su bile omogućene i koliko su dugo dijelovi pokretanja trajali.

Prikupljaju se sljedeća polja: 

- **attach_base_context_millis** – vrijeme između početka osnovnog konteksta i stavke onCreate()

- **device_ram_in_mb** – količina RAM-a dostupna na uređaju

- **has_company_portal** – je li instalirana aplikacija portala tvrtke

- **hx_okhttp_mode** – koristi li nova komponenta servisa sinkronizacije poruka e-pošte OKHttp za slanje i primanje mrežnih zahtjeva koji se temelje na HTTP-u

- **initial_activity_name** – aktivnost sustava Android koja je pokrenula aplikaciju

- **manufacturer** – proizvođač uređaja

- **model** – model uređaja

- **on_create_millis** – vrijeme koje je proteklo za metodu onCreate()

- **on_resume_millis** – vrijeme koje je proteklo za metodu onResume()

- **time_until_attach** – vrijeme koje je proteklo između učitavanja razreda i pokretanja osnovnog konteksta

- **total_millis** – ukupno vrijeme od početka učitavanja razreda do dovršavanja nastavka aktivnosti sustava Android

#### <a name="boottime"></a>boot.time 

Ovaj nam događaj omogućuje otkrivanje kada su nastupile kritične pogreške aplikacije koje bi uzrokovale rušenje vaše aplikacije ili iskustvo ozbiljnih problema, primjerice prikaz praznih redaka u vašoj ulaznoj pošti. Ovaj događaj prikuplja informacije koje nam omogućuju kategorizaciju i razvrstavanje problema kako bismo mogli odrediti prioritet utjecaja problema na korisnike.

Prikupljaju se sljedeća polja:

- **black_list_reason** – govori nam postoji li razlog zašto bismo trebali zanemariti ove podatke. Pojedini primjeri uključuju pokretanje zbog udaljene obavijesti i pokretanje zbog pozadinskog dohvaćanja.

- **step_premain** – govori nam koliko je vremena bilo potrebno da Outlook nakon korisnikovog dodirivanja ikone prijeđe na step0_main, "glavni" korak definiran u ovom dokumentu.

- **step0_main** – govori nam koliko je vremena bilo potrebno da Outlook dospije do koraka „main”, što je korak koji je odredila tvrtka Apple.

- **step1_appWillFinishLaunching** – govori nam koliko je vremena bilo potrebno da Outlook dospije od koraka „main” do koraka „appWillFinishLaunching”, što je korak koji je odredila tvrtka Apple.

- **step2_appDidFinishLaunching** – govori nam koliko je vremena bilo potrebno da Outlook dospije od koraka „appWillFinishLaunching” do koraka „appDidFinishLaunching”, što je korak koji je odredila tvrtka Apple.

- **step3_engineStarted** – govori nam koliko je vremena potrebno da Outlook dospije od koraka „appDidFinishLaunching” do pokretanja modula aplikacije, koji upravlja spremanjem i sinkronizacijom podataka.

- **step4_runLoopFirstIdle** – govori nam koliko je vremena bilo potrebno da Outlook dospije od koraka „engineStarted” do faze bez potrebe za dovršavanjem dodatnih zadataka.

- **total_time** – govori nam koliko je vremena bilo potrebno da Outlook dovrši proces pokretanja.

#### <a name="dnslookupop"></a>DnsLookupOp

Prikuplja se kada korisnik pokuša otvoriti dokument zaštićen IRM-om ili primijeniti zaštite IRM-a.  Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada se provodi operacija pretraživanja DNS podataka. 

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere

- **AppInfo.Name** – naziv aplikacije.

- **AppInfo.Version** – verzija aplikacije

- **iKey** – identifikacijski broj poslužitelja pružatelja usluge zapisivanja

- **RMS.ApplicationScenarioId** – identifikacijski broj scenarija koji pruža aplikacija

- **RMS.Duration** – ukupno vrijeme potrebno za dovršavanje operacije

- **RMS.DurationWithoutExternalOps** – ukupno vrijeme umanjeno za potrošene vanjske operacije poput latencije mreže.

- **RMS.ErrorCode** – kod pogreške koji, ako postoji, vraća operacija

- **RMS.HttpCall** – označava postoji li operacija HTTP-a

- **RMS.LicenseFormat** – format licence: Xrml ili Json

- **RMS.NoOfDomainsSearched** – broj pretraženih domena    

- **RMS.NoOfDomainsSkipped** – broj preskočenih domena 

- **RMS.Result** – uspjeh ili neuspjeh operacije

- **RMS.ScenarioId** – identifikacijski broj scenarija koji definira klijent usluge upravljanja pravima

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

- **RMS.ServerType** – vrsta poslužitelja usluge upravljanja pravima 

- **RMS.StatusCode** – kod statusa rezultata operacije

#### <a name="firstvisible"></a>first.visible

Ovaj nam događaj omogućuje prepoznavanje prvog puta kada korisnik namjerno pokrene aplikaciju. Ovaj je događaj obavezan za osiguravanje da aplikacija uspješno radi u međuverzijama originalnog proizvođača opreme (OEM).

Prikupljaju se sljedeća polja:

- **is_oem** – praćenje polja koje označava je li aplikacija pokrenuta na varijanti OEM-a

- **is_system_install** – polje koje prati prisutnost prethodno instalirane datoteke svojstava koja treba označavati da je ta instalacija OEM 

- **manufacturer** – proizvođač uređaja

- **model** – model uređaja

- **systemFlagSet** – vrijednost zastavice sustava Android (ApplicationInfo.FLAG_SYSTEM) koja označava je li aplikacija bila instalirana kao dio slike sustava uređaja

#### <a name="getuserop"></a>GetUserOp

Prikuplja se kada korisnik pokuša otvoriti dokument zaštićen IRM-om ili primijeniti zaštite IRM-a.  Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada se provodi operacija dobivanja korisničkih certifikata. 

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere

- **AppInfo.Name** – naziv aplikacije

- **AppInfo.Version** – verzija aplikacije

- **iKey** – identifikacijski broj poslužitelja pružatelja usluge zapisivanja

- **RMS.ApplicationScenarioId** – identifikacijski broj scenarija koji pruža aplikacija

- **RMS.ContentId** – identifikacijski broj sadržaja

- **RMS.Duration** – ukupno vrijeme potrebno za dovršavanje operacije

- **RMS.DurationWithoutExternalOps** – ukupno vrijeme umanjeno za potrošene vanjske operacije poput latencije mreže.

- **RMS.ErrorCode** – kod pogreške koji vraća operacija

- **RMS.HttpCall** – označava postoji li operacija HTTP-a

- **RMS.LicenseFormat** – format licence: Xrml ili Json

- **RMS.Result** – uspjeh ili neuspjeh operacije

- **RMS.ScenarioId** – identifikacijski broj scenarija koji definira klijent usluge upravljanja pravima

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

- **RMS.ServerType** – vrsta poslužitelja usluge upravljanja pravima 

- **RMS.StatusCode** – kod statusa rezultata operacije

- **RMS.Type** – vrsta informacija o korisniku

#### <a name="httpop"></a>HttpOp

Prikuplja se kada korisnik pokuša otvoriti dokument zaštićen IRM-om ili primijeniti zaštite IRM-a.  Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada se provodi operacija zahtjeva HTTP-a.

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere
    
- **AppInfo.Name** – naziv aplikacije

- **AppInfo.Version** – verzija aplikacije

- **iKey** – identifikacijski broj poslužitelja pružatelja usluge zapisivanja

- **RMS.ApplicationScenarioId** – identifikacijski broj scenarija koji pruža aplikacija

- **RMS.CallBackStatus** – status vraćenog rezultata povratnog poziva za provjeru autentičnosti

- **RMS.CallbackTime** – vrijeme koje je utrošio povratni poziv za provjeru autentičnosti 

- **RMS.CorrelationId** – ID korelacijskog zahtjeva HTTP-a

- **RMS.DataSize** – veličina podataka zahtjeva HTTP-a

- **RMS.Duration** – ukupno vrijeme potrebno za dovršavanje operacije

- **RMS.DurationWithoutExternalOps** – ukupno vrijeme umanjeno za potrošene vanjske operacije poput latencije mreže.

- **RMS.ErrorCode** – kod pogreške koji, ako postoji, vraća operacija

- **RMS.HttpCall** – označava postoji li ugniježđena operacija HTTP-a 

- **RMS.LicenseFormat** – format licence: Xrml ili Json

- **RMS.OperationName** – naziv operacije

- **RMS.Result** – uspjeh ili neuspjeh operacije

- **RMS.ScenarioId** – identifikacijski broj scenarija koji definira klijent usluge upravljanja pravima

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

- **RMS.ServerType** – vrsta poslužitelja usluge upravljanja pravima 

- **RMS.StatusCode** – kod statusa rezultata operacije

- **RMS.Url** – URL poslužitelja usluge upravljanja pravima

- **RMS.WinhttpCallbackStatus** – status rezultata povratnog poziva WinHTTP-a

#### <a name="initialized"></a>Initialized

Omogućuje nam analizu stanja sučelja koje omogućuje da mobilne aplikacije dohvaćaju postavke sigurnosti i zaštite privatnosti iz usluga programa Office te dijagnozu problema sa servisom postavki povezivanja i zaštite privatnosti.

Prikupljaju se sljedeća polja:

- **roamingSettingType** – označava mjesto s kojeg smo pokušali čitati postavke

#### <a name="ipccreateoauth2token"></a>IpcCreateOauth2Token

Prikuplja se kada korisnik pokuša otvoriti dokument zaštićen IRM-om ili primijeniti zaštite IRM-a. Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada se stvori IpcCreateOauth2Token poziv API-ja.

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere
    
- **AppInfo.Name** – naziv aplikacije.

- **AppInfo.Version** – verzija aplikacije

- **iKey** – identifikacijski broj poslužitelja pružatelja usluge zapisivanja

- **RMS.Duration** – ukupno vrijeme potrebno za dovršavanje poziva API-ja

- **RMS.DurationWithoutExternalOps** – ukupno vrijeme umanjeno za potrošene vanjske operacije poput latencije mreže.

- **RMS.ErrorCode** – kod pogreške koji, ako postoji, vraća poziv API-ja

- **RMS.HttpCall** – označava postoji li operacija HTTP-a

- **RMS.Result** – uspjeh ili neuspjeh poziva API-ja

- **RMS.ScenarioId** – identifikacijski broj scenarija definiran API-jem

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

- **RMS.StatusCode** – kod statusa vraćenog rezultata


#### <a name="officeandroidaccountstorageinfo"></a>Office.Android.AccountStorageInfo

Tim se događajem određuje broj računa MSA i ADAL u registru i zajedničkim postavkama. Omogućuje analizu nedosljednosti među spremištima podataka i omogućuje stabiliziranje performansi aplikacija.

Prikupljaju se sljedeća polja:

- **RegistryADALCount** – upućuje na broj računa ADAL u registru.

- **RegistryLiveIdCount** – upućuje na broj računa MSA u registru.

- **SharedPrefADALCount** – upućuje na broj računa ADAL u zajedničkim postavkama.

- **SharedPrefLiveIdCount** – upućuje na broj računa MSA u zajedničkim postavkama.


#### <a name="officeandroidandroidoffice16bootlatency"></a>Office.Android.AndroidOffice16BootLatency

Ključno je za snimanje metrike performansi aplikacije s obzirom na vrijeme odaziva aplikacije prilikom pokretanja.  Microsoft to upotrebljava za prikupljanje vremena potrebnog za reagiranje aplikacije i otkrivanje scenarija koji mogu utjecati na vrijeme pokretanja u aplikacijama Word, Excel ili PowerPoint.

Prikupljaju se sljedeća polja:

- **AppLaunchResponsiveTimeInMilliSec** – vrijeme pokretanja aplikacije

- **AppSuspendedDuringBoot** – Booleova vrijednost koja označava je li aplikacija obustavljena tijekom pokretanja

- **CollectionTime** – vrijeme događaja

- **FileActivationAttempted** – Booleova vrijednost koja označava je li pokušana aktivacije datoteke

- **FirstIdleOnAppThreadTimeInMilliSec** – vrijeme neaktivnosti niti aplikacije

- **IsThisFirstLaunch** – Booleova vrijednost koja označava je li ovo prvo pokretanje aplikacije

- **UserDialogInterruptionDuringBoot** – Booleova vrijednost koja označava je li blokiralo korisničko sučelje tijekom pokretanja

#### <a name="officeextensibilityofficejsappactivated"></a>Office.Extensibility.OfficeJS.Appactivated

Bilježi informacije o neočekivanim isključivanjima sustava Office. To nam omogućuje prepoznavanje rušenja ili blokiranja proizvoda kako bismo na njih mogli reagirati.

Prikupljaju se sljedeća polja:

  - **Data\_AirspaceInitTime:integer–** trajanje inicijalizacije komponente Airspace za Office

  - **Data\_AllShapes:integer –** broj oblika u dokumentu

  - **Data\_APIInitTime:integer –** trajanje inicijalizacije API modula za Visio

  - **Data\_AppSizeHeight –** visina prozora dodatka **-**

  - **Data\_AppSizeWidth –** širina prozora dodatka **-**

  - **Data\_AppURL –** URL dodatka; bilježi puni URL za dodatke iz trgovine i domenu URL-a za dodatke koji nisu iz trgovine

  - **Data_Doc_AsyncOpenKind:long –** označava je li otvorena predmemorirana verzija dokumenta u oblaku i koja je logika za asinkrono osvježavanje korištena.

  - **Data\_AuthorsCount:integer –** broj autora koji su uređivali dokument u toj sesiji

  - **Data\_BackgroundPages:integer –** broj pozadinskih stranica u dijagramu

  - **Data\_BootTime:integer –** trajanje pokretanja programa Visio

  - **Data\_Browser –** niz preglednika s informacijama o pregledniku kao što su vrsta i verzija

  - **Data\_ChildWindowMixedModeTime:integer –** trajanje omogućavanja mješovitog načina rada u programu Visio (podređeni prozor može imati drukčije svojstvo DpiAwareness od nadređenog)

  - **Data\_CommentsCount:integer –** broj komentara u dokumentu

  - **Data\_ConnectionCount:integer –** broj podatkovnih veza u dijagramu

  - **Data\_ContentMgrInitTim:integer –** trajanje inicijalizacije upravitelja sadržaja

  - **Data\_CreateMainFrameTime:integer –** vrijeme stvaranja glavnog okvira

  - **Data\_CreatePaletteTime:integer –** trajanje stvaranja globalne palete boja

  - **Data\_DispFormatCount:integer –** broj podatkovnih grafika u dijagramu

  - **Data\_Doc\_Ext:string –** nastavak dokumenta

  - **Data\_Doc\_Fqdn:string –** mjesto pohrane dokumenta (SharePoint.com, live.net), dostupno samo za domene sustava Office 365

  - **Data\_Doc\_FqdnHash:string –** raspršivanje mjesta pohrane dokumenta

  - **Data\_Doc\_IsIncrementalOpen:bool–** : je li dokument otvoren inkrementalno (nova značajka koja otvara dokument bez potrebe za preuzimanjem cijelog dokumenta)

  - **Data\_Doc\_IsOpeningOfflineCopy:bool –** otvara li se dokument iz lokalne predmemorije?

  - **Data\_Doc\_IsSyncBacked:bool–** istinito kad je riječ o poslužiteljskom dokumentu koji postoji lokalno te se sinkronizira s poslužiteljem (na primjer, putem servisa OneDrive ili ODB klijentskih aplikacija)

  - **Data\_Doc\_Location:long–** : unaprijed definiran skup vrijednosti mjesta na kojima se dokument pohranjuje (lokalno, SharePoint, WOPI, mreža itd.)

  - **Data\_Doc\_LocationDetails:long –** unaprijed definiran skup vrijednosti detaljnijih lokacija (mapa Temp, mapa preuzimanja, dokumenti servisa One Drive, slike servisa One Drive)

  - **Data\_Doc\_ResourceIdHash:string –** raspršivanje identifikatora resursa za dokumente pohranjene u oblaku

  - **Data_Doc_RtcType –** označava kako je kanal u stvarnom vremenu (RTC) postavljen za trenutnu datoteku (onemogućen, nepodržan, na zahtjev, uvijek uključen itd.).

  - **Data\_Doc\_ServerDocId:string –** nepromjenjivi identifikator za dokumente pohranjene u oblaku

  - **Data\_Doc\_SessionId:long –** generirani GUID koji identificira instancu dokumenta u sklopu iste sesije procesa

  - **Data\_Doc\_SizeInBytes:long –** veličina dokumenta u bajtovima

  - **Data\_Doc\_SpecialChars:long –** dugačka bit-maska koja pokazuje posebne znakove u URL-u ili putu dokumenta

  - **Data\_Doc\_SyncBackedType –** pokazatelj vrste dokumenta (lokalni ili na servisu) 

  - **Data\_Doc\_UrlHash:string –** raspršivanje punog URL-a dokumenata pohranjenih u oblaku

  - **Data\_DpiAwarenessTime:integer –** trajanje omogućivanja svjesnosti o razlučivosti po monitoru

  - **Data\_DurationToCompleteInMilliseconds:double–** trajanje spremanja u milisekundama

  - **Data\_ErrorCode:int –** 0 za uspjelo, a cijeli broj za neuspjelo spremanje

  - **Data\_FailureReason:integer –** razlog neuspjeha za asinkrono spremanje

  - **Data\_FileExtension –** datotečni nastavak otvorenog dijagrama

  - **Data\_FileHasDGMaster:bool –** istinito kada datoteka sadrži podatkovne grafike

  - **Data\_FileHasImportedData:bool –** istinito kada datoteka sadrži uvezene podatke

  - **Data\_FileHasShapesLinked:bool –** istinito kada datoteka sadrži oblike povezane s podacima

  - **Data\_FileIOBytesRead:int –** ukupan broj bajtova pročitanih prilikom spremanja

  - **Data\_FileIOBytesReadSquared:int –** kvadrat vrijednosti Data\_FileIOBytesRead

  - **Data\_FileIOBytesWritten:int –** ukupan broj bajtova zapisanih prilikom spremanja

  - **Data\_FileIOBytesWrittenSquared:int–** kvadrat vrijednosti Data\_FileIOBytesWritten

  - **Data\_FilePathHash:binary** – binarno raspršivanje puta datoteke

  - **Data\_FilePathHash:binary** – GUID puta datoteke

  - **Data\_FileSize –** veličina dokumenta u bajtovima

  - **Data\_ForegroundPages:integer –** broj stranica u prvom planu u dijagramu

  - **Data\_ForegroundShapes:integer –** cijeli broj oblika na stranicama u prvom planu

  - **Data\_GdiInitTime:integer –** trajanje inicijalizacije GDI modula

  - **Data\_HasCoauthUserEdit:bool –** istinito ako se dokument uređivao u sesiji suautorstva

  - **Data\_HasCustomPages:bool –** istinito ako dokument sadrži prilagođene stranice

  - **Data\_HasCustPatterns:bool –** istinito ako datoteka sadrži prilagođene uzorke

  - **Data\_HasDynConn:bool –** istinito ako dokument sadrži dinamičku vezu

  - **Data\_HasScaledPages:bool –** istinito ako dokument sadrži skalirane stranice

  - **Data\_HasUserWaitTime:bool –** istinito kada se prilikom spremanja prikaže dijaloški okvir

  - **Data\_InitAddinsTime:integer –** trajanje inicijalizacije i učitavanja dodatka za COM

  - **Data\_InitBrandTime:integer –** trajanje inicijalizacije pozdravnog zaslona i komponenti sustava Office za brendiranje

  - **Data\_InitGimmeTime:integer –** trajanje inicijalizacije komponente sustava Office

  - **Data\_InitLicensingTime:integer –** trajanje inicijalizacije komponente za licenciranje sustava Office

  - **Data\_InitMsoUtilsTime:integer –** trajanje inicijalizacije za MSOUTILS komponentu sustava Office

  - **Data\_InitPerfTime:integer –** trajanje inicijalizacije komponente sustava Office za performanse

  - **Data\_InitTCOTime:integer –** trajanje inicijalizacije upravitelja komponenti sustava Office

  - **Data\_InitTrustCenterTime:integer –** trajanje inicijalizacije komponente centra za pouzdanost sustava Office

  - **Data\_InitVSSubSystemsTime:integer –** trajanje inicijalizacije komponenti programa Visio

  - **Data\_InternalFile:bool –** istinito ako je datoteka interna datoteka. Na primjer, Šablona

  - **Data\_IsAsyncSave:bool –** istinito ako je spremanje bilo asinkrono

  - **Data\_IsAutoRecoveredFile:bool –** istinito ako je datoteka bila automatski oporavljena

  - **Data\_IsEmbedded:bool –** istinito ako je datoteka programa Visio bila ugrađena u nekoj drugoj aplikaciji

  - **Data\_IsInfinitePageDisabledForAllPages:bool –** ako je beskonačna stranica onemogućena za sve stranice dokumenta

  - **Data\_IsIRMProtected:bool –** istinito ako je datoteka zaštićena pravima na informacije

  - **Data\_IsLocal:bool –** istinito ako je datoteka lokalna

  - **Data\_IsRecoverySave:bool –** istinito ako je spremanje aktivirano zbog oporavka

  - **Data\_IsShapeSearchPaneHiddenState:bool –** istinito ako je okno za pretraživanje oblika bilo sakriveno za dokument

  - **Data\_IsSmartDiagramPresentInActivePageOfFile:bool –** Booleova vrijednost, istinito ako je vizualni dijagram pametnih podataka prisutan na aktivnoj stranici datoteke

  - **Data\_IsSmartDiagramPresentInFile:bool –** Booleova vrijednost, istinito ako je vizualni dijagram pametnih podataka prisutan u datoteci.

  - **Data\_IsUNC:bool –** istinito ako se put dokumenta pridržava konvencije o univerzalnom imenovanju

  - **Data\_LandscapePgCount:integer –** broj stranica s vodoravnim usmjerenjem u dijagramu

  - **Data\_Layers:integer –** broj slojeva u dijagramu

  - **Data\_LoadProfileTime:integer –** trajanje učitavanja alata za profiliranje u sustavu Office

  - **Data\_LoadRichEditTim:integer–** trajanje učitavanja komponente za obogaćeno uređivanje

  - **Data\_LoadVisIntlTime:integer –** trajanje učitavanja međunarodnog DLL-a za Visio

  - **Data\_Location:integer –** lokacija s koje je datoteka otvorena: 0 lokalno, 1, mreža, 2, SharePoint, 3 – web

  - **Data\_MasterCount:integer –** broj matrica u dijagramu

  - **Data\_MaxCoauthUsers:integer –** maksimalan broj suautora koji u bilo kojem trenutku surađuju na datotečnom sustavu, registru, prvoj strani, SDX-u sesije

  - **Data\_MaxTilesAutoSizeOn:integer –** maksimalan broj pločica stranice za koju je omogućena automatska veličina

  - **Data\_MsoBeginBootTime:integer –** trajanje pokretanja MSO-a

  - **Data\_MsoDllLoadTime:integer –** trajanje učitavanja MSO DLL-a

  - **Data\_MsoEndBootTime:integer –** trajanje zatvaranja MSO DLL-a

  - **Data\_MsoInitCoreTime:integer –** trajanje inicijalizacije MSO komponente sustava Office

  - **Data\_MsoInitUITime:integer –** trajanje inicijalizacije korisničkog sučelja MSO komponente sustava Office

  - **Data\_MsoMigrateTime:integer –** trajanje migriranja korisničkih postavki prilikom prvog pokretanja ako je korisnik proveo nadogradnju s prethodne verzije

  - **Data\_NetworkIOBytesRead:int –** ukupan broj mrežnih bajtova pročitanih prilikom spremanja

  - **Data\_NetworkIOBytesReadSquared:int –** kvadrat vrijednosti Data\_NetworkIOBytesRead

  - **Data\_NetworkIOBytesWritten:int –** ukupan broj mrežnih bajtova zapisanih prilikom spremanja

  - **Data\_NetworkIOBytesWrittenSquared :int–** kvadrat vrijednosti NetworkIOBytesWritten

  - **Data\_OartStartupTime:integer –** trajanje inicijalizacije OART komponente sustava Office

  - **Data\_OleInitTime:integer –** trajanje inicijalizacije OLE komponente sustava Office

  - **Data\_OpenDurationTimeInMs:integer –** trajanje otvaranja datoteke u milisekundama

  - **Data\_OriginatedFromTemplateID:integer –** identifikator za predložak iz kojeg je dijagram stvoren. NULL za predloške drugih proizvođača

  - **Data\_Pages:integer –** broj stranica u dokumentu

  - **Data\_PositionToolbarsTime:integer –** trajanje postavljanja alatnih traka na njihovo mjesto

  - **Data\_ReadOnly:bool –** istinito ako je datoteka samo za čitanje

  - **Data\_RecordSetCount:integer –** broj skupova zapisa u dijagramu

  - **Data\_RecoveryTime:integer –** trajanje otvaranja datoteka za oporavak

  - **Data\_ReviewerPages:integer –** broj stranica pregledavatelja u dijagramu

  - **Data\_RibbonTime:integer –** trajanje postupka prikazivanja trake stanja

  - **Data\_RoamingSettingsStartupTime:integer –** trajanje stvaranja i učitavanja svih trenutnih zajedničkih postavki programa Visio

  - **Data\_SchemeMgrStartupTime:integer –** trajanje inicijalizacije upravitelja shema

  - **Data\_SDX\_AssetId –** postoji SAMO za dodatke iz trgovine. OMEX dodatku dodjeljuje AssetId prilikom ulaska u trgovinu

  - **Data\_SDX\_BrowserToken –** identifikator u predmemoriji web-preglednika

  - **Data\_SDX\_HostJsVersion –** ovo je verzija sustava Office.js specifična za određenu platformu (na primjer, outlook web16.01.js) i sadrži podlogu API-ja za dodatke

  - **Data\_SDX\_Id –** GUID dodatka koji ga identificira na jedinstven način

  - **Data\_SDX\_InstanceId –** predstavlja par dokumenata u dodatku

  - **Data\_SDX\_MarketplaceType –** označava odakle se dodatak instalirao

  - **Data\_SDX\_OfficeJsVersion –** to je verzija sustava Office.js koja će se preusmjeriti na verziju specifičnu za određenu platformu.

  - **Data\_SDX\_Version –** verzija dodatka

  - **Data\_ShellCmdLineTime:integer –** trajanje raščlambe i izvođenja naredbi ljuske u naredbenom retku

  - **Data\_Size:long** – veličina datoteke u bajtovima

  - **Data\_StartEndTransactionTime:integer –** trajanje inicijalizacije komponenti programa Visio

  - **Data\_STNInitTime:integer –** trajanje inicijalizacije konfiguracije prozora šablone

  - **Data\_Tag:string –** jedinstveni identifikator za prepoznavanje događaja „Spremi kao”

  - **Data\_ThemeCount:integer –** broj tema u dijagramu

  - **Data\_TimeStamp –** vremenska oznaka u trenutku zatvaranja dokumenta

  - **Data\_UIInitTime:integer –** trajanje inicijalizacije korisničkog sučelja

  - **Data\_WasSuccessful:bool –** istinito ako je spremanje bilo uspješno

  - **Data\_WinLaunchTime:integer –** trajanje pokretanja početnog okna programa Visio itd.)

  
#### <a name="officeextensibilitysandboxodpactivationhanging"></a>Office.Extensibility.Sandbox.ODPActivationHanging

Prikuplja se kada je dodatku sustava Office potrebno neočekivano puno vremena za pokretanje (>5 sek). Koristi se za otkrivanje i rješavanje problema u vezi s pokretanjem dodataka sustava Office.
 
Prikupljaju se sljedeća polja:

- **AppId** – ID aplikacije

- **AppInfo** – podaci koji se odnose na vrstu dodatka (okno zadatka ili UILess ili u sadržaju itd.) i vrstu pružatelja (omen, SharePoint, filesystem itd.)

- **AppInstanceId** – ID instance aplikacije 

- **AssetId** – ID sadržaja aplikacije

- **IsPreload** – upućuje na to je li dodatak unaprijed učitan u pozadini radi poboljšanja performansi aktivacije

- **NumberOfAddinsActivated** – brojač aktiviranih dodataka

- **RemoterType** – određuje vrstu daljinskog elementa (Trusted, untrusted, Win32webView, Trusted UDF itd.) koji se koristi za aktivaciju dodatka

- **StoreType** – porijeklo aplikacije

- **TimeForAuth** – vrijeme utrošeno na autorizaciju 

- **TimeForSandbox** – vrijeme utrošeno na testno okruženje

- **TimeForServerCall** – vrijeme utrošeno na poziv poslužitelja 

- **TotalTime** – ukupno utrošeno vrijeme

- **UsesSharedRuntime** – upućuje na to da koristi li aplikacija sharedRuntime ili ne.

#### <a name="officelenslenssdklaunchlens"></a>Office.Lens.LensSdk.LaunchLens

Kada korisnik pokrene Lens da bi snimio/la ili uvezao/la slike u bilo kojoj aplikaciji, pokrenut će se Lens SDK, a taj će se događaj prikupiti. Podaci o pokretanju pomažu nam utvrditi broj korisnika / uređaja koji pokreću aplikaciju i dalje razumjeti upotrebu značajki. Pomaže nam u praćenju broja korisnika koji koriste proizvod, kao i prepoznavanju promjena u trendovima, pomaže u traženju i ispravljanju problema u proizvodu.

Prikupljaju se sljedeća polja:

- **Data_isResumeSession** – Je li aplikacija pokrenuta u nastavku ili je korisnik započeo novi postupak. (Booleova polja) 

- **Data_launchPerf** – Cijeli broj koji označava vrijeme koje je potrebno za pokretanje aplikacije (na sustavu Android)

- **Data_LaunchWorkFlowItem** – polje određuje je li aplikacija pokrenuta sa zaslona fotoaparata ili na zaslonu uređivanje. 

- **Data_mediaCompressionFactor** – faktor pomoću kojeg aplikacija komprimira slike.

- **Data_RecoveryMode** -Boolean polje koje upućuje na to je li ta sesija vraćena kada je aplikacija ubijena (na sustavu Android)

- **IsDexModeEnabled** -Booleov izraz označava ako uređaj podržava Samsung Dex značajke.

- **IsEmbeddedLaunch** -Boolean polje koje upućuje na to je li korisnik pokrenuo kontrolu u načinu slike u slici.

- **IsInterimCropEnabled** –Boolean polje koje upućuje na to je li korisnik odabrao ručno obrezivanje svake slike.

- **IsMultiWindowEnabled** – Boolean polje koje pokazuje da li je moguće pokrenuti aplikaciju na podijeljenom zaslonu.

- **LaunchPerf** – Cijeli broj koji označava vrijeme koje je potrebno za pokretanje aplikacije (na sustavu iOS)

- **Ponovno ponavljanje** -Boolean polje koje upućuje na to je li ta sesija vraćena nakon ubojstva aplikacije (na sustavu iOS)

- **SDKMode** – Način na koji su snimljene slike.


#### <a name="officeofficemobileappactivationlaunch"></a>Office.OfficeMobile.AppActivation.Launch

Ovaj događaj identificira prvu i daljnje aktivacije putem vanjskih okidača koji aktiviraju aplikaciju. Aktivacija aplikacije učitava određene ovisnosti koje su odgovorne za rad aplikacije bez poteškoća i taj će događaj zabilježiti jesu li se uspješno učitale. Također će zabilježiti izvor aktivacije i namjeru aplikacije koja je bila odgovorna za aktivaciju aplikacije.

Prikupljaju se sljedeća polja:

- **ActionName** – mapiranje vrijednosti cijelog broja na ime radnje/značajke koja je pozvana iz točke aktivacije.
 
- **ActivationType** – mapiranje vrijednosti cijelog broja na izvor aktivacije
  
- **IsActionTriggered** – Booleova vrijednost koja određuje je li radnja pokrenuta nakon uspješne aktivacija aplikacije.

- **IsFirstRun** – Booleova vrijednost koja određuje radi li se o prvom ili daljnjem izvršavanju aplikacije.
 

#### <a name="officeofficemobilefrefirstrunsetup"></a>Office.OfficeMobile.FRE.FirstRunSetup

Prvo pokretanje aplikacije nakon instalacije aktivirat će taj događaj otkucaja srca. To će pomoći pri prepoznavanju instalacija i automatskih nadogradnji sa starijih verzija aplikacije te nam omogućiti prepoznavanje pogrešaka u automatskim nadogradnjama, uključujući neuspjela učitavanja biblioteka i preuzimanja paketa proširenja ili jezičnih paketa.

Prikupljaju se sljedeća polja:

- **IsFlightAssigned** – Booleova vrijednost koja određuje je li korisnik dio bilo koje unaprijed dodijeljene grupe za testne verzije koja može uzrokovati izlaganje određenim doživljajima.

- **IsFRELoadSuccessful** – cijeli broj koji navodi rezultantno stanje

#### <a name="officeonenoteandroidappappbootcomplete-officeandroidearlytelemetryappbootcomplete"></a>Office.OneNote.Android.App.AppBootComplete, Office.Android.EarlyTelemetry.AppBootComplete

*[Ovaj je događaj prethodno imenovan OneNote.AppLaunch.]*

Ključni signal korišten za osiguravanje da novi privatni korisnici (Microsoftov račun) uspješno mogu prvi put koristiti aplikaciju OneNote.  To se koristi za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge.  Ako korisnici ne mogu prvi put pokrenuti aplikaciju, time bi se izazvao incident visoke ozbiljnosti.

Prikupljaju se sljedeća polja: 

- **ACTIVITY_BOOT_TIME_IN_MS** – vrijeme potrebno za dovršetak stvaranja aktivnosti

- **ACTIVITY_NAME** – naziv otvorene aktivnosti prilikom pokretanja 

- **ANY_DIALOG_SHOWN** – označava pokazuje li se tijekom pokretanja neki dijaloški okvir

- **APP_SUSPEND_DURING_EVENT** – označava je li pokretanje sustava spriječeno

- **APP_THREAD_CREATION_WAIT_TIME_TIME_FOR_APP_THREAD_CREATION** – vrijeme potrebno za stvaranje niti aplikacije

- **AVAILABLE_MEMORY_IN_MB** – ukupna memorija dostupna na uređaju 

- **AVG_SNAPSHOT_POPULATION_TIME** – prosječno vrijeme potrebno za dohvaćanje struktura bilježnica tijekom korištenja aplikacije

- **BOOT_END_AT_VIEW** – potkategorija naziva aktivnosti (naziv prikaza)

- **BOOT_SNAPSHOTS** – pojedinosti dohvaćanja strukture bilježnica za račun(e) korištene u aplikaciji

- **COREAPP_STARTUP_ACCOUNT_SETUP_STARTUP_ACCOUNT_SETUP** – vrijeme potrebno za provjeru i pokretanje SSO iskustva

- **CRASH_INTERACTION_DURING_BOOT> 0** – upućuje je li se aplikacija srušila tijekom posljednje sesije

- **DALVIK_HEAP_LIMIT_IN_MB** – zastarjelo

- **DELAY_LOAD_STICKY_NOTES** – označava učitavaju li se ljepljive bilješke sa zakašnjenjem ili ne

- **FISHBOWL_SHOWN_DURING_EVENT** – označava slučajeve kada sadržaj nije sinkroniziran

- **HAS_LOGCAT_LOGGING_IMPACT_ON_BOOT** – označava utječu li zapisnici na vrijeme pokretanja

- **INIT_SNAPSHOT_DURATION** – vrijeme potrebno za dobivanje strukture bilježnice za korisničke račune

- **IS_COLD_BOOT** – upućuje na to je li aplikacija pokrenuta kada se aplikacija nije izvodila u pozadini.

- **IS_FIRST_LAUNCH** – upućuje na to je li ovo prvi put da je aplikacija pokrenuta na uređaju

- **IS_FOLDABLE_TYPE** – označava je li uređaj sklopivi uređaj

- **IS_PHONE** – označava je li uređaj telefon ili tablet

- **IS_RECENT_PAGES_AVAILABLE_ON_FRAGMENT_CREATION** – upućuje na to je li sučelje spremno i čeka da sadržaj postane dostupan 

- **IS_REHYDRATE_LAUNCH** – upućuje na to je li sustav zaustavio aplikaciju

- **IS_UPGRADE** – označava pokreće li se aplikacija nakon nadogradnje

- **JOT_MAIN_APP_CREATE_TIME_MAIN_APP_CREATE_TIME** – vrijeme potrebno za stvaranje JOT komponente (komponenta zajedničkog koda) 

- **JOT_MAIN_APP_INIT_TIME_MAIN_APP_INIT_TIME** – vrijeme potrebno za inicijalizaciju JOT komponente

- **LAUNCH_POINT** – označava je li aplikacija pokrenuta iz widgeta, ikone aplikacije ili hiperveze ili opcije „Zajednički koristi na“, itd.

- **MSO_ACTIVATION_TIME_ACTIVATION_TIME** – vrijeme potrebno za inicijalizaciju MSO-a

- **NATIVE_LIBRARIES_LOAD_TIME** – vrijeme potrebno za učitavanje biblioteka

- **NAVIGATION_CREATE_TO_NAVIGATION_RESUME_CREATE_TO_NAVIGATION_RESUME** – vrijeme potrebno za dovršavanje navigacije

- **NAVIGATION_RESUME_TO_BOOT_END_RESUME_TO_BOOT_END** – vrijeme potrebno za mjerenje kašnjenja u učitavanju stranice nakon pokretanja

- **NAVIGATION_SET_CONTENT_VIEW_TIME_SET_CONTENT_VIEW_TIME** – vrijeme potrebno za unošenje sadržaja

- **NUMBER_Of_RUNNING_PROCESSES** – označava broj aktivnih procesa koji se izvode

- **NUMBER_OF_SNAPSHOTS** – broj dohvaćanja struktura bilježnice tijekom pokretanja

- **OFFICEASSETMANAGER_INITIALIZATION_TIME** – vrijeme potrebno za raspakiranje i pokretanje upravitelja sadržaja

- **PROCESS_BOOT_TIME_IN_MS** – vrijeme potrebno za dovršetak stvaranja procesa

- **ROOT_ACTIVITY_CREATE_ACTIVITY_CREATE** – vrijeme potrebno za prijelaz s korijenskog sloja 

- **ROOT_ACTIVITY_DISK_CHECK_ACTIVITY_DISK_CHECK** – zastarjelo

- **ROOT_ACTIVITY_LAUNCH_NEXTACTIVITY_ACTIVITY_LAUNCH_NEXTACTIVITY** – zastarjelo

- **ROOT_ACTIVITY_PROCESS_INTENT_ACTIVITY_PROCESS_INTENT** – zastarjelo 

- **ROOT_ACTIVITY_SESSION_ACTIVITY_SESSION** – vrijeme potrebno za prijelaz s korijenskog sloja 

- **ROOT_TO_NAVIGATION_TRANSITION_TO_NAVIGATION_TRANSITION** – vrijeme potrebno za upravljanje navigacijom iz korijena

- **SNAPSHOT_PUBLISH_TO_RENDERING_END_PUBLISH_TO_RENDERING_END** – vrijeme za dovršetak prikazivanja sadržaja

- **SPLASH_ACTIVITY_SESSION_ACTIVITY_SESSION** – vrijeme potrebno za prikazivanje pozdravnog zaslona

- **SPLASH_TO_ROOT_TRANSITION_TO_ROOT_TRANSITION** – vrijeme potrebno za prijelaz s korijenskog sloja 

- **TIME_BETWEEN_PROCESS_BOOT_AND_ACTIVITY_BEGIN_IN_MS** – vrijeme između stvaranja procesa i aktivnosti 

- **TIME_TAKEN_IN_MS** – vrijeme potrebno za dovršavanje pokretanja
 
- **TOTAL_MEMORY_IN_MB** – ukupna memorija uređaja
 
- **USER_INTERACTED_DURING_EVENT** – označava je li korisnik komunicirao tijekom pokretanja

#### <a name="officeonenoteandroidapponenoteappforeground-officeandroidearlytelemetryonenoteappforeground"></a>Office.OneNote.Android.App.OneNoteAppForeground, Office.Android.EarlyTelemetry.OneNoteAppForeground

*[Ovaj je događaj prethodno imenovan OneNote.App.OneNoteAppForeground.]*

Signal koji upućuje da je OneNote aplikacija u prvom planu.  Telemetrija se koristi za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. 

Prikupljaju se sljedeća polja: 

- Nijedno

#### <a name="officeonenoteandroidapplaunch-officeandroidearlytelemetryapplaunch"></a>Office.OneNote.Android.AppLaunch, Office.Android.EarlyTelemetry.AppLaunch

*[This event was previously named OneNote.AppLaunch.]*

Ključni signal koji se koristi za osiguravanje da korisnici aplikacije OneNote mogu uspješno pokrenuti aplikaciju.  Telemetrija se koristi za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. 

Prikupljaju se sljedeća polja: 

- **ANDROID_SDK_VERSION** – bilježi verziju SDK-a sustava Android

- **FirstLaunchTime** – bilježi vrijeme prvog pokretanja aplikacije

- **InstallLocation** – upućuje na to je li aplikacija unaprijed instalirana ili je preuzeta iz trgovine

- **is_boot_completed_ever** – upućuje na to je li aplikacija nekada bila uspješno pokrenuta na uređaju

- **IS_DARK_MODE_ENABLED** – Booleova vrijednost koja označava je li aplikacija u tamnom načinu rada ili nije

- **NewOneNoteUser** – identificira je li korisnik novi korisnik

#### <a name="officeoutlookdesktopexchangepuidandtenantcorrelation"></a>Office.Outlook.Desktop.ExchangePuidAndTenantCorrelation

Jedanput po sesiji prikuplja PUID korisnika i identifikator klijenta. Korelacija PUID-a i klijenta nužna je za razumijevanje i dijagnosticiranje problema s programom Outlook na razini pojedinih klijenata.

Prikupljaju se sljedeća polja:

  - **CollectionTime** – vremenska oznaka događaja

  - **ConnId** – identifikator veze: identifikator veze kojom se raščlanjuju PUID i identifikator OMS klijenta

  - **OMSTenantId** – jedinstveni identifikator klijenta, koji generira Microsoft

  - **PUID** – PUID sustava Exchange za jedinstvenu identifikaciju korisnika


#### <a name="officeoutlookmacmacolkactivationstate"></a>Office.Outlook.Mac.MacOLKActivationState

Prikuplja način na koji se program Outlook aktivira, primjerice s pretplatom ili količinskim licenciranjem. Kako ne bi bilo porasta u pogreškama, podaci se nadziru. Također analiziramo podatke kako bismo pronašli područja poboljšanja. 

Prikupljaju se sljedeća polja:

- **SetupUIActivationMethod** – način aktivacije programa Outlook, primjerice s pretplatom ili količinskim licenciranjem

#### <a name="officepowerpointdocoperationopen"></a>Office.PowerPoint.DocOperation.Open 

Prikuplja se svaki put kada PowerPoint otvori datoteku. Sadrži informacije o uspješnosti, pojedinosti neuspjeha, metriku performansi i osnovne detalje o datoteci, uključujući vrstu oblika datoteke i metapodatke dokumenta. Te su informacije nužne da bi se osiguralo da PowerPoint može uspješno otvarati datoteke bez smanjenja performansi. To omogućuje dijagnosticiranje bilo kakvih problema koje otkrijemo.

Prikupljaju se sljedeća polja:

  - **Data\_AddDocTelemetryResult –** sadrži li ova stavka zapisnika svu potrebnu telemetriju dokumenta (polja Data\_Doc\_\*)

  - **Data\_AddDocumentToMruList –** trajanje izvršavanja metode AddDocumentToMruList

  - **Data\_AlreadyOpened –** je li taj dokument prethodno otvaran (u kontekstu iste sesije procesa)

  - **Data\_AntiVirusScanMethod –** unaprijed definiran skup vrijednosti vrste antivirusnog pregleda (IOAV, AMSI, None itd.)

  - **Data\_AntiVirusScanStatus –** unaprijed definiran skup vrijednosti antivirusnog pregleda koji se provodi za svaki otvoreni dokument (NoThreatsDetected, Failed, MalwareDetected itd.)

  - **Data\_AsyncOpenKind –** unaprijed definiran skup vrijednosti asinkronih mogućnosti (Collab, ServerOnly, SyncBacked, NotAsync)

  - **Data\_CancelBackgroundDownloadHr –** je li preuzimanje dokumenta prekinuto? Ako jest, što je bio rezultat tog prekida?

  - **Data\_CheckForAssistedReadingReasons –** trajanje izvršavanja metode CheckForAssistedReadingReasons u milisekundama

  - **Data\_CheckForDisabledDocument –** trajanje izvršavanja metode CheckForDisabledDocument u millisekundama

  - **Data\_CheckForExistingDocument –** trajanje izvršavanja metode CheckForExistingDocument u millisekundama

  - **Data\_CheckIncOpenResult –** trajanje izvršavanja metode CheckIncOpenResult u milisekundama

  - **Data\_CheckLambdaResult –** trajanje izvršavanja metode CheckLambdaResult u milisekundama

  - **Data\_CheckPackageForRequiredParts –** trajanje izvršavanja metode CheckPackageForRequiredParts u milisekundama

  - **Data\_CheckPackageForSpecialCases –** trajanje izvršavanja metode CheckPackageForSpecialCases u milisekundama

  - **Data\_CheckRequiredPartsLoaded –** trajanje izvršavanja metode CheckRequiredPartsLoaded u milisekundama

  - **Data\_CheckWebSharingViolationForIncOpen –** trajanje izvršavanja metode CheckWebSharingViolationForIncOpen u milisekundama
   
  - **Data_CloseAndReopenWithoutDiscard –** Je li dokument zatvoren i ponovno otvoren tijekom otvorenog postupka bez odbacivanja.

  - **Data\_ContentTransaction –** unaprijed definiran skup vrijednosti kojima se određuje kada je moguće stvoriti transakciju (AllowedOnLoadDocument, AllowedOnOpenComplete itd.)

  - **Data_CorrelationId-** GUID proslijeđen u PowerPoint pomoću rukovatelja protokolom za korelaciju telemetrije. Rukovatelj protokolom zaseban je proces koji upravlja Office vezama za OS.

  - **Data\_CppUncaughtExceptionCount:long –** neuhvaćene lokalne iznimke dok je aktivnost pokrenuta

  - **Data\_CreateDocumentTimeMS –** trajanje izvršavanja metode CreateDocumentTimeMS u milisekundama

  - **Data\_CreateDocumentToken –** trajanje izvršavanja metode CreateDocumentToken u milisekundama

  - **Data\_CreateDocumentToW –** trajanje izvršavanja metode CreateDocumentToW u milisekundama

  - **Data\_CreateDocWindow –** trajanje izvršavanja metode CreateDocWindow u milisekundama

  - **Data\_CreateLocalTempFile –** trajanje izvršavanja metode CreateLocalTempFile u milisekundama

  - **Data\_DetachedDuration:long –** vrijeme tijekom kojeg je aktivnost bila odvojena ili se nije izvršavala

  - **Data\_DetermineFileType –** trajanje izvršavanja metode DetermineFileType u milisekundama

  - **Data\_Doc\_AccessMode:long –** kako je dokument otvoren (samo za čitanje / samo za pisanje)

  - **Data\_Doc\_AssistedReadingReasons:long –** unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

  - **Data_Doc_AsyncOpenKind:long –** označava je li otvorena predmemorirana verzija dokumenta u oblaku i koja je logika za asinkrono osvježavanje korištena.

  - **Data\_Doc\_ChunkingType:long –** kako je dokument pohranjen u sustavu SharePoint

  - **Data\_Doc\_EdpState:long –** stanje dokumenta s obzirom na zaštitu korporativnih podataka

  - **Data\_Doc\_Ext:string –** nastavak dokumenta

  - **Data\_Doc\_Extension:string –** nastavak dokumenta

  - **Data\_Doc\_FileFormat:long –** unaprijed definirani skup vrijednosti oblika datoteke (precizniji od nastavka)

  - **Data\_Doc\_Fqdn:string – -** mjesto pohrane dokumenta (SharePoint.com, live.net), dostupno samo za domene sustava Office 365

  - **Data\_Doc\_FqdnHash:string – -** raspršivanje mjesta pohrane dokumenta

  - **Data\_Doc\_IdentityTelemetryId:string – -** jedinstveni GUID korisnika

  - **Data\_Doc\_IdentityUniqueId:string –** jedinstveni identifikator identiteta korištenog za akciju zajedničkih dokumenata

  - **Data\_Doc\_IOFlags:long –** bit-maska za razne zastavice vezane uz ulaz i izlaz za određeni dokument

  - **Data\_Doc\_IrmRights:long –** unaprijed definiran skup vrijednosti za vrstu informacija koju upravljanje pravima na informacije primjenjuje na ovom dokumentu (proslijedi, odgovori, SecureReader, uređivanje itd.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool –** istinito ako je HTTP zaglavlje „IsCloudCollabEnabled“ već prihvaćeno iz zahtjeva MOGUĆNOSTI.

  - **Data\_Doc\_IsIncrementalOpen:bool – -** je li dokument otvoren inkrementalno (nova značajka koja otvara dokument bez potrebe za preuzimanjem cijelog dokumenta)

  - **Data\_Doc\_IsOcsSupported:bool –** podržava li dokument suautorstvo pomoću novog servisa OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool –** otvara li se dokument iz lokalne predmemorije?

  - **Data\_Doc\_IsSyncBacked:bool –** otvara li se dokument iz mape koja koristi aplikaciju OneDrive za povratnu sinkronizaciju

  - **Data\_Doc\_Location:long –** unaprijed definiran skup vrijednosti mjesta na kojima se dokument pohranjuje (lokalno, SharePoint, WOPI, mreža itd.)

  - **Data\_Doc\_LocationDetails:long –** unaprijed definiran skup vrijednosti detaljnijih lokacija (mapa Temp, mapa preuzimanja, dokumenti servisa One Drive, slike servisa One Drive itd.)

  - **Data\_Doc\_NumberCoAuthors:long –** broj suautora prilikom otvaranja dokumenta

  - **Data\_Doc\_PasswordFlags:long –** unaprijed definirani skup vrijednosti načina na koji je dokument šifriran pomoću lozinke (nema, lozinka za čitanje, lozinka za uređivanje)

  - **Data\_Doc\_ReadOnlyReasons:long –** unaprijed definirani skup vrijednosti koji naznačuje zašto je dokument označen samo za čitanje (zaključan na poslužitelju, konačni dokument, zaštićen lozinkom za uređivanje itd.)

  - **Data\_Doc\_ResourceIdHash:string –** raspršivanje identifikatora resursa za dokumente pohranjene u oblaku

  - **Data_Doc_RtcType –** označava kako je kanal u stvarnom vremenu (RTC) postavljen za trenutnu datoteku (onemogućen, nepodržan, na zahtjev, uvijek uključen itd.).

  - **Data\_Doc\_ServerDocId:string –** nepromjenjivi identifikator za dokumente pohranjene u oblaku

  - **Data\_Doc\_ServerProtocol:long –** unaprijed definirani skup vrijednosti o protokolu koji se koristi za komuniciranje s poslužiteljem (Http, Cobalt, WOPI itd.)
 
  - **Data\_Doc\_ServerType:long –** unaprijed definiran skup vrijednosti za vrstu poslužitelja (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long –** temelji li se poslužitelj na sustavu Office14, Office15 ili Office 16?

  - **Data\_Doc\_SessionId:long –** generirani GUID koji identificira instancu dokumenta u sklopu iste sesije procesa

  - **Data\_Doc\_SharePointServiceContext:string –** neprozirni niz, obično GridManagerID.FarmID. Korisno za korelaciju klijentskih i poslužiteljskih zapisnika

  - **Data\_Doc\_SizeInBytes:long –** veličina dokumenta u bajtovima

  - **Data\_Doc\_SpecialChars:long –** bit-maska koja pokazuje posebne znakove u URL-u ili putu dokumenta

  - **Data\_Doc\_StorageProviderId:string –** niz koji određuje davatelja pohrane dokumenta, primjerice „DropBox“

  - **Data\_Doc\_StreamAvailability:long –** unaprijed definiran skup vrijednosti statusa toka dokumenta (dostupno, trajno onemogućeno, nije dostupno)

  - **Data\_Doc\_UrlHash:string –** raspršivanje punog URL-a dokumenata pohranjenih u oblaku

  - **Data\_Doc\_UsedWrsDataOnOpen:bool –** istinito ako je datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka na glavnom računalu

  - **Data\_Doc\_WopiServiceId:string –** identifikator WOPI servisa, na primjer, „Dropbox“

  - **Data\_DownloadExcludedData –** trajanje izvršavanja metode DownloadExcludedData u milisekundama

  - **Data\_DownloadExcludedDataTelemetry –** unaprijed definiran skup vrijednosti stanja sinkronog čekanja na preuzimanje (SynchronousLogicHit, UserCancelled RunModalTaskUnexpectedHResult itd.)

  - **Data\_DownloadFileInBGThread –** trajanje izvršavanja metode DownloadFileInBGThread u millisekundama

  - **Data\_DownloadFragmentSize –** veličina fragmenta (bloka datoteke koji je moguće preuzeti), obično 3,5 MB

  - **Data\_ExcludedEmbeddedItems –** broj zip dijelova izuzetih iz prvog prikaza

  - **Data\_ExcludedEmbeddedItemsSize –** ukupna veličina zip dijelova izuzetih iz prvog prikaza

  - **Data\_ExcludedRequiredItems –** broj zip dijelova koji su izuzeti, ali su obavezni za prvi prikaz

  - **Data\_ExcludedRequiredItemsSize –** ukupna veličina zip dijelova koji su izuzeti, ali su obavezni za prvi prikaz

  - **Data\_ExecutionCount –** koliko je puta izvršen protokol IncOpen

  - **Data\_FailureComponent:long –** unaprijed definirani skup vrijednosti koji označava koja je komponenta uzrokovala neuspjeh ovog protokola? (Conflict, CSI, Internal itd.)

  - **Data\_FailureReason:long –** unaprijed definiran skup vrijednosti razloga neuspjeha (FileIsCorrupt, BlockedByAntivirus itd.)

  - **Data\_FCreateNew –** je li to nov prazan dokument

  - **Data\_FCreateNewFromTemplate –** je li to nov dokument iz predložaka

  - **Data_FErrorAfterDocWinCreation:boolean –** je li se dogodila pogreška ili iznimka nakon stvaranja prozora dokumenta.

  - **Data\_FileUrlLocation –** unaprijed definiran skup vrijednosti mjesta pohrane dokumenta (NetworkShare, LocalDrive, ServerOther itd.)

  - **Data\_FirstSlideCompressedSize –** komprimirana veličina zip dijela prvog slajda (obično Slide1.xml)

  - **Data_FIsAutoBackupFile-** Je li ta datoteka automatska datoteka sigurnosne kopije?

  - **Data\_FIsDownloadFileInBgThreadEnabled –** je li omogućeno preuzimanje u pozadinskoj niti?

  - **Data\_fLifeguarded:bool –** je li dokument ikad popravljen pomoću značajke lifeguard (značajka za popravljanje pogrešaka dokumenta bez slanja upita korisniku)?

  - **Data\_ForceReopenOnIncOpenMergeFailure –** Oznaka koja predstavlja ako smo bili prisiljeni ponovno se otvoriti zbog neuspjeha spajanja u Inc Open

  - **Data\_ForegroundThreadPass0TimeMS –** (samo na Macu) ukupno vrijeme provedeno u niti u prvom planu u prvom prolazu

  - **Data\_ForegroundThreadPass1TimeMS –** (samo na Macu) ukupno vrijeme provedeno u niti u prvom planu u drugom prolazu

  - **Data\_FWebCreatorDoc –** je li dokument stvoren iz predloška ili alata za brz početak rada

  - **Data\_HasDocToken –** ima li taj dokument CSI token dokumenta (interni kod)

  - **Data\_HasDocument –** ima li taj dokument CSI dokument (interni kod)

  - **Data\_InclusiveMeasurements –** obuhvaćaju li izmjere trajanja metoda i trajanje pozivanja podređenih metoda

  - **Data\_IncompleteDocReasons –** unaprijed definiran skup vrijednosti razloga zbog kojih otvaranje nije bilo potpuno (Nepoznato, DiscardFailure itd.)

  - **Data\_IncOpenDisabledReasons –** unaprijed definiran skup vrijednosti razloga zbog kojih je onemogućeno inkrementalno otvaranje

  - **Data\_IncOpenFailureHr –** rezultat koji govori zašto inkrementalno otvaranje nije uspjelo

  - **Data\_IncOpenFailureTag –** oznaka (pokazivač na mjesto u kodu) mjesta na kojem je inkrementalno otvaranje doživjelo neuspjeh

  - **Data\_IncOpenFallbackReason –** zašto IncOpen nije pokrenut

  - **Data\_IncOpenRequiredTypes –** unaprijed definiran skup vrijednosti vrsta sadržaja potrebnih za prvi prikaz (RequiredXmlZipItem, RequiredNotesMaster itd.)

  - **Data\_IncOpenStatus –** unaprijed definiran skup vrijednosti statusa inkrementalnog otvaranja (Attempted, FoundExcludedItems, DocIncOpenInfoCreated itd.)

  - **Data\_InitFileContents –** trajanje izvršavanja metode InitFileContents u milisekundama

  - **Data\_InitialExcludedItems –** broj inicijalno izuzetih zip dijelova

  - **Data\_InitialExcludedItemsSize –** ukupna veličina inicijalno izuzetih zip dijelova

  - **Data\_InitializationTimeMS –** (samo na Macu) vrijeme inicijalizacije

  - **Data\_InitialRoundtripCount –** broj odgovora poslužitelja potrebnih za formiranje inicijalne zip arhive

  - **Data\_InitLoadProcess –** trajanje izvršavanja metode InitLoadProcess u milisekundama

  - **Data\_InitPackage –** trajanje izvršavanja metode InitPackage u milisekundama

  - **Data\_InitSecureReaderReasons –** trajanje izvršavanja metode InitSecureReaderReasons u milisekundama

  - **Data\_IsIncOpenInProgressWhileOpen –** u slučaju višestrukog otvaranja istog dokumenta, je li protokol za inkrementalno otvaranje pokrenut paralelno s protokolom za otvaranje?

  - **Data\_IsMultiOpen –** podržavamo li višestruko otvaranje?

  - **Data\_IsOCS –** je li dokument u OCS načinu rada u svom zadnjem poznatom stanju

  - **Data\_IsODPFile –** koristi li se dokument u obliku Open Document Format na servisu OpenOffice.org

  - **Data\_IsPPTMetroFile –** je li dokument u metro (pptx) obliku datoteke

  - **Data\_LoadDocument –** trajanje izvršavanja metode LoadDocument u milisekundama

  - **Data\_MeasurementBreakdown –** raščlamba šifriranih izmjera (performanse skraćene detaljne metode)

  - **Data\_Measurements –** šifrirane izmjere

  - **Data\_MethodId –** zadnja izvršena metoda

  - **Data\_NotRequiredExcludedItems –** ukupan broj stavki paketa programa PowerPoint koje nisu nužne za prvi prikaz te su izuzete

  - **Data\_NotRequiredExcludedItemsSize –** ukupna veličina stavki paketa programa PowerPoint koje nisu nužne za prvi prikaz te su izuzete

  - **Data\_NotRequiredExcludedParts –** ukupan broj zip dijelova koji nisu nužni za prvi prikaz te su izuzeti

  - **Data\_NotRequiredExcludedPartsSize –** ukupan broj zip dijelova koji nisu nužni za prvi prikaz te su izuzeti

  - **Data_OngoingBlockingOpenCount –** broj koliko se blokirajućih otvorenih protokola trenutno izvodi.
  
  - **Data_OngoingOpenCount –** broj koliko se otvorenih protokola trenutno izvodi.

  - **Data\_OpenCompleteFailureHR –** rezultat koji govori zašto protokol OpenComplete nije uspio

  - **Data\_OpenCompleteFailureTag –** oznaka (pokazivač na mjesto u kodu) mjesta na kojem je protokol OpenComplete doživio neuspjeh

  - **Data\_OpenLifeguardOption –** unaprijed definiran skup vrijednosti izbora za lifeguard operaciju (None, TryAgain, OpenInWebApp itd.)

  - **Data\_OpenReason –** unaprijed definiran skup vrijednosti načina na koji je taj dokument otvoren (FilePicker, OpenFromMru, FileDrop itd.)

  - **Data\_OSRPolicy –** pravilnik za sigurni čitač

  - **Data\_OSRReason –** razlozi zašto je dokument otvoren u sigurnom čitaču

  - **Data\_OtherContentTypesWithRequiredParts –** nestandardne vrste sadržaja koje su izuzete, ali su obavezne za prvi prikaz

  - **Data\_PrepCacheAsync –** zastavica za OcsiOpenPerfPrepCacheAsync

  - **Data\_PreviousDiscardFailed –** označava da prethodni pokušaj otvaranja/zatvaranja dokumenta nije pravilno oslobodio svu memoriju

  - **Data\_PreviousFailureHr –** U slučaju ponovnog otvaranja istog dokumenta, što je bio rezultat zadnjeg neuspjeha

  - **Data\_PreviousFailureTag –** u slučaju ponovnog otvaranja istog dokumenta, koja je bila oznaka zadnjeg neuspjeha (pokazivač na mjesto u kodu)

  - **Data\_RemoteDocToken –** je li omogućeno daljinsko otvaranje (prototipna značajka koja omogućuje otvaranje datoteke iz servisa umjesto s glavnog računala)?

  - **Data\_Repair –** jesmo li u načinu rada za popravak dokument (za oštećene dokumente koji se mogu popraviti)

  - **Data\_RequestPauseStats –** koliko je puta kod zatražio pauziranje snimanja performansi

  - **Data\_RequiredPartsComressedSize –** ukupna veličina obaveznih dijelova za PowerPoint potrebnih za prvi prikaz

  - **Data\_RequiredPartsDownload –** ukupna veličina preuzetih obaveznih dijelova za PowerPoint

  - **Data\_RequiredPartsRoundtripCount –** ukupan broj kružnih putovanja (poziva glavnom računalu) potrebnih za prikupljanje svih dijelova obaveznih za prvi prikaz u programu PowerPoint

  - **Data\_RequiredZipItemsDownload –** ukupna veličina obaveznih zip stavki potrebnih za prvi prikaz

  - **Data\_RequiredZipItemsRoundtripCount –** ukupan broj kružnih putovanja (poziva glavnom računalu) potrebnih za prikupljanje svih obaveznih zip dijelova za prvi prikaz

  - **Data\_RoundtripsAfterMissingRequiredParts –** ukupan broj kružnih putovanja (poziva glavnom računalu) potrebnih nakon što smo pronašli nedostajuće obavezne dijelove za PowerPoint

  - **Data\_RoundtripsAfterMissingRequiredZipItems –** ukupan broj kružnih putovanja (poziva glavnom računalu) potrebnih nakon što smo pronašli nedostajuće obavezne zip dijelove

  - **Data\_RoundtripsAfterRequiredPackage –** ukupan broj kružnih putovanja (poziva glavnom računalu) potrebnih nakon što smo stvorili paket

  - **Data\_RoundtripsAfterRequiredParts –** ukupan broj kružnih putovanja (poziva glavnom računalu) potrebnih nakon što smo preuzeli sve obavezne dijelove

  - **Data\_SetDocCoAuthAutoSaveable –** trajanje izvršavanja metode SetDocCoAuthAutoSaveable u milisekundama

  - **Data\_SniffedFileType –** utemeljena procjena vrste datoteke oštećenog dokumenta

  - **Data\_StartTime –** brojač performansi u trenutku početka otvaranja

  - **Data\_StopwatchDuration:long –** ukupno vrijeme za aktivnost

  - **Data\_SyncSlides –** trajanje izvršavanja metode SyncSlides u milisekundama

  - **Data\_TimerStartReason –** unaprijed definiran skup vrijednosti načina na koje je pokrenut mjerač vremena (CatchMissedSyncStateNotification, WaitingForFirstDownload itd.)

  - **Data\_TimeSplitMeasurements –** raščlamba šifriranih izmjera (performanse skraćene detaljne metode)

  - **Data\_TimeToInitialPackage –** trajanje stvaranja inicijalnog paketa

  - **Data\_TimeToRequiredPackage –** trajanje stvaranja obaveznog paketa

  - **Data\_TimeToRequiredParts –** trajanje stvaranja paketa koji sadrži sve obavezne dijelove

  - **Data\_TotalRequiredParts –** ukupan broj dijelova za PowerPoint obaveznih za prvi prikaz

  - **Data\_UnknownRequiredParts –** ukupan broj nestandardnih dijelova obaveznih za prvi prikaz

  - **Data\_UnpackLinkWatsonId –** identifikator pogreške za Watson prilikom otvaranja dokumenta putem URL-a za zajedničko korištenje na servisu OneDrive

  - **Data\_UnpackResultHint –** unaprijed definiran skup vrijednosti rezultata raspakiravanja URL-a za zajedničko korištenje (NavigateToWebWithoutError, UrlUnsupported, AttemptOpen itd.)

  - **Data\_UnpackUrl –** trajanje izvršavanja metode UnpackUrl u milisekundama

  - **Data\_UpdateAppstateTimeMS –** trajanje izvršavanja metode UpdateAppstate u milisekundama

  - **Data\_UpdateCoauthoringState –** trajanje izvršavanja metode UpdateCoauthoringState u milisekundama

  - **Data\_UpdateReadOnlyState –** trajanje izvršavanja metode UpdateReadOnlyState u milisekundama

  - **Data\_WACCorrelationId –** u slučaju otvaranja datoteke u pregledniku dobijte korelaciju WebApp zapisnika

  - **Data\_WasCachedOnInitialize –** je li taj dokument predmemoriran tijekom inicijalizacije

  - **Data\_WBDirtyBeforeDiscard –** je li radni ogranak postao prljav prije ponovnog otvaranja dokumenta

  - **Data\_ZRTOpenDisabledReasons –** zašto nije bilo moguće otvoriti dokument iz predmemorije (bez kružnog putovanja)

#### <a name="officepowerpointpptdesktopbootime"></a>Office.PowerPoint.PPT.Desktop.Bootime

Prikupljanje načina na koji je PowerPoint pokrenut. Obuhvaća pokretanje u zaštićenom prikazu, u načinu za pomoć pri čitanju, iz makronaredbe, ispisa, novog i praznog dokumenta, oporavka dokumenta, automatizacije ili klikom do cilja. Prikuplja i trajanje pokretanja programa PowerPoint. Ti su podaci ključni da bi se moglo jamčiti da su performanse programa PowerPoint zadovoljavajuće pri pokretanju u različitim načinima rada. Microsoft te podatke koristi da bi opazio dugo trajanje pokretanja prilikom otvaranja programa PowerPoint u različitim načinima rada.

Prikupljaju se sljedeća polja:

  - **AssistedReading –** u načinu rada za pomoć pri čitanju

  - **Automation –** putem automatizacije

  - **Benchmark –** pokretanje standardiziranog testa performansi

  - **Blank –** prazan dokument

  - **BootTime –** trajanje pokretanja sesije

  - **Embedding –** ugrađivanje dokumenta

  - **IsC2R –** jest klikom do cilja

  - **IsNew –** novi dokument

  - **IsOpen –** otvoren je

  - **Macro1 –** izvođenje makronaredbe

  - **Macro2 –** izvođenje makronaredbe

  - **NonStandardSpaceInCmdLine** – nema nestandardnog razmaka u naredbenom retku

  - **Print –** ispis dokumenta

  - **PrintDialog –** ispis dokumenta putem dijaloškog okvira

  - **PrintPrinter –** ispis dokumenta putem pisača

  - **ProtectedView –** u zaštićenom prikazu

  - **Regserver –** registriranje programa PowerPoint kao COM poslužitelja

  - **Restore –** vraćanje dokumenta

  - **Show –** prikaz dokumenta

  - **Time –** vrijeme sesije

  - **UnprotectedView –** u nezaštićenom prikazu

#### <a name="officepowerpointppthasuserediteddocument"></a>Office.PowerPoint.PPT.HasUserEditedDocument

Prikuplja se kada korisnik počne uređivati dokument. Microsoft te podatke koristi za izračun broja aktivnih korisnika koji su uređivali dokument programa PowerPoint

Prikupljaju se sljedeća polja:

  - **CorrelationId** – korelacijski identifikator dokumenta

#### <a name="officeprojectbootandopenproject"></a>Office.Project.BootAndOpenProject

Project je pokrenut otvaranjem datoteke. Taj događaj označava da je korisnik otvorio Office Project putem pridružene datoteke. Sadrži podatke ključne za uspješnu potvrdu da se Project može pokrenuti i da može učitati datoteku.

Prikupljaju se sljedeća polja:

  - **Data\_AlertTime –** trajanje aktivnosti dijaloškog okvira pri pokretanju.

  - **Data\_BootTime –** trajanje pokretanja programa Project

  - **Data\_CacheFileSize –** ako je datoteka predmemorirana, veličina datoteke

  - **Data\_EntDocType –** vrsta otvorene datoteke

  - **Data\_IsInCache –** je li otvorena datoteka predmemorirana

  - **Data\_LoadSRAs –** želi li korisnik učitati SRA-ove

  - **Data\_Outcome –** ukupno trajanje pokretanja i otvaranja datoteke.

  - **Data\_OpenFromDocLib –** ako je otvorena datoteka programa Project bila iz biblioteke dokumenata

  - **Data\_ProjectServerVersion –** trenutna verzija i međuverzija programa Project

#### <a name="officeprojectbootproject"></a>Office.Project.BootProject

Project je pokrenut bez otvaranja datoteke. Taj događaj označava da je korisnik otvorio Office Project bez pridružene datoteke. Sadrži podatke ključne za uspješnu potvrdu da se Project može pokrenuti.

Prikupljaju se sljedeća polja:

  - **Data\_BootTime –** trajanje pokretanja programa Project

  - **Data\_FileLoaded –** neistinito ako se otvara izvana ili s novim praznim projektom

  - **Data\_IsEntOfflineWithProfile –** jesu li korisnici u profesionalnom SKU-u pa nisu povezani s poslužiteljem

  - **Data\_IsEntOnline –** je li sesija programa Project povezana s poslužiteljem za Project sa značajkama za velike tvrtke

  - **Data\_IsLocalProfile –** je li sesija programa Project povezana s poslužiteljem za Project sa značajkama za velike tvrtke

  - **Data\_ProjectServerVersion –** trenutna verzija i međuverzija programa Project


#### <a name="officeprojectopenproject"></a>Office.Project.OpenProject

Project otvara datoteku. Taj događaj označava da korisnik izravno otvara datoteku programa Project. Sadrži podatke ključne za uspješnu potvrdu otvaranja datoteka u programu Project.

Prikupljaju se sljedeća polja:

  - **Data\_AgileMode –** definira je li otvoreni projekt kumulativan ili agilan

  - **Data\_AlertTime –** trajanje aktivnosti dijaloškog okvira pri pokretanju

  - **Data\_CacheFileSize –** ako je datoteka predmemorirana, veličina datoteke

  - **Data\_EntDocType –** vrsta otvorene datoteke

  - **Data\_IsInCache –** je li otvorena datoteka predmemorirana

  - **Data\_LoadSRAs –** želi li korisnik učitati SRA-ove

  - **Data\_OpenFromDocLib –** ako je otvorena datoteka programa Project bila iz biblioteke dokumenata

  - **Data\_Outcome –** ukupno trajanje pokretanja i otvaranja datoteke

  - **Data\_Outcome –** ukupno trajanje pokretanja i otvaranja datoteke.

  - **Data\_ProjectServerVersion –** trenutna verzija i međuverzija programa Project

#### <a name="officesessionidproviderofficeprocesssessionstart"></a>Office.SessionIdProvider.OfficeProcessSessionStart

Primjenjuje se na sve aplikacije sustava Office za Windows: win32 i UWP

Prikupljaju se sljedeća polja:

- **OfficeProcessSessionStart** šalje osnovne informacije nakon što započne nova sesija sustava Office. Koristi se za brojanje jedinstvenih sesija na određenom uređaju. To se koristi kao impulsni događaj da bi se pouzdano utvrdilo je li aplikacija pokrenuta na uređaju. Osim toga, služi i kao ključni signal za općenitu pouzdanost aplikacije

- **AppSessionGuid** – identifikator određene sesije aplikacije, koja započinje u trenutku stvaranja procesa i traje do njegovog okončanja. Oblikovan je kao standardni 128-bitni GUID, ali se sastoji od četiri dijela. Ta su četiri dijela redom: (1) 32-bitni ID procesa (2) 16-bitni ID sesije (3) 16-bitni ID pokretanja (4) 64-bitno UTC vrijeme stvaranja procesa, izraženo u koracima od 100 ns

- **processSessionId** – nasumično generirani guid za identifikaciju sesije aplikacije

- **UTCReplace_AppSessionGuid** – konstantna Booleova vrijednost. Uvijek istinito.

#### <a name="officesystemsessionhandoff"></a>Office.System.SessionHandoff

Označava da je trenutna sesija sustava Office ručno premještanje. To znači da se rukovanje korisnikovim zahtjevom za otvaranje dokumenta predaje već pokrenutoj instanci iste aplikacije.

Prikupljaju se sljedeća polja.

- **ParentSessionId** – ID sesije koja će preuzeti rukovanje korisnikovim zahtjevom.

#### <a name="officetelemetryengineisprelaunch"></a>Office.TelemetryEngine.IsPreLaunch

Primjenjuje se na aplikacije sustava Office za UWP.  Taj se događaj pokreće kada se aplikacija sustava Office prvi put pokrene nakon nadogradnje/instalacije iz trgovine. Dio je osnovnih dijagnostičkih podataka, a koristi se za praćenje je li riječ o sesiji prvog pokretanja.

Prikupljaju se sljedeća polja:

- **appVersionBuild** – broj međuverzije aplikacije.

- **appVersionMajor** – broj glavne verzije aplikacije.

- **appVersionMinor** – broj sporedne verzije aplikacije.

- **appVersionRev** – broj verzije revizije aplikacije.

- **sessionID** – nasumično generirani GUID za identifikaciju sesije aplikacije

#### <a name="officetelemetryenginesessionhandoff"></a>Office.TelemetryEngine.SessionHandOff

Primjenjuje se na aplikacije sustava Office za Win32.  Taj nam događaj pomaže razumjeti je li stvorena nova sesija za obradu događaja otvaranja datoteke koje je pokrenuo korisnik. To je ključna dijagnostička informacija koja se koristi za izvođenje signala pouzdanosti i provjeru radi li aplikacija prema očekivanjima.

Prikupljaju se sljedeća polja:

- **appVersionBuild** – broj međuverzije aplikacije.

- **appVersionMajor** – broj glavne verzije aplikacije.

- **appVersionMinor** – broj sporedne verzije aplikacije.

- **appVersionRev** – broj verzije revizije aplikacije.

- **childSessionID** – nasumično generirani guid za identifikaciju sesije aplikacije

- **parentSessionId** – nasumično generirani guid za identifikaciju sesije aplikacije

#### <a name="officevisiovisioiosappboottime"></a>Office.Visio.VisioIosAppBootTime

To se pokreće svaki put kada se pokrene aplikacija Visio iOS. Bitno je razumjeti performanse pokretanja aplikacije Visio iOS. Koristi se za otklanjanje poteškoća s lošim performansama. 

Prikupljaju se sljedeća polja:

- **Data_AppBootTime** – trajanje potrebno za pokretanje aplikacije u milisekundama.

#### <a name="officevisiovisioiosappresumetime"></a>Office.Visio.VisioIosAppResumeTime 

Ovaj se događaj pokreće svaki put kada se aplikacija Visio iOS nastavi izvoditi. Neophodno je izmjeriti performanse nastavka izvođenja aplikacije i riješiti probleme s performansama aplikacije Visio iOS.

Prikupljaju se sljedeća polja:

- **Data_AppResumeTime** – Trajanje nastavka izvođenja aplikacije u milisekundama.

#### <a name="officewordfileopenopencmdfilemrupriv"></a>Office.Word.FileOpen.OpenCmdFileMruPriv

Taj događaj označava da Office Word otvara dokument s popisa nedavno korištenih dokumenata (MRU). Sadrži i ključne podatke o performansama otvaranja datoteka, a iz perspektive korisnika predstavlja događaj pokretanja aplikacije. Događaj nadzire funkcionira li otvaranje datoteka s MRU-a prema očekivanjima. Koristi se i za izračunavanje broja mjesečnih aktivnih korisnika/uređaja i metriku pouzdanosti oblaka.

Prikupljaju se sljedeća polja:

- **Data_AddDocTelemRes** – Izvještava jesmo li u slučaju uspjeli pravilno popuniti druge vrijednosti povezane s telemetrijom dokumenta. Koristi se za dijagnostiku kvalitete podataka.

- **Data_BytesAsynchronous** – broj (sažetih) bajtova za koje vjerujemo da možemo otvoriti datoteku bez njih ako ih dobijemo prije nego što korisnik poželi početi uređivati ili možda spremati

- **Data_BytesAsynchronousWithWork** – broj (sažetih) bajtova bez kojih bismo možda mogli otvoriti datoteku, ali bi to zahtijevalo značajna ulaganja u kod

- **Data_BytesSynchronous** – broj (sažetih) bajtova koje moramo imati prije nego što možemo početi otvarati datoteku

- **Data_BytesUnknown** – broj bajtova u dijelovima dokumenta koje ne očekujemo pronaći 

- **Data_DetachedDuration** – koliko je dugo aktivnost bila odvojena od niti

- **Data_Doc_AccessMode** – dokument je samo za čitanje/uređivanje

- **Data_Doc_AssistedReadingReasons** – unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

- **Data_Doc_AsyncOpenKind –** označava je li otvorena predmemorirana verzija dokumenta u oblaku i koja je logika za asinkrono osvježavanje korištena.

- **Data_Doc_ChunkingType** – jedinice koje se koriste za inkrementalno otvaranje dokumenta

- **Data_Doc_EdpState** – postavka zaštite elektroničkih podataka za dokument

- **Data_Doc_Ext** – nastavak dokumenta (docx/xlsb/pptx itd.)

- **Data_Doc_FileFormat** – verzija protokola oblika datoteke

- **Data_Doc_Fqdn** – naziv domene servisa OneDrive ili sustava SharePoint Online

- **Data_Doc_FqdnHash** – jednosmjerno raspršivanje naziva domene koji identificira korisnika

- **Data_Doc_IdentityTelemetryId** – jednosmjerno raspršivanje korisničkog identiteta kojim se izvršava otvaranje

- **Data_Doc_InitializationScenario** – bilježi način otvaranja dokumenta

- **Data_Doc_IOFlags** – izvješćuje o predmemoriranim zastavicama za postavljanje mogućnosti zahtjeva

- **Data_Doc_IrmRights** – radnje koje dopuštaju pravila zaštite elektroničkih podataka koja su primijenjena na dokument/korisnika

- **Data_Doc_IsIncrementalOpen** – zastavica koja označava da je dokument inkrementalno otvoren

- **Data_Doc_IsOcsSupported** – zastavica koja označava da je dokument podržan u servisu za suradnju

- **Data_Doc_IsOpeningOfflineCopy** – zastavica koja označava da je otvorena izvanmrežna kopija dokumenta

- **Data_Doc_IsSyncBacked** – zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

- **Data_Doc_Location** – označava koji je servis pružio dokument (OneDrive, File Server, SharePoint itd.)

- **Data_Doc_LocationDetails** – označava koja je poznata mapa pružila lokalno pohranjeni dokument

- **Data_Doc_NumberCoAuthors** – broj drugih korisnika u sesiji zajedničkog uređivanja

- **Data_Doc_PasswordFlags** – označava postavljene zastavice za čitanje/pisanje lozinke

- **Data_Doc_ReadOnlyReasons** – razlozi zbog kojih je dokument otvoren samo za čitanje

- **Data_Doc_ResourceIdHash** – anonimizirani identifikator dokumenta za dijagnosticiranje problema

- **Data_Doc_RtcType** – označava kako je postavljen kanal u stvarnom vremenu (RTC) za trenutnu datoteku (Onemogućeno, nepodržano, na zahtjev, uvijek uključeno itd.).

- **Data_Doc_ServerDocId** – nepromjenjivi anonimizirani identifikator dokumenta za dijagnosticiranje problema 

- **Data_Doc_ServerProtocol** – verzija protokola za komuniciranje sa servisom

- **Data_Doc_ServerType** – vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.)

- **Data_Doc_ServerVersion** – verzija poslužitelja koji pruža servis

- **Data_Doc_SessionId** – označava određenu sesiju uređivanja dokumenta u cijeloj sesiji

- **Data_Doc_SharePointServiceContext** – dijagnostičke informacije iz zahtjeva sustava SharePoint Online

- **Data_Doc_SizeInBytes** – pokazatelj veličine dokumenta

- **Data_Doc_SpecialChars** – pokazatelj posebnih znakova u URL-u dokumenta 

- **Data_Doc_SyncBackedType** – pokazatelj vrste dokumenta (lokalni ili na servisu)

- **Data_Doc_UrlHash** – jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta

- **Data_Doc_WopiServiceId** – sadrži jedinstveni identifikator davatelja usluga WOPI

- **Data_EditorDisablingRename** – identifikator prvog uređivača koji je uzrokovao onemogućivanje preimenovanja

- **Data_EditorsCount** – broj uređivača dokumenta

- **Data_ForceReadWriteReason** – cijeli broj koji predstavlja razlog zbog kojeg je datoteka prisilno prebačena u način rada za čitanje/pisanje

- **Data_FSucceededAfterRecoverableFailure** – označava da je otvaranje uspjelo nakon popravljanja neuspjelog otvaranja dokumenta

- **Data_LastLoggedTag** – jedinstvena oznaka mjesta pozivanja koda, koja se koristi za identifikaciju dvokratnog neuspjelog pokušaja otvaranja (koristi se za dijagnostiku kvalitete podataka)

- **Data_LinkStyles** – označava povezujemo li se sa stilovima predloška

- **Data_MainPdod** – identifikator dokumenta u sklopu procesa Office Word

- **Data_Measurements** – šifrirani niz koji sadrži analizu trajanja različitih dijelova otvaranja. Koristi se za mjerenje performansi.

- **Data_MoveDisabledReason** – pogreška koja onemogućuje premještanje dokumenta

- **Data_MoveFlightEnabled** – je li omogućena testna verzija za značajku premještanja

- **Data_PartsUnknown** – broj dijelova dokumenta za koje nismo mogli pribaviti podatke

- **Data_RecoverableFailureInitiationLocationTag** – jedinstvena oznaka mjesta pozivanja koda, koja se koristi za identifikaciju mjesta na kojem pokušavamo popraviti datoteku prije otvaranja

- **Data_RenameDisabledReason** – pogreška koja uzrokuje onemogućivanje preimenovanja za taj dokument

- **Data_RenameFlightEnabled** – je li omogućena testna verzija za značajku preimenovanja

- **Data_SecondaryTag** – jedinstvena oznaka mjesta pozivanja koda, koja se koristi za dodavanje dodatnih podataka o neuspjelom otvaranju 

- **Data_TemplateFormat** – oblik datoteke predloška na kojem se dokument temelji.

- **Data_UsesNormal** – označava temelji li se otvoreni dokument na predlošku Normal

- **PathData_Doc_StreamAvailability** – pokazatelj je li niz dokumenata dostupan/onemogućen


#### <a name="officewordfileopenopenffileopenxstzcore"></a>Office.Word.FileOpen.OpenFFileOpenXstzCore

Taj događaj označava da Office Word otvara dokument koji je korisnik dvaput kliknuo. Sadrži i ključne podatke o performansama otvaranja datoteka, a iz perspektive korisnika predstavlja događaj pokretanja aplikacije. Događaj nadzire funkcionira li otvaranje datoteke dvostrukim klikom prema očekivanjima. Koristi se i za izračunavanje broja mjesečnih aktivnih korisnika/uređaja i metriku pouzdanosti oblaka.

Prikupljaju se sljedeća polja:

- **Data_AddDocTelemRes** – Izvještava jesmo li u slučaju uspjeli pravilno popuniti druge vrijednosti povezane s telemetrijom dokumenta. Koristi se za dijagnostiku kvalitete podataka
    
- **Data_BytesAsynchronous** – broj (sažetih) bajtova za koje vjerujemo da možemo otvoriti datoteku bez njih ako ih dobijemo prije nego što korisnik poželi početi uređivati ili možda spremati
    
- **Data_BytesAsynchronousWithWork** – broj (sažetih) bajtova bez kojih bismo možda mogli otvoriti datoteku, ali bi to zahtijevalo značajna ulaganja u kod

- **Data_BytesSynchronous** – broj (sažetih) bajtova koje moramo imati prije nego što možemo početi otvarati datoteku
    
- **Data_BytesUnknown** – broj bajtova u dijelovima dokumenta koje ne očekujemo pronaći

- **Data_DetachedDuration** – koliko je dugo aktivnost bila odvojena od niti

- **Data_Doc_AccessMode** – dokument je samo za čitanje/uređivanje

- **Data_Doc_AssistedReadingReasons** – unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

- **Data_Doc_AsyncOpenKind –** označava je li otvorena predmemorirana verzija dokumenta u oblaku i koja je logika za asinkrono osvježavanje korištena.

- **Data_Doc_ChunkingType** – jedinice koje se koriste za inkrementalno otvaranje dokumenta

- **Data_Doc_EdpState** – postavka zaštite elektroničkih podataka za dokument

- **Data_Doc_Ext** – nastavak dokumenta (docx/xlsb/pptx itd.)

- **Data_Doc_FileFormat** – verzija protokola oblika datoteke

- **Data_Doc_Fqdn** – naziv domene servisa OneDrive ili sustava SharePoint Online

- **Data_Doc_FqdnHash** – jednosmjerno raspršivanje naziva domene koji identificira korisnika

- **Data_Doc_IOFlags** – izvješćuje o predmemoriranim zastavicama za postavljanje mogućnosti zahtjeva

- **Data_Doc_IdentityTelemetryId** – jednosmjerno raspršivanje korisničkog identiteta kojim se izvršava otvaranje

- **Data_Doc_InitializationScenario** – bilježi način otvaranja dokumenta

- **Data_Doc_IrmRights** – radnje koje dopuštaju pravila zaštite elektroničkih podataka koja su primijenjena na dokument/korisnika

- **Data_Doc_IsIncrementalOpen** – zastavica koja označava da je dokument inkrementalno otvoren

- **Data_Doc_IsOcsSupported** – zastavica koja označava da je dokument podržan u servisu za suradnju
    
- **Data_Doc_IsOpeningOfflineCopy** – zastavica koja označava da je otvorena izvanmrežna kopija dokumenta

- **Data_Doc_IsSyncBacked** – zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

- **Data_Doc_Location** – označava koji je servis pružio dokument (OneDrive, File Server, SharePoint itd.)
    
- **Data_Doc_LocationDetails** – označava koja je poznata mapa pružila lokalno pohranjeni dokument

- **Data_Doc_NumberCoAuthors** – broj drugih korisnika u sesiji zajedničkog uređivanja

- **Data_Doc_PasswordFlags** – označava postavljene zastavice za čitanje/pisanje lozinke

- **Data_Doc_ReadOnlyReasons** – razlozi zbog kojih je dokument otvoren samo za čitanje

- **Data_Doc_ResourceIdHash** – anonimizirani identifikator dokumenta za dijagnosticiranje problema

- **Data_Doc_RtcType** – označava kako je postavljen kanal u stvarnom vremenu (RTC) za trenutnu datoteku (Onemogućeno, nepodržano, na zahtjev, uvijek uključeno itd.).

- **Data_Doc_ServerDocId** – nepromjenjivi anonimizirani identifikator dokumenta za dijagnosticiranje problema

- **Data_Doc_ServerProtocol** – verzija protokola za komuniciranje sa servisom

- **Data_Doc_ServerType** – vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.)
    
- **Data_Doc_ServerVersion** – verzija poslužitelja koji pruža servis 

- **Data_Doc_SessionId** – označava određenu sesiju uređivanja dokumenta u cijeloj sesiji

- **Data_Doc_SharePointServiceContext** – dijagnostičke informacije iz zahtjeva sustava SharePoint Online

- **Data_Doc_SizeInBytes** – pokazatelj veličine dokumenta

- **Data_Doc_SpecialChars** – pokazatelj posebnih znakova u URL-u ili putu dokumenta

- **Data_Doc_StreamAvailability** – pokazatelj je li niz dokumenata dostupan/onemogućen

- **Data_Doc_SyncBackedType** – pokazatelj vrste dokumenta (lokalni ili na servisu)

- **Data_Doc_UrlHash** – jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta

- **Data_Doc_WopiServiceId** – sadrži jedinstveni identifikator davatelja usluga WOPI

- **Data_EditorDisablingRename** – identifikator prvog uređivača koji je uzrokovao onemogućivanje preimenovanja

- **Data_EditorsCount** – broj uređivača dokumenta

- **Data_FSucceededAfterRecoverableFailure** – označava da je otvaranje uspjelo nakon popravljanja neuspjelog otvaranja dokumenta

- **Data_ForceReadWriteReason** – cijeli broj koji predstavlja razlog zbog kojeg je datoteka prisilno prebačena u način rada za čitanje/pisanje
    
- **Data_LastLoggedTag** – jedinstvena oznaka mjesta pozivanja koda, koja se koristi za identifikaciju dvokratnog neuspjelog pokušaja otvaranja (koristi se za dijagnostiku kvalitete podataka)

- **Data_LinkStyles** – označava povezujemo li se sa stilovima predloška

- **Data_MainPdod** – identifikator dokumenta u sklopu procesa Office Word

- **Data_Measurements** – šifrirani niz koji sadrži analizu trajanja različitih dijelova otvaranja. Koristi se za mjerenje performansi.
    
- **Data_MoveDisabledReason** – pogreška koja onemogućuje premještanje dokumenta

- **Data_MoveFlightEnabled** – je li omogućena testna verzija za značajku premještanja

- **Data_PartsUnknown** – broj dijelova dokumenta za koje nismo mogli pribaviti podatke

- **Data_RecoverableFailureInitiationLocationTag** – jedinstvena oznaka mjesta pozivanja koda, koja se koristi za identifikaciju mjesta na kojem pokušavamo popraviti datoteku prije otvaranja.

- **Data_RenameDisabledReason** – pogreška koja uzrokuje onemogućivanje preimenovanja za taj dokument

- **Data_RenameFlightEnabled** – je li omogućena testna verzija za značajku preimenovanja

- **Data_SecondaryTag** – jedinstvena oznaka mjesta pozivanja koda, koja se koristi za dodavanje dodatnih podataka o neuspjelom otvaranju.

- **Data_TemplateFormat** – oblik datoteke predloška na kojem se dokument temelji.

- **Data_UsesNormal** – označava temelji li se otvoreni dokument na predlošku Normal.


#### <a name="officewordfileopenopenifrinitargs"></a>Office.Word.FileOpen.OpenIfrInitArgs

Taj događaj označava da Office Word otvara dokument putem COM aktivacije ili naredbenog retka. Sadrži i ključne podatke o performansama otvaranja datoteka, a iz perspektive korisnika predstavlja događaj pokretanja aplikacije. Događaj nadzire funkcionira li otvaranje datoteka iz naredbenog retka prema očekivanjima. Koristi se i za izračunavanje broja mjesečnih aktivnih korisnika/uređaja i metriku pouzdanosti oblaka.

Prikupljaju se sljedeća polja:

  - **Data\_AddDocTelemRes –** izvješćuje jesmo li mogli pravilno popuniti ostale vrijednosti vezane uz telemetriju dokumenta u sklopu događaja. Koristi se za dijagnostiku kvalitete podataka.

  - **Data\_BytesAsynchronous –** broj (sažetih) bajtova za koje vjerujemo da možemo otvoriti datoteku bez njih ako ih dobijemo prije nego što korisnik poželi početi uređivati ili možda spremati.

  - **Data\_BytesAsynchronousWithWork –** broj (sažetih) bajtova bez kojih bismo možda mogli otvoriti datoteku, ali bi to zahtijevalo značajna ulaganja u kod

  - **Data\_BytesSynchronous –** broj (sažetih) bajtova koje moramo imati prije nego što možemo početi otvarati datoteku

  - **Data\_BytesUnknown –** broj bajtova u dijelovima dokumenta koje ne očekujemo pronaći.

  - **Data\_Doc\_AccessMode –** dokument je samo za čitanje ili za uređivanje

  - **Data\_Doc\_AssistedReadingReasons –** unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

  - **Data_Doc_AsyncOpenKind –** označava je li otvorena predmemorirana verzija dokumenta u oblaku i koja je logika za asinkrono osvježavanje korištena.

  - **Data\_Doc\_ChunkingType –** jedinice korištene za inkrementalno otvaranje dokumenta

  - **Data\_Doc\_EdpState –** postavka zaštite elektroničkih podataka za dokument

  - **Data\_Doc\_Ext –** nastavak dokumenta (docx/xlsb/pptx itd.)

  - **Data\_Doc\_FileFormat –** verzija protokola za oblik datoteke

  - **Data\_Doc\_Fqdn –** naziv domene servisa OneDrive ili sustava SharePoint Online

  - **Data\_Doc\_FqdnHash –** jednosmjerno raspršivanje naziva domene koji identificira korisnika

  - **Data\_Doc\_IOFlags –** izvješćuje o predmemoriranim zastavicama korištenima za postavljanje mogućnosti otvorenog zahtjeva

  - **Data\_Doc\_IdentityTelemetryId –** jednosmjerno raspršivanje korisničkog identiteta koji se koristio za otvaranje

  - **Data\_Doc\_InitializationScenario –** bilježi način otvaranja dokumenta

  - **Data\_Doc\_IrmRights –** radnje dopuštene pravilima zaštite elektroničkih podataka primijenjenima na dokument/korisnika

  - **Data\_Doc\_IsIncrementalOpen –** zastavica koja označava da je dokument inkrementalno otvoren

  - **Data\_Doc\_IsOcsSupported –** zastavica koja označava da je dokument podržan u servisu za suradnju

  - **Data\_Doc\_IsOpeningOfflineCopy –** zastavica koja označava da je otvorena izvanmrežna kopija dokumenta

  - **Data\_Doc\_IsSyncBacked –** zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

  - **Data\_Doc\_Location –** označava koji je servis dobavio dokument (OneDrive, File Server, SharePoint)

  - **Data\_Doc\_LocationDetails –** označava koja je poznata mapa dobavila lokalno pohranjeni dokument

  - **Data\_Doc\_NumberCoAuthors –** broj drugih korisnika u sesiji zajedničkog uređivanja

  - **Data\_Doc\_PasswordFlags –** označava postavljene zastavice za čitanje ili čitanje i pisanje lozinke

  - **Data\_Doc\_ReadOnlyReasons –** razlozi zbog kojih je dokument otvoren samo za čitanje

  - **Data\_Doc\_ResourceIdHash –** anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

  - **Data_Doc_RtcType –** označava kako je kanal u stvarnom vremenu (RTC) postavljen za trenutnu datoteku (onemogućen, nepodržan, na zahtjev, uvijek uključen itd.).

  - **Data\_Doc\_ServerDocId –** nepromjenjivi anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

  - **Data\_Doc\_ServerProtocol –** verzija protokola korištena za komuniciranje sa servisom

  - **Data\_Doc\_ServerType –** vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.)

  - **Data\_Doc\_ServerVersion –** verzija poslužitelja koji pruža servis

  - **Data\_Doc\_SessionId –** verzija poslužitelja koji pruža servis

  - **Data\_Doc\_SharePointServiceContext –** dijagnostičke informacije iz zahtjeva sustava SharePoint Online

  - **Data\_Doc\_SizeInBytes –** pokazatelj veličine dokumenta

  - **Data\_Doc\_SpecialChars –** pokazatelj posebnih znakova u URL–u ili putu dokumenta

  - **Data\_Doc\_StreamAvailability –** pokazatelj je li tok dokumenta dostupan/onemogućen

  - **Data\_Doc\_SyncBackedType –** pokazatelj vrste dokumenta (lokalni ili na servisu)

  - **Data\_Doc\_UrlHash –** jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta

  - **Data\_Doc\_WopiServiceId –** sadrži jedinstveni identifikator davatelja usluge WOPI

  - **Data\_EditorDisablingRename –** identifikator prvog uređivača koji je uzrokovao onemogućivanje preimenovanja

  - **Data\_EditorsCount –** broj uređivača dokumenta

  - **Data\_FSucceededAfterRecoverableFailure –** označava da je otvaranje uspjelo nakon popravljanja neuspjelog otvaranja dokumenta

  - **Data\_ForceReadWriteReason –** cijeli broj koji predstavlja razlog zbog kojeg je datoteka prisilno prebačena u način rada za čitanje/pisanje

  - **Data\_LastLoggedTag –** jedinstvena oznaka mjesta pozivanja koda, koja se koristi za identifikaciju dvokratnog neuspjelog pokušaja otvaranja (koristi se za dijagnostiku kvalitete podataka)

  - **Data\_LinkStyles –** označava povezujemo li se sa stilovima predloška

  - **Data\_MainPdod –** identifikator dokumenta u sklopu procesa Office Word

  - **Data\_Measurements –** šifrirani niz koji sadrži analizu trajanja različitih dijelova otvaranja. Koristi se za dijagnosticiranje performansi otvaranja.

  - **Data\_MoveDisabledReason –** pogreška koja onemogućuje premještanje dokumenta

  - **Data\_MoveFlightEnabled –** je li omogućena testna verzija za značajku premještanja

  - **Data\_PartsUnknown –** broj dijelova dokumenta za koje nismo mogli pribaviti podatke

  - **Data\_RecoverableFailureInitiationLocationTag –** jedinstvena oznaka mjesta pozivanja koda, koja se koristi za identifikaciju mjesta na kojem pokušavamo popraviti datoteku prije otvaranja

  - **Data\_RenameDisabledReason –** pogreška koja uzrokuje onemogućivanje preimenovanja za taj dokument

  - **Data\_RenameFlightEnabled –** je li omogućena testna verzija za značajku preimenovanja

  - **Data\_SecondaryTag –** jedinstvena oznaka mjesta pozivanja koda, koja se koristi za dodavanje dodatnih podataka o neuspjelom otvaranju.

  - **Data\_TemplateFormat –** oblik datoteke predloška na kojem se dokument temelji.

  - **Data\_UsesNormal –** označava temelji li se otvoreni dokument na predlošku Normal.


#### <a name="officewordfileopenopenloadfile"></a>Office.Word.FileOpen.OpenLoadFile

Taj događaj označava da Office Word otvara dokument putem dijaloškog okvira Otvaranje. Sadrži i ključne podatke o performansama otvaranja datoteka, a iz perspektive korisnika predstavlja događaj pokretanja aplikacije. Događaj nadzire funkcionira li otvaranje datoteke putem dijaloškog okvira Otvaranje prema očekivanjima. Koristi se i za izračunavanje broja mjesečnih aktivnih korisnika/uređaja i metriku pouzdanosti oblaka.

Prikupljaju se sljedeća polja:

- **Data_AddDocTelemRes** – Izvještava jesmo li u slučaju uspjeli pravilno popuniti druge vrijednosti povezane s telemetrijom dokumenta. Koristi se za dijagnostiku kvalitete podataka.

- **Data_BytesAsynchronous** – broj (sažetih) bajtova za koje vjerujemo da možemo otvoriti datoteku bez njih ako ih dobijemo prije nego što korisnik poželi početi uređivati ili možda spremati

- **Data_BytesAsynchronousWithWork** – broj (sažetih) bajtova bez kojih bismo možda mogli otvoriti datoteku, ali bi to zahtijevalo značajna ulaganja u kod
    
- **Data_BytesSynchronous** – broj (sažetih) bajtova koje moramo imati prije nego što možemo početi otvarati datoteku

- **Data_BytesUnknown** – broj bajtova u dijelovima dokumenta koje ne očekujemo pronaći

- **Data_DetachedDuration** – koliko je dugo aktivnost bila odvojena od niti

- **Data_Doc_AccessMode** – dokument je samo za čitanje/uređivanje

- **Data_Doc_AssistedReadingReasons** – unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

- **Data_Doc_AsyncOpenKind –** označava je li otvorena predmemorirana verzija dokumenta u oblaku i koja je logika za asinkrono osvježavanje korištena.

- **Data_Doc_ChunkingType** – jedinice koje se koriste za inkrementalno otvaranje dokumenta

- **Data_Doc_EdpState** – postavka zaštite elektroničkih podataka za dokument

- **Data_Doc_Ext** – nastavak dokumenta (docx/xlsb/pptx itd.)

- **Data_Doc_FileFormat** – verzija protokola oblika datoteke

- **Data_Doc_Fqdn** – naziv domene servisa OneDrive ili sustava SharePoint Online

- **Data_Doc_FqdnHash** – jednosmjerno raspršivanje naziva domene koji identificira korisnika

- **Data_Doc_IdentityTelemetryId** – jednosmjerno raspršivanje korisničkog identiteta kojim se izvršava otvaranje

- **Data_Doc_InitializationScenario** – bilježi način otvaranja dokumenta

- **Data_Doc_IOFlags** – izvješćuje o predmemoriranim zastavicama za postavljanje mogućnosti zahtjeva

- **Data_Doc_IrmRights** – radnje koje dopuštaju pravila zaštite elektroničkih podataka koja su primijenjena na dokument/korisnika
    
- **Data_Doc_IsIncrementalOpen** – zastavica koja označava da je dokument inkrementalno otvoren

- **Data_Doc_IsOcsSupported** – zastavica koja označava da je dokument podržan u servisu za suradnju

- **Data_Doc_IsOpeningOfflineCopy** – zastavica koja označava da je otvorena izvanmrežna kopija dokumenta

- **Data_Doc_IsSyncBacked** – zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

- **Data_Doc_Location** – označava koji je servis pružio dokument (OneDrive, File Server, SharePoint itd.)

- **Data_Doc_LocationDetails** – označava koja je poznata mapa pružila lokalno pohranjeni dokument

- **Data_Doc_NumberCoAuthors** – broj drugih korisnika u sesiji zajedničkog uređivanja

- **Data_Doc_PasswordFlags** – označava postavljene zastavice za čitanje/pisanje lozinke

- **Data_Doc_ReadOnlyReasons** – razlozi zbog kojih je dokument otvoren samo za čitanje

- **Data_Doc_ResourceIdHash** – anonimizirani identifikator dokumenta za dijagnosticiranje problema

- **Data_Doc_RtcType** – označava kako je postavljen kanal u stvarnom vremenu (RTC) za trenutnu datoteku (Onemogućeno, nepodržano, na zahtjev, uvijek uključeno itd.).

- **Data_Doc_ServerDocId** – nepromjenjivi anonimizirani identifikator dokumenta za dijagnosticiranje problema 

- **Data_Doc_ServerProtocol** – verzija protokola za komuniciranje sa servisom

- **Data_Doc_ServerType** – vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.)

- **Data_Doc_ServerVersion** – verzija poslužitelja koji pruža servis

- **Data_Doc_SessionId** – označava određenu sesiju uređivanja dokumenta u cijeloj sesiji

- **Data_Doc_SharePointServiceContext** – dijagnostičke informacije iz zahtjeva sustava SharePoint Online

- **Data_Doc_SizeInBytes** – pokazatelj veličine dokumenta

- **Data_Doc_SpecialChars** – pokazatelj posebnih znakova u URL-u ili putu dokumenta

- **Data_Doc_StreamAvailability** – pokazatelj je li niz dokumenata dostupan/onemogućen

- **Data_Doc_SyncBackedType** – pokazatelj vrste dokumenta (lokalni ili na servisu)

- **Data_Doc_UrlHash** – jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta

- **Data_EditorDisablingRename** – identifikator prvog uređivača koji je uzrokovao onemogućivanje preimenovanja

- **Data_EditorsCount** – broj uređivača dokumenta

- **Data_ForceReadWriteReason** – cijeli broj koji predstavlja razlog zbog kojeg je datoteka prisilno prebačena u način rada za čitanje/pisanje
    
- **Data_FSucceededAfterRecoverableFailure** – označava da je otvaranje uspjelo nakon popravljanja neuspjelog otvaranja dokumenta

- **Data_LastLoggedTag** – jedinstvena oznaka mjesta pozivanja koda, koja se koristi za identifikaciju dvokratnog neuspjelog pokušaja spremanja (koristi se za dijagnostiku kvalitete podataka)

- **Data_LinkStyles** – označava povezujemo li se sa stilovima predloška

- **Data_MainPdod** – identifikator dokumenta u sklopu procesa Office Word

- **Data_Measurements** – šifrirani niz koji sadrži analizu trajanja različitih dijelova otvaranja. Koristi se za mjerenje performansi.

- **Data_MoveDisabledReason** – pogreška koja onemogućuje premještanje dokumenta

- **Data_MoveFlightEnabled** – je li omogućena testna verzija za značajku premještanja

- **Data_PartsUnknown** – broj dijelova dokumenta za koje nismo mogli pribaviti podatke

- **Data_RecoverableFailureInitiationLocationTag** – jedinstvena oznaka mjesta pozivanja koda, koja se koristi za identifikaciju mjesta na kojem pokušavamo popraviti datoteku prije otvaranja

- **Data_RenameDisabledReason** – pogreška koja uzrokuje onemogućivanje preimenovanja za taj dokument

- **Data_RenameFlightEnabled** – je li omogućena testna verzija za značajku preimenovanja

- **Data_SecondaryTag** – jedinstvena oznaka mjesta pozivanja koda, koja se koristi za dodavanje dodatnih podataka o neuspjelom otvaranju

- **Data_TemplateFormat** – oblik datoteke predloška na kojem se dokument temelji

- **Data_UsesNormal** – označava temelji li se otvoreni dokument na predlošku Normal


#### <a name="renewuserop"></a>RenewUserOp

Prikuplja se kada korisnik pokuša otvoriti dokument zaštićen IRM-om ili primijeniti zaštite IRM-a.  Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada se provodi operacija obnavljanja korisničkih certifikata. 

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere

- **AppInfo.Name** – naziv aplikacije.

- **AppInfo.Version** – verzija aplikacije

- **iKey** – identifikacijski broj poslužitelja zapisnika

- **RMS.ApplicationScenarioId** – identifikacijski broj scenarija koji pruža aplikacija

- **RMS.Duration** – ukupno vrijeme potrebno za dovršavanje operacije

- **RMS.DurationWithoutExternalOps** – ukupno vrijeme umanjeno za potrošene vanjske operacije poput latencije mreže.

- **RMS.ErrorCode** – kod pogreške koji, ako postoji, vraća operacija

- **RMS.HttpCall** – označava postoji li operacija HTTP-a

- **RMS.LicenseFormat** – format licence: Xrml ili Json

- **RMS.Result** – uspjeh ili neuspjeh operacije

- **RMS.ScenarioId** – identifikacijski broj scenarija koji definira klijent usluge upravljanja pravima

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

- **RMS.ServerType** – vrsta poslužitelja usluge upravljanja pravima 

- **RMS.StatusCode** – kod statusa rezultata operacije

- **RMS.Type** – vrsta informacija o korisniku

#### <a name="servicediscoveryop"></a>ServiceDiscoveryOp

Prikuplja se kada korisnik pokuša otvoriti dokument zaštićen IRM-om ili primijeniti zaštite IRM-a.  Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada se provodi operacija otkrivanja usluge. 

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere

- **AppInfo.Name** – naziv aplikacije.

- **AppInfo.Version** – verzija aplikacije

- **iKey** – identifikacijski broj poslužitelja pružatelja usluge zapisivanja

- **RMS.ApplicationScenarioId** – identifikacijski broj scenarija koji pruža aplikacija

- **RMS.Duration** – ukupno vrijeme potrebno za dovršavanje operacije

- **RMS.DurationWithoutExternalOps** – ukupno vrijeme umanjeno za potrošene vanjske operacije poput latencije mreže.

- **RMS.ErrorCode** – kod pogreške koji, ako postoji, vraća operacija

- **RMS.HttpCall** – označava postoji li operacija HTTP-a

- **RMS.LicenseFormat** – format licence: Xrml ili Json

- **RMS.OperationName** – naziv operacije

- **RMS.Result** – uspjeh ili neuspjeh operacije

- **RMS.ScenarioId** – identifikacijski broj scenarija koji definira klijent usluge upravljanja pravima

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

- **RMS.ServerType** – vrsta poslužitelja usluge upravljanja pravima 

- **RMS.StatusCode** – kod statusa rezultata operacije


### <a name="office-accessibility-configuration-subtype"></a>*Podvrsta konfiguracije pristupačnosti za Office*

Značajke pristupačnosti u sustavu Office

#### <a name="officeaccessibilityaccessibilitytoolsessionpresencewin32"></a>Office.Accessibility.AccessibilityToolSessionPresenceWin32

Omogućuje otkrivanje ima li korisnik alat za pomoćne tehnologije i kako se taj alat zove. To nam omogućuje razumjeti ima li korisnik sustava Office problema s određenim alatom za pomoćne tehnologije.

Prikupljaju se sljedeća polja:

  - **Data\_Data\_Jaws –** označava je li Jaws bio pokrenut tijekom sesije **Data\_Data\_Magic –** označava je li Magic bio pokrenut tijekom sesije

  - **Data\_Data\_Magnify –** označava je li Povećavanje bilo pokrenuto tijekom sesije

  - **Data\_Data\_Narrator –** označava je li Pripovjedač bio pokrenut tijekom sesije

  - **Data\_Data\_NVDA –** označava je li NVDA bila pokrenuta tijekom sesije

  - **Data\_Data\_SA –** označava je li SA bila pokrenuta tijekom sesije

  - **Data\_Data\_Supernova –** označava je li Supernova bila pokrenuta tijekom sesije

  - **Data\_Data\_SuperNovaessSuite –** označava je li SuperNovaAccessSuite bio pokrenut tijekom sesije

  - **Data\_Data\_WinEyes –** označava je li WinEyes bio pokrenut tijekom sesije

  - **Data\_Data\_ZoomText –** označava je li ZoomText bio pokrenut tijekom sesije

#### <a name="officeappledarkmode"></a>Office.Apple.DarkMode

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj nam govori je li korisnik pokrenuo sustav u Tamnom načinu i je li korisnik prepisao postavke sustava Tamni način u sustavu Office.  Koristimo ovaj događaj da bismo vam pomogli osigurati pristupačnost i odredili prioritete optimizacije korisničkog iskustva.

Prikupljaju se sljedeća polja:

- **Data_DarkModeIsEnabled** – je li Tamni način omogućen u sustavu.

- **Data_RequiresAquaSystemAppearanceEnabled** – je li Tamni način prepisan u sustav Office.

#### <a name="officeapplehardwarekeyboardinuseapple"></a>Office.Apple.HardwareKeyboardInUse.Apple

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj nam govori da korisnik priključuje tipkovnicu na svoj mobilni uređaj. Događaj nam pomaže poboljšati pristupačnost i optimizirati korisničko iskustvo.

Prikupljaju se sljedeća polja:

- **Data_CollectionTime**– vremenska oznaka koja označava vrijeme prikupljanja događaja.

#### <a name="officeapplembuinstrumentdeviceaccessibilitysettings"></a>Office.Apple.MbuInstrument.DeviceAccessibilitySettings

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj prikuplja stanje različitih mogućnosti pristupačnosti dostupnih tijekom sesije. Koristimo ovaj događaj da bismo vam pomogli osigurati pristupačnost i odredili prioritete optimizacije korisničkog iskustva.

Prikupljaju se sljedeća polja:

- **Data_AccessibilityContentSize** – zastavica koja upućuje na to je li postavka omogućena

- **Data_AssistiveTouchRunning** – zastavica koja upućuje na to je li postavka omogućena

- **Data_BoldTextEnabled** – zastavica koja upućuje na to je li postavka omogućena

- **Data_CollectionTime** – zastavica koja upućuje na to je li postavka omogućena

- **Data_DarkerSystemColorsEnabled** – zastavica koja upućuje na to je li postavka omogućena

- **Data_DifferentiateWithoutColor** – zastavica koja upućuje na to je li postavka omogućena

- **Data_GrayscaleEnabled** – zastavica koja upućuje na to je li postavka omogućena

- **Data_GuidedAccessEnabled** – zastavica koja upućuje na to je li postavka omogućena

- **Data_IncreaseContrast** – zastavica koja upućuje na to je li postavka omogućena

- **Data_InvertColorsEnabled** – zastavica koja upućuje na to je li postavka omogućena

- **Data_PreferredContentSizeCategory** – zastavica koja upućuje na to je li postavka omogućena

- **Data_ReduceMotionEnabled** – zastavica koja upućuje na to je li postavka omogućena

- **Data_ReduceTransparency** – zastavica koja upućuje na to je li postavka omogućena

- **Data_ReduceTransparencyEnabled** – zastavica koja upućuje na to je li postavka omogućena

- **Data_ShakeToUndeEnabled** – zastavica koja upućuje na to je li postavka omogućena. (Zastarjelo – koristi se samo na starim međuverzijama).

- **Data_ShakeToUndoEnabled** – zastavica koja upućuje na to je li postavka omogućena.

- **Data_SpeakScreenEnabled** – zastavica koja upućuje na to je li postavka omogućena

- **Data_SpeakSelectionEnabled** – zastavica koja upućuje na to je li postavka omogućena

- **Data_SwitchControlRunning** – zastavica koja upućuje na to je li postavka omogućena

- **Data_UAZoomEnabled** – zastavica koja upućuje na to je li postavka omogućena

- **Data_VoiceOverRunning** – zastavica koja upućuje na to je li postavka omogućena

#### <a name="officewordaccessibilitylearningtoolsreadaloudplayreadaloud"></a>Office.Word.Accessibility.LearningTools.ReadAloud.PlayReadAloud

Taj događaj označava da Office Word naglas čita tekst u dokumentu. Taj je događaj impuls za značajku pristupačnosti koji Microsoftu omogućuje procjenu stanja značajke čitanja teksta naglas.

Prikupljaju se sljedeća polja:

  - **Data\_ParagraphCount –** broj odlomaka u dokumentu

  - **Data\_Play –** je li to prvi put da Word čita naglas

  - **Data\_ViewKind –** prikaz vrste dokumenta

#### <a name="officewordaccessibilitylearningtoolsreadaloudstopreadaloud"></a>Office.Word.Accessibility.LearningTools.ReadAloud.StopReadAloud

Taj događaj označava da Office Word prestaje naglas čitati tekst u dokumentu. Taj događaj Microsoftu omogućuje procjenu stanja značajke čitanja teksta naglas mjerenjem trajanja funkcioniranja.

Prikupljaju se sljedeća polja:

  - Nijedno

### <a name="privacy-subtype"></a>*Podvrsta zaštite privatnosti*

Postavke zaštite privatnosti u sustavu Office 

#### <a name="officeintelligentserviceprivacyconsentprivacyevent"></a>Office.IntelligentService.PrivacyConsent.PrivacyEvent

Ovaj događaj predstavlja radnju pokrenutu od strane korisnika ili sustava koja je dio korisničkog iskustva zaštite privatnosti za Office. Pokreće se u dijaloškim okvirima zaštite privatnosti Prvog pokretanja, dijaloškom okviru za zaštitu privatnosti računa i obavijestima o zaštiti privatnosti. Događaj se koristi za razumijevanje sljedećeg: korisnici pristaju na postavke zaštite privatnosti sustava Office, korisnici mijenjaju postavke zaštite privatnosti sustava Office i postavke zaštite privatnosti sustava Office ažuriraju se u korisničkim sesijama.

Prikupljaju se sljedeća polja:

  - **Data_ActionId –** korisnička akcija u dijaloškom okviru za zaštitu privatnosti

  - **Data_ControllerConnectedServicesState –** postavka korisničkih pravila za dodatna neobavezna povezana iskustva

  - **Data_DownloadedContentServiceGroupState –** korisnička postavka za preuzeti sadržaj 
 
  - **Data_ForwardLinkId –** veza za dokumentaciju o privatnosti za korisnički scenarij

  - **Data_HRESULT –** zapis o pogreškama tijekom interakcije s dijalogom zaštite privatnosti

  - **Data_IsEnterpriseUser –** kategorija korisničke licence

  - **Data_OfficeServiceConnectionState –** korisnička postavka za povezane usluge

  - **Data_RecordRegistry –** zapis o prikazivanje dijaloškog okvira privatnosti za veliku tvrtku

  - **Data_Scenario –** scenarij prvog pokretanja na temelju korisničke licence i kategorije

  - **Data_SeenInsidersDialog –** zapis o prikazivanje dijaloškog okvira privatnosti za program Insiders

  - **Data_SendTelemetryOption –** korisnička postavka za telemetriju

  - **Data_SendTelemetryOptionPolicy –** korisnička postavka pravilnika za telemetriju

  - **Data_UserCategory –** vrsta korisničkog računa  

  - **Data_UserCCSDisabled –** korisničko nadjačavanje za neobavezna povezana iskustva

   - **Data_UserContentServiceGroupState –** korisnička postavka za analizu sadržaja

  - **Data_WillShowDialogs –** zapis korisnika koji želi vidjeti dijaloške okvire privatnosti Prvog pokretanja



## <a name="product-and-service-performance-data-events"></a>Događaji koji se odnose na podatke o performansama proizvoda i usluga

Ovo su podvrste podataka u toj kategoriji:
- [Neočekivano zatvaranje (rušenje) aplikacije](#unexpected-application-exit-crash-subtype)
- [Performanse značajki aplikacije ](#application-feature-performance-subtype)
- [Pogreška aktivnosti aplikacije](#application-activity-error-subtype)

### <a name="unexpected-application-exit-crash-subtype"></a>*Podvrsta neočekivanog zatvaranja (rušenja) aplikacije*

Neočekivana zatvaranja aplikacija i stanje aplikacije kada se to dogodi.

#### <a name="appstartupreason"></a>app.startup.reason

Ovaj nam događaj omogućuje prepoznavanje i rješavanje problema zbog kojih se program Outlook srušio tijekom pokretanja aplikacije.  Ovaj događaj uključuje informacije o tome zašto je došlo do rušenja kako bismo brzo mogli riješiti ovaj problem.

Prikupljaju se sljedeća polja: 

- **app_background_time** – vrijeme tijekom kojeg je aplikacija u posljednjoj sesiji bila u pozadini

- **startup_reason_type** – označava razlog zašto se aplikacija pokreće, a to će označiti je li je bilo potrebno prisilno zaustaviti ili je bio posrijedi drugi razlog. 

- **watch_status_info** – prati sljedeće informacije, ako je primjenjivo. 

  - **is_watch_app_installed** – utvrđuje je li korisnik instalirao aplikaciju Watch

  - **is_watch_paired** – utvrđuje je li uređaj iOS uparen sa satom

  - **is_watch_supported_and_active** – označava ima li sat mogućnost podrške te je li aktivan tijekom sesije

Sljedeća se polja prikupljaju samo za Outlook Mobile za iOS:

- **clean_exit_reason** – niz riječi koji označava je li postojao razlog za zaustavljanje aplikacije

- **is_agenda_user** – označava je li korisnik nedavno otvorio raspored, što upućuje na to zapisuje li se na disk tijekom pokretanja

- **is_watch_supported_and_active** – označava ima li sat mogućnost podrške te je li aktivan tijekom sesije


#### <a name="applicationcrash"></a>application.crash

Koristi se za nadzor kritičnih rušenja aplikacije i pomaže nam prikupiti informacije o razlogu zašto se aplikacija srušila te kako to možemo spriječiti.

Prikupljaju se sljedeća polja: 

- **android.hardware.** – (na primjer, android.hardware.bluetooth) Vrijednosti konfiguracije hardvera koje pruža platforma Android

- **android.software.** – (npr. android.software.device_admin) Vrijednosti konfiguracije softvera koje pruža platforma Android

- **android_version** – naziv verzije sustava Android kao što označava android.os.Build.VERSION#RELEASE

- **application_package_name** – naziv paketa aplikacija kao što označava android.content.Context#getPackageName()

- **application_stack_trace** – snop praćenja rušenja

- **application_version_code** – kod verzije aplikacije koji je definirala aplikacija Outlook

- **application_version_name** – naziv verzije aplikacije koji je definirala aplikacija Outlook 

- **com.** (na primjer, com.google.android.feature.FASTPASS_BUILD, com.amazon.feature.PRELOAD, com.samsung.android.bio.face) Vrijednosti konfiguracije specifične za proizvođača koje je pružila platforma Android

- **crash_report_sdk** – SDK za slanje zapisnika o zatvaranju. Ili Hockey ili AppCenter

- **crash_type** – crash_type može biti: java, izvorni i koji nisu fatalni.

     - java – ako se zatvaranje zabilježi u aplikacijskom sloju.

     - izvorni – ako se zatvaranje zabilježi u okviru aplikacije. 

     - nije fatalni – zatvaranje se bilježi da bi se ispravila pogreška bilo koje značajke. Aplikacija se neće zatvoriti, ali će prenositi zapisnike o zatvaranju koji nisu fatalni da biste lakše mogu ispravljati pogreške na značajci.

- **device_brand** – marka uređaja (proizvođač ili nosač) kao što označava android.os.Build#BRAND

- **device_ID** – jedinstveni ID uređaja (IMEI)

- **device_manufacturer** – proizvođač uređaja kao što označava android.os.Build#MANUFACTURER

- **device_model** – model uređaja kao što označava android.os.Build#MODEL

- **device_name** – naziv uređaja kao što označava android.os.Build#DEVICE

- **device_total_memory** – procjena ukupne veličine memorije uređaja na temelju statistika datotečnog sustava.

- **glEsVersion** – ključ verzije ugrađenih sustava OpenGL Embedded


#### <a name="crashevent"></a>crash.event

Omogućuje nam prepoznavanje i ispravak situacija tijekom kojih je došlo do kritičnih rušenja aplikacije i pomaže nam prikupiti informacije o razlogu zašto se aplikacija srušila te kako to možemo spriječiti.

Prikupljaju se sljedeća polja: 

- **crashTime** – datum i vrijeme u koje se rušenje dogodilo kao pomoć tijekom istrage

- **crash_time_from_start** – proteklo vrijeme od pokretanja aplikacije do rušenja, kao pomoć tijekom istrage

- **exceptionName** – naziv iznimke koja je izazvala rušenje kao pomoć tijekom istrage

- **exception_reason** – naziv razloga koji je izazvao rušenje kao pomoć tijekom istrage

- **hasHx** – govori nam da račun koristi naš novi servis sinkronizacije kako bi nam pomogao prepoznati probleme uzrokovane našim servisom sinkronizacije

- **incidentIdentifier** – jedinstveni ID za izvješće o rušenju kako bismo mogli pronaći odgovarajući problem

- **isAppKill** – pomaže nam razumjeti je li ta aplikacija bila zaustavljena ili zatvorena na uređaju

- **is_crashloop** – pomaže nam razumjeti je li vjerojatno da je uzrok rušenja nastanak petlje rušenja.

- **reportKey** – jedinstveni ID za instalaciju aplikacije na uređaju za buduću istragu

- **signal** – signal koji je uzrokovao rušenje kako bi nam mogao pružiti više pojedinosti za istraživanje rušenja


#### <a name="error"></a>Error

Omogućuje nam razumijevanje problema s kojima se mobilne aplikacije suočavaju tijekom pokušavanja dohvaćanja postavki zaštite privatnosti s poslužitelja.

Prikupljaju se sljedeća polja:

- **correlationId** – jedinstveni identifikator za servisnu vezu koja je rezultirala pogreškom, što nam omogućuje što nije bilo u redu

- **errorCode** – prepoznaje relevantni kod pogreške primljen iz usluge koji se može koristiti za dijagnosticiranje problema

- **exceptionType** – vrsta pogreške koju je biblioteka prepoznala tijekom dohvaćanja postavke

- **message** – prepoznaje poruku o pogrešci primljenu od servisa

- **roamingSettingType** – označava mjesto s kojeg smo pokušali čitati postavke

- **settingId** – postavka koju se pokušalo dohvatiti

#### <a name="officeappdomainunhandledexceptionhandlerfailed"></a>Office.AppDomain.UnhandledExceptionHandlerFailed

Prikuplja informacije za sve neobrađene iznimke pomoću aplikacije Data Streamer. Ti se podaci koriste za praćenje stanja aplikacije. Taj događaj generira dodatak Microsoft Data Streamer za Excel.

Prikupljaju se sljedeća polja:

- **Iznimka** – poziv stogu zbog iznimke

- **Naziv događaja** – naziv događaja je kategorija i oznaka događaja.

#### <a name="officeappleidentitydomainname"></a>Office.Apple.IdentityDomainName

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za nadziranje stanja našeg sustava kao i za ispitivanje uzroka pogrešaka određenih korisnika domene. Prikupljamo domenu koju koriste naši korisnici prilikom provjere autentičnosti.  Te podatke koristimo za identificiranje i rješavanje onih problema koji se na širokoj razini možda ne čine previše utjecajni, ali koji ispadaju vrlo utjecajni za određenu domenu korisnika.

Prikupljaju se sljedeća polja:

- **Data_Domain** – domena koja se koristi za provjeru autentičnosti

- **Data_IdentityProvider** – naziv davatelja identiteta provjere autentičnosti. (odnosno LiveId ili ADAL)

- **Data_IdentityProviderEnum** – kôd davatelja identiteta provjere autentičnosti. (Broj)

#### <a name="officeapplesystemhealthappexitmacandios"></a>Office.Apple.SystemHealthAppExitMacAndiOS

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za nadziranje stanja aplikacija sustava Office kao i za ispitivanje uzroka pogrešaka. Prikupljamo podatke pri svakom izlazu iz aplikacije kako bismo utvrdili je li aplikacija zatvorena bez poteškoća.

Prikupljaju se sljedeća polja:

- **Data_AffectedProcessSessionID** – identifikator za sesiju koja ima izlaz iz aplikacije.

- **Data_AffectedSessionBuildNumber** – sporedna verzija aplikacije u kojoj je uočen izlaz iz aplikacije.

- **Data_AffectedSessionDuration** – duljina sesije od početka do kraja

- **Data_AffectedSessionIDSMatch** – pokazatelj stanja telemetrije.

- **Data_AffectedSessionMERPSessionID** – pokazatelj stanja telemetrije.

- **Data_AffectedSessionOSLocale** – regionalna shema OS-a na kojoj je uočen izlaz iz aplikacije.

- **Data_AffectedSessionOSVersion** – verzija OS-a u okviru koje je uočen izlaz iz aplikacije.

- **Data_AffectedSessionResidentMemoryOnCrash** – količina ugrađene memorije koja je potrošena kada je došlo do izlaza iz aplikacije

- **Data_AffectedSessionStackHash** – pokazatelj koji će označavati da je određena pogreška pogođena.

- **Data_AffectedSessionStartTime** – vrijeme početka sesije.

- **Data_AffectedSessionUAEType** – vrsta uočenog izlaza iz aplikacije (ako je bio izlaz bez poteškoća, taj će kôd označiti vrstu opažene pogreške)

- **Data_AffectedSessionVersion** – glavna verzija aplikacije u kojoj je uočen izlaz iz aplikacije.

- **Data_AffectedSessionVirtualMemoryOnCrash** – količina virtualne memorije koja je potrošena kada je došlo do izlaza iz aplikacije.

- **Data_ExitWasGraceful** – je li izlaz iz aplikacije bio bez poteškoća ili nije.

#### <a name="officeextensibilitycomaddinunhandledexception"></a>Office.Extensibility.COMAddinUnhandledException

Događaj koji se generira kad se COM dodatak sruši na potrošačkoj verziji aplikacija sustava Office. 

Ovo se upotrebljava se za izračun globalne „primjene” programa Microsoft 365 Apps za velike tvrtke za dodatak koji se zatim upotrebljava u drugim alatima, kao što je Readiness Toolkit. To korisnicima omogućuje da provjere valjanost dodataka koji su razmješteni u njihovim organizacijama u odnosu na kompatibilnost s najnovijim verzijama okruženja Microsoft 365 Apps za velike tvrtke te u skladu s tim planiraju njihove nadogradnje. 

Prikupljaju se sljedeća polja:

- **ScopeId** – doseg trenutne niti

- **Method** – metoda sustava Office u kojoj je došlo do iznimke

- **Interface** – sučelje sustava Office u kojem je došlo do iznimke

- **AddinId** – ID klase dodatka

- **AddinProgId** – ukinut

- **AddinFriendlyName** – ukinut

- **AddinTimeDateStamp** – vremenska oznaka dodatka iz metapodataka DLL-a

- **AddinVersion** – ukinut

- **AddinFileName** – ukinut

- **VSTOAddIn** – je li dodatak VSTO

- **AddinConnectFlag** – trenutno ponašanje učitavanja

- **LoadAttempts** – broj pokušaja učitavanja dodatka

#### <a name="officeextensibilitycomaddinunhandledexceptionenterprise"></a>Office.Extensibility.COMAddinUnhandledExceptionEnterprise

Događaj koji se stvara kad se COM dodatak sruši na verziji Enterprise aplikacija sustava Office.

Ovo se upotrebljava za izračun globalne „primjene” programa Microsoft 365 Apps za velike tvrtke za dodatak koji se zatim upotrebljava u drugim alatima, kao što je Readiness Toolkit. To korisnicima omogućuje da provjere valjanost dodataka koji su razmješteni u njihovim organizacijama u odnosu na kompatibilnost s najnovijim verzijama okruženja Microsoft 365 Apps za velike tvrtke te u skladu s tim planiraju njihove nadogradnje. 

- **ScopeId** – doseg trenutne niti

- **Method** – metoda sustava Office u kojoj je došlo do iznimke

- **Interface** – sučelje sustava Office u kojem je došlo do iznimke

- **AddinId** – ID klase dodatka

- **AddinProgId** – ukinut

- **AddinFriendlyName** – ukinut

- **AddinTimeDateStamp** – vremenska oznaka dodatka iz metapodataka DLL-a

- **AddinVersion** – ukinut

- **AddinFileName** – ukinut

- **VSTOAddIn** – je li dodatak VSTO

- **AddinConnectFlag** – trenutno ponašanje učitavanja

- **LoadAttempts** – broj pokušaja učitavanja dodatka

#### <a name="officeextensibilitysandboxodpactivationheartbeat"></a>Office.Extensibility.Sandbox.ODPActivationHeartbeat

Dodaci za Office pokreću se u testnom okruženju. Ovaj događaj prikuplja impulsne informacije o aktivacijama. Kada se dodatak sruši, taj događaj prikuplja razlog zašto se srušio u slučaju da je povezan s našim testnim okruženjem. Koristi se za istraživanje kada korisnici eskaliraju probleme.
 
Prikupljaju se sljedeća polja:

- **AppId** – ID aplikacije

- **AppInfo** – podaci koji se odnose na vrstu dodatka (okno zadatka ili UILess ili u sadržaju itd.) i vrstu pružatelja (omen, SharePoint, filesystem itd.)

- **AppInstanceId** – ID instance aplikacije 

- **AssetId** – ID sadržaja aplikacije

- **ErrorCode** – ukupno utrošeno vrijeme

- **IsAugmentationScenario** – upućuje na to je li augmentacijska petlja odgovorna za pokretanje kontrole Okvir s rješenjima sustava Office

- **IsDebug** – označava je li u pitanju sesija uklanjanje pogrešaka

- **IsPreload** – upućuje na to je li dodatak unaprijed učitan u pozadini radi poboljšanja performansi aktivacije.

- **IsWdagContainer** – upućuje na to odvija li se aktivacija dodatka u Application Guard spremniku programa Windows Defender.

- **NumberOfAddinsActivated** – brojač aktiviranih dodataka

- **RemoterType** – određuje vrstu daljinskog elementa (Trusted, untrusted, Win32webView, Trusted UDF itd.) koji se koristi za aktivaciju dodatka

- **StoreType** – porijeklo aplikacije

- **Tag**– određuje gdje točno kôd nije uspio pomoću jedinstvene oznake povezane s njim.

- **UsesSharedRuntime** – upućuje na to da koristi li aplikacija sharedRuntime ili ne.


#### <a name="officeextensibilityvbatelemetrybreak"></a>Office.Extensibility.VbaTelemetryBreak

Događaj koji se stvara kada datoteka s omogućenim makronaredbama naiđe na pogrešku pri kompiliranju ili izvođenju

Analitika za stolna računala: koristi se kao brojnik za izračun stanja vrsta makronaredbi (na primjer, makronaredbe za Word, Excel itd.) koje je specifično za velike tvrtke i koje se tijekom pilot-programa koristi da bi se zaključilo je li dodatak „spreman za nadogradnju” u produkcijskom okruženju.

Prikupljaju se sljedeća polja:

- **TagId** – ID telemetrijske oznake

- **BreakReason** – razlog zastoja (izvođenje, kompiliranje, druga pogreška)

- **SolutionType** – vrsta rješenja (dokument, predložak, dodatak za aplikaciju, COM dodatak)

- **Data.ErrorCode** – kod pogreške koji je prijavio VBA modul


#### <a name="officefindtimeappfailedtostart"></a>Office.FindTime.AppFailedToStart

Prikuplja se ako se aplikacija ne uspijeva pokrenuti zbog neočekivane pogreške prilikom pokretanja. Koristi se za praćenje iznimki i rušenja.  Omogućuje nadzor i ispravljanje pogrešaka stanja aplikacije.

Prikupljaju se sljedeća polja: 

- **DateTime** – vremenska oznaka zapisivanja događaja.

- **EventName** – naziv događaja koji se zapisuje.

#### <a name="officeoutlookdesktophangbucketmetrics"></a>Office.Outlook.Desktop.HangBucketMetrics

Prikuplja vrijeme blokiranja programa Outlook – jedinstveni identifikator po blokiranju, proteklom vremenu i informacijama o pozivanju stoga. Podaci se koriste za otkrivanje i identifikaciju rušenja aplikacije radi rješavanja problema u budućim ažuriranjima.

Prikupljaju se sljedeća polja:

  - **BucketId** – raspršivanje poziva stogu 

  - **ElapsedTotal** – ukupno vrijeme provedeno u pozivu

  - **ElapsedHanging** – vrijeme blokade provedeno u pozivu

#### <a name="officeoutlookdesktophangreportingscopeperfmetrics"></a>Office.Outlook.Desktop.HangReportingScopePerfMetrics

Prikuplja vrijeme potrebno za osnovne scenarije u programu Outlook – switchfolder, switchmodule, sendmailoutbox, openitemclassic, sendmailtransport. Aktivno se nadzire ima li u podacima problema s neuobičajenim performansama. Koristi se za otkrivanje i dijagnosticiranje problema s performansama, i za poboljšanje performansi sa svakim ažuriranjem.

Prikupljaju se sljedeća polja:

  - **ElapsedTotal** – ukupno vrijeme provedeno u tom pozivu

  - **ScopeId** – naziv funkcije koja sadrži deklaraciju ili prilagođeni naziv zadan putem definicije dosega

#### <a name="officeoutlookdesktopwatsonbuckets"></a>Office.Outlook.Desktop.WatsonBuckets

To pravilo prikuplja podatke o rušenju iz zapisnika događaja kada se Outlook srušio tijekom prethodne sesije.

Aktivno se nadzire ima li u podacima neuobičajenih blokada. Koristi se za otkrivanje i identifikaciju blokada radi rješavanja problema u budućim ažuriranjima.

Prikupljaju se sljedeća polja:

  - **BucketId** – raspršivanje poziva stogu

  - **ElapsedTotal** – ukupno vrijeme provedeno u pozivu

  - **ElapsedHanging** – vrijeme blokade provedeno u pozivu

#### <a name="officepowerpointsession"></a>Office.PowerPoint.Session

Prikupljanje korištenja značajki u svakoj sesiji programa PowerPoint. Ti se podaci koriste za izračun stope neočekivanih izlazaka iz programa PowerPoint prilikom korištenja značajke. Stopa neočekivanih izlazaka iz programa PowerPoint ključni je signal koji jamči da PowerPoint funkcionira prema očekivanjima.

Prikupljaju se sljedeća polja:

  - **Flag** – zastavice sesije

  - **Usage** – upotreba značajki

#### <a name="officepowerpointuaedialog"></a>Office.PowerPoint.UAE.Dialog

Prikuplja se svaki put kada se PowerPoint neočekivano zatvori dok je iznad njegovog glavnog prozora otvoren dijaloški okvir. Taj je podatak ključan za bilježenje slučajeva neočekivanog zatvaranja programa PowerPoint zbog toga što aktivan dijaloški okvir blokira njegov glavni prozor. Microsoft koristi te podatke za dijagnosticiranje problema da bi jamčio da PowerPoint funkcionira prema očekivanjima.

Prikupljaju se sljedeća polja:

  - **DlgCnt** – ukupan broj otvorenih dijaloških okvira u trenutku rušenja sesije

  - **DlgId** – identifikator otvorenog dijaloškog okvira

  - **IdType** – vrsta identifikatora otvorenog dijaloškog okvira

  - **InitTime** – vrijeme inicijalizacije sesije koja se srušila

  - **SessionId** – identifikator sesije koja se srušila

  - **TopId** – identifikator dijaloškog okvira na vrhu

  - **Version** – verzija sesije koja se srušila

#### <a name="officepowerpointuaedocument"></a>Office.PowerPoint.UAE.Document

Prikuplja podatke o značajci koja se koristila na dokumentu u trenutku neočekivanog zatvaranja programa PowerPoint. U te se značajke ubrajaju dijaprojekcija, otvaranje dokumenta, spremanje, uređivanje, suautorstvo i isključivanje. Te su informacije ključne za bilježenje slučajeva neočekivanog zatvaranja programa PowerPoint tijekom korištenja neke značajke. Microsoft koristi te podatke za dijagnosticiranje problema da bi jamčio da PowerPoint funkcionira prema očekivanjima.

Prikupljaju se sljedeća polja:

  - **CoauthFlag** – zastavice korištenja suautorstva

  - **CommandFlag** – zastavice izmjene dokumenta

  - **FileIOFlag** – zastavice korištenja ulazno-izlaznih operacija s datotekom

  - **InitTime** – vrijeme inicijalizacije sesije koja se srušila

  - **Location** – lokacija dokumenta

  - **ServerDocId** – identifikator poslužiteljskog dokumenta

  - **SessionId** – identifikator sesije koja se srušila

  - **UrlHash** – raspršivanje URL-a dokumenta

  - **Usage** – upotreba značajki

  - **Version** – verzija sesije koja se srušila

#### <a name="officepowerpointuaeopen"></a>Office.PowerPoint.UAE.Open

Prikuplja se svaki puta kada se PowerPoint neočekivano zatvori prilikom otvaranja dokumenta. Te su informacije ključne za bilježenje slučajeva neočekivanog zatvaranja programa PowerPoint tijekom otvaranja dokumenta. Microsoft koristi te podatke za dijagnosticiranje problema da bi jamčio da PowerPoint funkcionira prema očekivanjima.

Prikupljaju se sljedeća polja:

  - **FileUrlLocation** – lokacija URL-a dokumenta

  - **Flag** – zastavice otvaranja

  - **InitTime** – vrijeme inicijalizacije sesije koja se srušila

  - **Location** – lokacija dokumenta

  - **OpenReason** – razlog otvaranja

  - **ServerDocId** – identifikator poslužiteljskog dokumenta

  - **SessionId** – identifikator sesije koja se srušila

  - **UrlHash** – raspršivanje URL-a dokumenta

  - **Version** – verzija sesije koja se srušila

#### <a name="officepowerpointuaesession"></a>Office.PowerPoint.UAE.Session

Prikuplja podatke o značajci koja se koristila u trenutku neočekivanog zatvaranja sesije programa PowerPoint.  Te su informacije ključne za bilježenje slučajeva neočekivanog zatvaranja programa PowerPoint. Microsoft koristi te podatke za dijagnosticiranje problema da bi jamčio da PowerPoint funkcionira prema očekivanjima.

Prikupljaju se sljedeća polja:

  - **Flag** – zastavice sesije

  - **InitTime** – vrijeme inicijalizacije sesije koja se srušila

  - **PreviousSessionId** – identifikator sesije koja se srušila

  - **Usage** – upotreba značajki

  - **Version** – verzija sesije koja se srušila

#### <a name="officepowerpointuaeshutdown"></a>Office.PowerPoint.UAE.Shutdown

Prikuplja podatke o neočekivanom zatvaranju programa PowerPoint tijekom njegovog isključivanja. Te su informacije ključne za bilježenje slučajeva neočekivanog zatvaranja programa PowerPoint tijekom njegovog isključivanja. Microsoft koristi te podatke za dijagnosticiranje problema da bi jamčio da PowerPoint funkcionira prema očekivanjima.

Prikupljaju se sljedeća polja:

  - **InitTime** – vrijeme inicijalizacije sesije koja se srušila

  - **SessionId** – identifikator sesije koja se srušila

  - **Stage** – faza isključivanja

  - **Version** – verzija sesije koja se srušila

#### <a name="officepowerpointuaeslideshow"></a>Office.PowerPoint.UAE.SlideShow

Prikuplja podatke o neočekivanom zatvaranju programa PowerPoint tijekom njegovog isključivanja. Te su informacije ključne za bilježenje slučajeva neočekivanog zatvaranja programa PowerPoint tijekom njegovog isključivanja. Microsoft koristi te podatke za dijagnosticiranje problema da bi jamčio da PowerPoint funkcionira prema očekivanjima.

Prikupljaju se sljedeća polja:

  - **InitTime** – vrijeme inicijalizacije sesije koja se srušila

  - **Mode** – dijaprojekcijski način rada

  - **SessionId** – identifikator sesije koja se srušila

  - **State** – stanje dijaprojekcije

  - **Version** – verzija sesije koja se srušila


#### <a name="officeprogrammabilityaddinscomaddincrash"></a>Office.Programmability.Addins.COMAddInCrash 

Događaj koji se stvara prilikom rušenja COM dodatka. Koristi se za utvrđivanje problema s usvajanjem i pouzdanošću dodataka za Office. 

Prikupljaju se sljedeća polja:

- **AddinConnectFlag** – predstavlja ponašanje učitavanja  

- **AddinDescriptionV2** – opis dodatka 

- **AddinFileNameV2** – naziv stvarnog DLL dodatka. Ne obuhvaća mjesto datoteke.

- **AddinFriendlyNameV2** – neslužbeni naziv dodatka

- **AddinIdV2** – ID klase dodatka (CLSID)

- **AddinProgIdV2** – programski ID dodatka 

- **AddinProviderV2** – davatelj usluge dodatka 

- **AddinTimeDateStampV2** – vremenska oznaka alata za kompiliranje

- **AddinVersionV2** – verzija dodatka 

- **Interface** – COM sučelje programskog dodatka koje je dovelo do pada 

- **LoadAttempts** – koliko je pokušaja učitavanja napravljeno prije pada 

- **Način** – COM metoda dodatka koja je dovela do prekida rada 


#### <a name="officeprogrammabilitytelemetryaddincrash"></a>Office.Programmability.Telemetry.AddInCrash

Događaj koji se stvara prilikom učitavanja COM dodatka. Taj je podatak ključan da bi se utvrdilo je li neki dodatak uzrokovao rušenje aplikacije sustava Office. Koristi se za procjenu globalne kompatibilnosti dodataka s aplikacijama sustava Office.

Prikupljaju se sljedeća polja:

  - **CLSID** – identifikator klase dodatka

  - **ConnectFlag** – ponašanje pri učitavanju trenutnog dodatka

  - **FileName** – naziv datoteke dodatka, bez puta datoteke

  - **FriendlyName** – neslužbeni naziv dodatka

  - **Interface** – sučelje sustava Office u kojem je došlo do iznimke

  - **LoadAttempts** – broj pokušaja učitavanja dodatka

  - **Method** – metoda sustava Office u kojoj je došlo do iznimke

  - **OfficeApplication** – aplikacija sustava Office u kojoj je došlo do iznimke

  - **OfficeVersion** – verzije sustava Office

  - **ProgId** – programski identifikator dodatka

#### <a name="officeprogrammabilitytelemetrymacrofileopened"></a>Office.Programmability.Telemetry.MacroFileOpened 

Aktivira se tijekom otvaranja datoteke koja sadrži makronaredbu (VBA) na uređaju koji je IT administrator uveo u aplikacije sustava Office kao uslugu (OAAS) i kada je aktivirano okruženje Microsoft 365 Apps za velike tvrtke s licencom za velike tvrtke. Događaj se koristi za shvaćanje zdravlja datoteka koje sadrže makronaredbu (VBA) na klijentu i uspoređuje se s Office.Programmability.Telemetry.VbaTelemetryBreak koji prati pogreške na datotekama koje sadrže VBA-e. 

Ne prikupljaju se nikakva polja.

#### <a name="officesystemsystemhealthungracefulappexitmacandios"></a>Office.System.SystemHealthUngracefulAppExitMacAndiOS

Događaj tijekom pokretanja koji bilježi neskladne izlaze aplikacija za daljnje istraživanje.

Prikupljaju se sljedeća polja:

- **AffectedProcessAppBuild** – broj međuverzije

- **AffectedProcessAppBuildRevision** – broj revizije međuverzije

- **AffectedProcessAppMajorVer** – glavni broj verzije aplikacije

- **AffectedProcessAppMinorVer** – sporedni broj verzije aplikacije

- **AffectedProcessAppName** – naziv aplikacije

- **AffectedProcessResidentMemoryOnCrash** – ugrađena memorija srušene aplikacije

- **AffectedProcessUnsymbolicatedChecksum** – ide u kombinaciji s raspršivanjem Stack za simbolizaciju

- **AffectedProcessVirtualMemoryOnCrash** – virtualna memorija srušene aplikacije

- **AffectedSessionDuration** – trajanje sesije u sekundama prije rušenja

- **AffectedSessionLongBuildNumber** – dugačak broj međuverzije

- **CrashedProcessSessionID** – ID sesije procesa tijekom rušenja aplikacije

- **DetectionTime** – datum i vrijeme rušenja aplikacije
    
- **DeviceModel** – model hardvera

- **MERPSessionID** – ID sesije MERP-a

- **ReportingOsLocaleTag** – regionalne postavke operacijskog sustava

- **ReportingOSVerStr** – verzija operacijskog sustava

- **SessionBuildNumber** – verzija srušene aplikacije

- **SessionIDSMatch** – Booleova vrijednost za provjeravanje je li ID sesije koji izvješćuje isti koji je zabilježio Merp

- **SessionVersion** – verzija srušene aplikacije – **StackHash** – raspršivanje snopa praćenja srušene aplikacije

- **UAEType** – identifikator koji nam pruža informacije o vrsti rušenja o kojoj je bila riječ

#### <a name="officethisaddinstartupfailed"></a>Office.ThisAddIn.StartupFailed

Prikuplja informacije o iznimci koja se pojavljuje prilikom pokretanja aplikacije Data Streamer. Ti se podaci koriste za praćenje stanja aplikacije. Taj događaj generira dodatak Microsoft Data Streamer za Excel.

Prikupljaju se sljedeća polja:

- **Iznimka** – poziv stogu zbog iznimke

- **Naziv događaja** – naziv događaja je kategorija i oznaka događaja.

#### <a name="onenotesafebootresetcrashcounteronappsuspend-officeonenoteandroidsafebootresetcrashcounteronappsuspend-officeandroidearlytelemetrysafebootresetcrashcounteronappsuspend"></a>OneNote.SafeBootResetCrashCounterOnAppSuspend, Office.OneNote.Android.SafeBootResetCrashCounterOnAppSuspend, Office.Android.EarlyTelemetry.SafeBootResetCrashCounterOnAppSuspend

Kritični signal šalje se kada ponovno postavimo brojač rušenja na suspenziju aplikacije prije nego što se prikaže dijaloški okvir za sigurno pokretanje. Ta je oznaka obavezna za praćenje i dijagnozu stanja aplikacije. Dijaloški okvir za sigurno pokretanje prikazuje se nakon kontinuiranog višestrukog rušenja aplikacije. On korisniku omogućuje ponovno postavljanje aplikacije. Ta će oznaka pomoći ustanoviti da li se dijaloški okvir za sigurno pokretanje nije prikazao korisniku usprkos udovoljavanju kriterijima za njegovo aktiviranje. 

Prikupljaju se sljedeća polja:

- Nijedno


#### <a name="telemetryerror"></a>telemetry.error

Ovaj nam događaj omogućuje dijagnosticiranje i rješavanje problema koji sprječavaju generiranje ili slanje potrebnih dijagnostičkih podataka. Ovi nam događaji pomažu shvatiti jesu li nam promaknuli ključni podaci potrebno za identifikaciju sigurnosnih problema ili velikih problema u vezi s načinom rada vaše aplikacije.

Prikupljaju se sljedeća polja: 

- **timer_name** – govori nam gdje se problem s telemetrijom događa, primjerice u komponenti poštanskog sandučića ili kalendara. Ovo nam pomaže prepoznati i riješiti probleme s telemetrijom koji se događaju u određenom dijelu aplikacije

- **type** – govori nam vrstu pogreške timera kako bi nam pomogao prepoznati kada naša aplikacija ima bilo kakve probleme sa slanjem dijagnostičkih telemetrijskih podataka


#### <a name="watchdoganr"></a>watchdog.anr

Potrebno za nadzor pogrešaka u funkciji aplikacije za sprječavanje slučajeva kada aplikacija prestane reagirati, a vaš se ekran zamrzne u aplikaciji (naziva se ANR – aplikacija ne reagira).

Prikupljaju se sljedeća polja: 

- **callstack** – poziv stoga koda gdje je ANR nastupio
 
- **caused_restart** – je li aplikacija bila prisiljena ponovno se pokrenuti zbog ANR-a
 
- **duration** – vrijeme tijekom kojeg je uređaj bio zamrznut
 
- **id** – jedinstveni identifikator za ANR
 
- **interval** – konfigurirani prag za aktivaciju ANR-a
 
- **is_application_object_initialized** – je li se ANR dogodio nakon što je aplikacija bila potpuno pokrenuta ili prije
 
- **last_known_is_in_foreground** – je li aplikacija nedavno bila u prvom planu ili pozadini


### <a name="application-feature-performance-subtype"></a>*Podvrsta performansi značajki aplikacije*

Loše vrijeme odziva ili performanse za scenarije poput pokretanja aplikacije ili otvaranja datoteke.

#### <a name="androidframemetrics"></a>android.frame.metrics

Omogućuje nam prepoznavanje i rješavanje situacija u kojima naše komponente aplikacije Android uzrokuju probleme s funkcijom, primjerice ako ne možete bez poteškoća listati ulaznom poštom.

Prikupljaju se sljedeća polja: 

- **animation_duration** – trajanje prikaza animacije u milisekundama

- **command_issue_duration** – trajanje problema s naredbama na platformi u milisekundama 

- **draw_duration** – trajanje crtanja korisničkog sučelja u milisekundama 

- **input_handling_duration** – trajanje upravljanja unosom u milisekundama 

- **layout_measure_duration** – trajanje mjerenja rasporeda u milisekundama

- **origin** – komponenta aplikacije koja se mjeri, primjerice kalendar ili pošta

- **sync_duration** – trajanje sinkronizacije okvira u milisekundama

- **swap_buffers_duration** – trajanje zamjene međuspremnika u milisekundama

- **total_duration** – ukupno trajanje prikaza okvira u milisekundama

- **unknown_delay** – kašnjenje uzrokovano nepoznatim izvorima koji nisu izričito praćena trajanja

#### <a name="calcomponent"></a>cal.component

Ovaj nam događaj omogućuje prepoznavanje i rješavanje problema u okviru kojih postoji primjetan utjecaj na funkciju naših komponenti korisničkog sučelja kalendara zbog kojih biste imali probleme s pomicanjem kalendara.

Prikupljaju se sljedeća polja: 

- **above_40fps** – broj prikazanih okvira iznad 40 fps

- **above_40rate** – stopa prikazanih okvira iznad 40 fps

- **above_50fps** – broj prikazanih okvira iznad 50 fps

- **above_50rate** – stopa prikazanih okvira iznad 50 fps

- **above_55fps** – broj prikazanih okvira iznad 55 fps

- **above_55rate** – stopa prikazanih okvira iznad 55 fps

- **account_counter** – prati broj računa povezanih za svaku vrstu kalendara, na primjer, 2 za kalendar sustava Gmail te koristi li taj račun naš novi servis sinkronizacije

- **app_instance** – Outlook ima dvije ulazne točke za Duo; jedna je za aplikaciju Kalendar, a druga za aplikaciju Pošta i obje se mogu pokrenuti usporedno u okruženju s više instanci. Tako doznajemo koja instanca provodi ovo izvješćivanje, Pošta ili Kalendar.

- **component_name** – govori nam naziv komponente kalendara kao što je Prikaz rasporeda ili Prikaz dana kako bi nam pomogao prepoznati probleme s funkcijom koji utječu na određenu komponentu u kalendaru

- **display_frame_data** – prati vrijeme utrošeno na prikaz svakih 60 okvira za utvrđivanje postoje li problemi s funkcijom. 

- **orientation** – govori nam je li uređaj bio u okomitom ili vodoravnom načinu kako bi nam pomogao prepoznati probleme s funkcijom koji utječu na određenu orijentaciju uređaja

- **taskId** – TaskId će nam dati taskId (ID zadatka) trenutačne instance. To će biti potrebno u okruženju s više instanci ako korisnik želi usporedno pokrenuti iste instance (Kalendar, Kalendar ili Pošta, Pošta)

- **view_duration** – govori nam koliko je trajao prikaz raznih komponenti korisničkog sučelja kalendara kako bi nam pomogao prepoznati probleme s funkcijom koji utječu na vaše iskustvo kalendara

#### <a name="contactaction"></a>contact.action

Taj se događaj pokreće u različitim radnjama u kontaktima – pregled, ažuriranje i brisanje kontakata, kao i pregled popisa kontakata. Koristi se za određivanje postoje li regresije izvedbe koje imaju veze sa kontaktima.

Prikupljaju se sljedeća polja: 

- **accounts_with_filters** – broj računa s filtrima primijenjenim na popis kontakata

- **action** – radnja koja je izvedena, npr. prikazivanje kontakta
 
- **duration_initial_view_load** – trajanje od otvaranja prikaza do početnog učitavanja popisa kontakata

- **duration_show_contacts** – trajanje od otvaranja prikaza do prikazivanja kontakata na popisu kontakata
 
- **total_contacts** – broj kontakata bez primijenjenih filtara
 
- **total_filtered_contacts** – broj kontakata s primijenjenim filtrima

#### <a name="conversationloadtime"></a>conversation.load.time

Ovaj nam događaj omogućuje otkrivanje i rješavanje problema u okviru kojih postoji zamjetan utjecaj na funkciju učitavanja vaših razgovora e-pošte kako bismo osigurali da se vaše poruke e-pošte učitavaju na očekivan način.

Prikupljaju se sljedeća polja: 

- **time** – govori nam količinu vremena koja je bila potrebna za dovršavanje učitavanja razgovora e-pošte.

#### <a name="conversationreloaded"></a>conversation.reloaded

Taj nam događaj omogućuje prepoznavanje učestalosti ponovnog umetanja razgovora na temelju obavijesti o servisiranju. Moramo pratiti jesu li obavijesti o ažuriranju preglasne i treba li ih obrezati jer pogoršavaju upotrebljivost.

Prikupljaju se sljedeća polja: 

- **average** – količina ponovnog učitavanja podijeljena s veličinom 

- **client-request-id** – identifikator zahtjeva klijenta za zahtjev koji je uzrokovao pogrešku

- **date** – datumska oznaka zahtjeva koji je uzrokovao pogrešku

- **duration** – vrijeme kada je razgovor bio otvoren 


#### <a name="coredatamigration"></a>core.data.migration

Omogućuje nam otkrivanje i rješavanje situacija u okviru kojih je došlo do pogreške pri ažuriranja podataka e-pošte na vašem uređaju na noviju verziju.

Prikupljaju se sljedeća polja:

- **db_size_megabytes** – prati veličinu baze podataka osnovnih podataka zaokruženu na najbližih 25 megabajta i s najvećom veličinom od 500 megabajta

- **db_wal_size_megabytes** – prati veličinu baze podataka osnovnih podataka kada je netaknuta glavna datoteka za spremanje zaokružena na najbliži 1 megabajt i s najvećom veličinom od 10 megabajta

- **free_space_megabytes** – prati slobodan prostor dostupan u grupama od 10, 100, 1000, 10 000 i zatim 100 000. 

- **migration_duration_seconds** – prati trajanje migracije zaokruženo na jedan od ovih termina – 0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 110, 120, 130, 140, 150, 160, 170, 180 (180 i više trebalo bi biti samo 180)

#### <a name="coredataperformance"></a>core.data.performance

Omogućuje nam otkrivanje i rješavanje situacija kada podaci e-pošte koje spremamo na vaš uređaj uzrokuju probleme s funkcijom.

Prikupljaju se sljedeća polja:

- **Caller** – prati naziv entiteta koji poziva radnju spremanja

- **db_size_megabytes** – prati veličinu baze podataka osnovnih podataka zaokruženu na najbližih 25 megabajta i s najvećom veličinom od 500 megabajta

- **duration** – prati veličinu vremena koja je potrebna za dovršavanje postupka

- **entity** – prati naziv entiteta koji je pozvao radnju dohvaćanja

- **operation** – neobrađena vrijednost radnje, bilo spremanje, dohvaćanje ili „read write queue blocked”

#### <a name="inboxcomponent"></a>inbox.component

Ovaj događaj prikuplja dvije vrste korisničkih podataka: status pretplate na Microsoft 365 i vidi li korisnik oglase. To nam omogućuje otkrivanje i rješavanje problema u okviru kojih postoji zamjetan utjecaj na funkciju komponenti korisničkog sučelja ulazne pošte korisnika koji bi doveli do neispravnog učitavanja ili prikaza poruka e-pošte, avatara ili stanja pročitano/nepročitano.

Prikupljaju se sljedeća polja: 

- **above_40fps** – broj prikazanih okvira iznad 40 fps

- **above_40rate** – stopa prikazanih okvira iznad 40 fps

- **above_50fps** – broj prikazanih okvira iznad 50 fps

- **above_50rate** – stopa prikazanih okvira iznad 50 fps

- **above_55fps** – broj prikazanih okvira iznad 55 fps

- **above_55rate** – stopa prikazanih okvira iznad 55 fps

- **account_counter** – količina svake vrste računa koji postoji na uređaju, primjerice račun sustava Office 365 = 1 račun, račun Outlook.com = 1 račun.

- **ad_not_shown_reason** – razlog zašto se oglasi ne prikazuju

- **ad_shown** – je li se određeni oglas prikazao (ako su oglasi omogućeni)

- **ad_shown_for_premium** – neočekivan prikaz oglasa premium korisnicima

- **age** – dob osobe (koristi se za potvrdu sukladnosti s dobnim ograničenjima za oglase) *[Ovo je polje uklonjeno iz trenutačnih međuverzija programa Office, ali može se i dalje prikazivati u drugim međuverzijama.]*

- **app_instance** – Outlook ima dvije ulazne točke za Duo; jedna je za aplikaciju Kalendar, a druga za aplikaciju Pošta i obje se mogu pokrenuti usporedno u okruženju s više instanci. Tako doznajemo koja instanca provodi ovo izvješćivanje, Pošta ili Kalendar.

- **component_name** – naziv komponente/prikaza koji je aktivan tijekom filtriranja

- **has_hx** – ima li uređaj najmanje jedan račun Hx (naš novi servis za sinkronizaciju poruka e-pošte)

- **has_subscription** – ima li uređaj pretplatu na oglase

- **is_all_accounts_inbox** – nalazi li se trenutna ulazna pošta u mapi „svi računi”

- **is_current_account** – je li trenutno aktivni račun ujedno račun za oglase

- **load_error_code** – kod pogreške tijekom učitavanja oglasa

- **network_error_code** – kod mrežne pogreške tijekom zahtijevanja oglasa

- **orientation** – orijentacija ekrana u trenutku događaja (okomito ili vodoravno)

- **provider** – davatelj usluge (Xandr ili Facebook) oglasa koji se trenutačno prikazuje

- **sub_error_type** – detaljna vrsta pogreške

- **taskId** – TaskId će nam dati taskId (ID zadatka) trenutačne instance. To će biti potrebno u okruženju s više instanci ako korisnik želi usporedno pokrenuti iste instance (Kalendar, Kalendar ili Pošta, Pošta)

- **total_count** – ukupan broj okvira koji komponenta prikazuje

- **view_duration** – koliko je dugo korisnik pregledavao komponentu

#### <a name="initialpagelanding"></a>Initial.page.landing 
 
Ovaj događaj pomaže u praćenju vrste iskustva koje korisnici vide kada otvore našu stranicu aplikacije.  Ti se podaci koriste za određivanje prometa korisnika koji se navode u svakom iskustvu u našoj aplikaciji i pomažu nam da lako konsolidiramo rezultate eksperimentiranja.
 
Prikupljaju se sljedeća polja: 

- **Page** – koristi se za praćenje iskustva koje korisnik prvi put vidi kada otvori našu stranicu. Moguće su vrijednosti „Probna verzija”, „Preskoči”, „Prepakirano”, „Pretplata” itd.

- **storeExperience** – koristi se za utvrđivanje je li korisnik ispunjavao uvjete da vidi sučelje SDK trgovine.

- **stringVariant** – koristi se za određivanje vrste nizova koje korisnik vidi kada otvori našu stranicu. Imajte na umu da na bilo kojoj stranici, kao što je primjerice „Probna verzija” korisnik može ispunjavati uvjete za prikaz različitih nizova ovisno o tome ima li instaliranu stariju verziju sustava Office ili ako je prethodno aktivirao Office. Moguće enumeracije tog svojstva su: „LegacyUpsell”, „OfficeOpened”, „Default”, „YesIntent”, „NoIntent” itd.

- **windowsBuildType** – koristi se za praćenje vrste međuverzije sustava Windows (WindowsBuildType) na kojem je korisnik. odnosno „RS4”, „RS5”, „RS19H1”, „Vibranium” itd. Kako naša iskustva obično ciljaju na različite WindowsBuildTypes, ovo svojstvo je od vitalne važnosti za razlikovanje implementacija. 

#### <a name="ipcpbootstrapuser"></a>IpcpBootstrapUser

Prikuplja se kada korisnik pokuša otvoriti dokument zaštićen IRM-om ili primijeniti zaštite IRM-a. Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada se stvori IpcpBootstrapUser poziv API-ja.

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere

- **AppInfo.Name** – naziv aplikacije.

- **AppInfo.Version** – verzija aplikacije

- **iKey** – identifikacijski broj poslužitelja pružatelja usluge zapisivanja

- **RMS.ApplicationScenarioId** – identifikacijski broj scenarija koji pruža aplikacija

- **RMS.AuthCallbackProvided** – označava pruža li se povratni poziv za provjeru autentičnosti kao unos poziva API-ja ili ne

- **RMS.ConnectionInfo.ExtranetUrl** – URL ekstraneta u informacijama o vezi

- **RMS.ConnectionInfo.IntranetUrl** – URL intraneta u informacijama o vezi

- **RMS.ConnectionMode** – način povezivanja između klijenta usluge upravljanja pravima i poslužitelja: na mreži ili izvan mreže

- **RMS.Duration** – ukupno vrijeme potrebno za dovršavanje poziva API-ja

- **RMS.DurationWithoutExternalOps** – ukupno vrijeme umanjeno za potrošene vanjske operacije poput latencije mreže.

- **RMS.ErrorCode** – kod pogreške koji, ako postoji, vraća poziv API-ja

- **RMS.GuestTenant** – identifikacijski broj klijenta gosta za korisnika

- **RMS.HomeTenant** – identifikacijski broj početnog klijenta za korisnika

- **RMS.HttpCall** – označava postoji li operacija HTTP-a

- **RMS.Identity.ExtranetUrl** – URL ekstraneta poslužitelja usluge upravljanja pravima za korisnika koji se prikuplja tijekom dobivanja novog certifikata za račun prava s poslužitelja

- **RMS.Identity.IntranetUrl** – URL intraneta poslužitelja usluge upravljanja pravima za korisnika koji se prikuplja tijekom dobivanja novog certifikata za račun prava s poslužitelja

- **RMS.Identity.Status** – prvi put dobivanja certifikata za račun prava s poslužitelja ili obnavljanja certifikata za račun prava 

- **RMS.Identity.Type** – vrsta korisničkog računa kao što je račun za Windows ili račun za Live

- **RMS.Identity.UserProvided** – označava je li adresa e-pošte korisnika pružena ili nije tijekom dobivanja novog certifikata za račun prava s poslužitelja

- **RMS.IssuerId** – identifikacijski broj poslužitelja usluge upravljanja pravima koji izdaje certifikat za račun prava  

- **RMS.LicenseFormat** – format licence: Xrml ili Json

- **RMS.RACType** – vrsta certifikata za račun prava

- **RMS.Result** – uspjeh ili neuspjeh poziva API-ja

- **RMS.ScenarioId** – identifikacijski broj scenarija definiran API-jem

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

- **RMS.ServerType** – vrsta poslužitelja usluge upravljanja pravima 

- **RMS.StatusCode** – kod statusa vraćenog rezultata

- **RMS.TemplatesCount** – broj predložaka

- **RMS.TokenProvided** – označava je li token pružen kao unos poziva API-ja ili ne 

- **RMS.UserProvided** – označava je li korisnik pružen kao unos poziva API-ja ili ne 

- **UserInfo.UserObjectId** – identifikacijski broj objekta korisnika

#### <a name="ipcpgetkey"></a>IpcpGetKey

Prikuplja se kada korisnik pokuša otvoriti dokument zaštićen značajkom upravljanja pravima na informacije (IRM) ili primijeniti zaštite IRM-a. Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada se stvori IpcpGetKey poziv API-ja.

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere

- **AppInfo.Name** – naziv aplikacije.

- **AppInfo.Version** – verzija aplikacije

- **iKey** – identifikacijski broj poslužitelja pružatelja usluge zapisivanja

- **RMS.ApplicationScenarioId** – identifikacijski broj scenarija koji pruža aplikacija

- **RMS.AuthCallbackProvided** – označava pruža li se povratni poziv za provjeru autentičnosti kao unos poziva API-ja ili ne

- **RMS.ConnectionMode** – način povezivanja između klijenta usluge upravljanja pravima i poslužitelja: na mreži ili izvan mreže

- **RMS.ContentId** – identifikacijski broj sadržaja dokumenta

- **RMS.Duration** – ukupno vrijeme potrebno za dovršavanje poziva API-ja

- **RMS.DurationWithoutExternalOps** – ukupno vrijeme umanjeno za potrošene vanjske operacije poput latencije mreže.

- **RMS.ErrorCode** – kod pogreške koji, ako postoji, vraća poziv API-ja

- **RMS.EulId** – ID licence krajnjeg korisnika

- **RMS.EulProvided** – označava je li licenca krajnjeg korisnika pružena kao unos poziva API-ja ili ne

- **RMS.GuestTenant** – identifikacijski broj klijenta gosta za korisnika 

- **RMS.HomeTenant** – identifikacijski broj početnog klijenta za korisnika

- **RMS.HttpCall** – označava postoji li operacija HTTP-a

- **RMS.Identity.ExtranetUrl** – URL ekstraneta poslužitelja usluge upravljanja pravima za korisnika koji se prikuplja tijekom dobivanja novog certifikata za račun prava s poslužitelja

- **RMS.Identity.IntranetUrl** – URL intraneta poslužitelja usluge upravljanja pravima za korisnika koji se prikuplja tijekom dobivanja novog certifikata za račun prava s poslužitelja

- **RMS.Identity.Status** – prvi put dobivanja certifikata za račun prava s poslužitelja ili obnavljanja certifikata za račun prava 

- **RMS.Identity.Type** – vrsta korisničkog računa kao što je račun za Windows ili račun za Live

- **RMS.Identity.UserProvided** – označava je li adresa e-pošte korisnika pružena ili nije tijekom dobivanja novog certifikata za račun prava s poslužitelja

- **RMS.IssuerId** – identifikacijski broj poslužitelja usluge upravljanja pravima koji izdaje certifikat za račun prava 

- **RMS.KeyHandle** – adresa memorije ručice ključa

- **RMS.LicenseFormat** – format licence: Xrml ili Json

- **RMS.PL.ExtranetUrl** – URL ekstraneta u licenci za izdavanje

- **RMS.PL.IntranetUrl** – URL intraneta u licenci za izdavanje

- **RMS.PL.KeyType** – vrijednosti „jedno” ili „dvostruko” označavaju je li PL bio zaštićen zaštitom s jednim ključem ili zaštitom s dvostrukim ključevima

- **RMS.RACType** – vrsta certifikata za račun prava

- **RMS.Result** – uspjeh ili neuspjeh poziva API-ja

- **RMS.ScenarioId** – identifikacijski broj scenarija definiran API-jem

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

- **RMS.ServerType** – vrsta poslužitelja usluge upravljanja pravima

- **RMS.StatusCode** – kod statusa vraćenog rezultata

- **RMS.TemplatesCount** – broj predložaka

- **RMS.TokenProvided** – označava je li token pružen kao unos poziva API-ja ili ne 

- **RMS.UserProvided** – označava je li korisnik pružen kao unos poziva API-ja ili ne 

- **UserInfo.UserObjectId** – identifikacijski broj objekta korisnika

#### <a name="jsonparseerror"></a>json.parse.error 
 
Ovaj događaj označava da pogrešku javlja raščlanitelj JSON-a.  Morat ćemo ispraviti pogrešku očitanog niza registra koja je poslana na JSON raščlanitelj kako bismo korisnicima omogućili nesmetano iskustvo.
 
Prikupljaju se sljedeća polja: 

- **Error** – sastoji se od poruke o pogrešci koju objekt pogreške vraća.

#### <a name="mailfiltercomponent"></a>mail.filter.component

Ovaj nam događaj omogućuje prepoznavanje i rješavanje problema u okviru kojih postoji zamjetan utjecaj na funkciju vašeg doživljaja filtriranja poruka e-pošte koji bi doveli do neispravnog učitavanja ili prikaza vaših filtara.

Prikupljaju se sljedeća polja: 

- **above_40fps** – broj prikazanih okvira iznad 40 fps

- **above_40rate** – stopa prikazanih okvira iznad 40 fps
 
- **above_50fps** – broj prikazanih okvira iznad 50 fps

- **above_50rate** – stopa prikazanih okvira iznad 50 fps
 
- **above_55fps** – broj prikazanih okvira iznad 55 fps

- **above_55rate** – stopa prikazanih okvira iznad 55 fps
 
- **account_counter** – količina svake vrste računa koji postoji na uređaju, primjerice račun sustava Office 365 = 1 račun, račun Outlook.com = 1 račun.
 
- **ad_not_shown_reason** – razlog zašto se oglasi ne prikazuju
 
- **ad_shown** – prikazuje li se određeni oglas (ako su oglasi omogućeni)
 
- **age** – dob osobe (koristi se za potvrdu usklađenosti s dobnim ograničenjima za oglase)

- **app_instance** – Outlook ima dvije ulazne točke za Duo; jedna je za aplikaciju Kalendar, a druga za aplikaciju Pošta i obje se mogu pokrenuti usporedno u okruženju s više instanci. Tako doznajemo koja instanca provodi ovo izvješćivanje, Pošta ili Kalendar.
 
- **component_name** – naziv komponente/prikaza koji je aktivan tijekom filtriranja
 
- **folder_type** – vrsta mape koja se filtrira (npr. Ulazna pošta, Smeće, Nije dio sustava)
 
- **has_hx** – ima li uređaj najmanje jedan račun Hx (novi servis za sinkronizaciju poruka e-pošte)
 
- **has_subscription** – ima li uređaj pretplatu na oglase
 
- **is_all_accounts_inbox** – nalazi li se trenutna ulazna pošta u mapi „svi računi”
 
- **is_current_account** – je li trenutno aktivni račun ujedno račun za oglase
 
- **load_error_code** – kod pogreške tijekom učitavanja oglasa
 
- **network_error_code** – kod mrežne pogreške tijekom zahtijevanja oglasa
 
- **orientation** – orijentacija ekrana u trenutku događaja (okomito ili vodoravno)
 
- **sub_error_type** – detaljna vrsta pogreške

- **taskId** – TaskId će nam dati taskId (ID zadatka) trenutačne instance. To će biti potrebno u okruženju s više instanci ako korisnik želi usporedno pokrenuti iste instance (Kalendar, Kalendar ili Pošta, Pošta)
 
- **total_count** – ukupan broj okvira koji komponenta prikazuje
 
- **view_duration** – koliko je dugo korisnik pregledavao komponentu

#### <a name="messagerenderingintercepted"></a>message.rendering.intercepted

Ovaj nam događaj omogućuje praćenje koliko često korisnici presreću postupak prikazivanja prije nego što je dovršen. Te podatke koristimo za otkrivanje problema s performansama.

Prikupljaju se sljedeća polja: 

- **is_cache** – bez obzira na to je li tijelo poruke učitano iz predmemorije

- **is_on_screen** – je li postupak prikazivanja vidljiv korisnicima (normalno prikazivanje)

- **is_rendering_complete** – bez obzira na to je li proces prikazivanja dovršen 

- **is_trimmed_body** – bez obzira na to je li tijelo poruke obrezano 

- **rendering_method** – način prikazivanja poruke

- **rendering_time** – trajanje prikazivanja poruke dok korisnik ne napusti stranicu

#### <a name="messagerenderingperformance"></a>message.rendering.performance

Taj nam događaj omogućuje praćenje performansi postupka prikazivanja poruka, tako da možemo analizirati performanse različitih procesa renderiranja i otkriti poteškoće s performansama. 

Prikupljaju se sljedeća polja: 

- **bundle_prepare_time** – vrijeme pripreme paketa za prikazivanja

- **full_rendering_time** – vrijeme potpunog postupka prikazivanja 

- **is_cache** – bez obzira na to je li tijelo poruke učitano iz predmemorije

- **is_on_screen** – je li postupak prikazivanja vidljiv korisnicima (normalno prikazivanje)

- **is_trimmed_body** – bez obzira na to je li tijelo poruke obrezano 

- **load_message_time** – vrijeme učitavanja poruke iz pozadine (može biti 0 ako je poruka predmemorirana)

- **native_preprocess_time** – vrijeme za predobradu tijela poruke u izvornoj strani 

- **prepare_body_time** – vrijeme pripreme tijela za poruke (uključujući poruku učitavanja i predobrade)

- **rendering_method** – način prikazivanja poruke

- **rendering_time** – vrijeme za prikazivanje poruke po paketu  

- **wait_time** – vrijeme za stvaranje URL-a poruke


#### <a name="officeandroidandroidofficelaunchtolandingpagelatency"></a>Office.Android.AndroidOfficeLaunchToLandingPageLatency

Ključno je za snimanje metrike performansi aplikacije s obzirom na vrijeme odaziva aplikacije prilikom pokretanja.  Microsoft to upotrebljava za prikupljanje vremena potrebnog za reagiranje aplikacije i otkrivanje scenarija koji mogu utjecati na vrijeme pokretanja u aplikacijama Word, Excel ili PowerPoint.

Prikupljaju se sljedeća polja:
 
- **AnyCrashInteractionDuringBoot** – Booleova vrijednost za svaki pad koji se dogodio tijekom pokretanja

- **AppActivationTimeInMs** – vrijeme faze aplikacije

- **AppSuspendedDuringBoot** – Booleova vrijednost za obustavljanje aplikacije tijekom pokretanja

- **AvailableMemoryInMB** – dostupna memorija

- **CollectionTime** – vrijeme događaja

- **DalvikHeapLimitInMB** – informacije o snopu

- **DocumentRecoveryInvoked** – Booleova vrijednost da naznači je li neki dokument oporavljen

- **ExtractionDone** – vrijeme izdvajanja izvorne biblioteke

- **FastBootGainTimeInMs** – vrijeme za brzo dovršavanje pokretanja

- **FileActivationAttempted** – Booleova vrijednost koja označava je li aplikacija pokrenuta zbog aktivacije datoteke

- **HasLogcatLoggingImpactOnBoot** – Booleova vrijednost koja označava je li logcat utjecao na vrijeme pokretanja

- **IsThisFirstLaunch** – Booleova vrijednost koja označava je li ovo prvo pokretanje aplikacije

- **LatencyTimeInMilliSec** – kašnjenje u milisekundama

- **LibrarySharingTimeInMs** – vrijeme za zajedničko korištenje biblioteka

- **LoadMinLibsTimeInMs** – vrijeme učitavanja za minimalni skup biblioteka

- **MruListingTimeInMs** – vrijeme za učitavanje servisa MRU

- **NativeLibrariesLoadTime** – vrijeme učitavanja CPP biblioteke

- **NumberOfRunningProcesses** – broj pokrenutih procesa

- **NumberOfRunningProcesses** – broj pokrenutih procesa

- **NumberOfRunningServices** – broj pokrenutih usluga

- **OfficeActivityTimeInMs** – vrijeme za pokretanje aktivnosti u sustavu Office

- **PostAppInitTimeInMs** – vrijeme faze aplikacije

- **PreAppInitializationTime** – vrijeme pokretanja faze aplikacije

- **PreAppInitTimeInMs** – vrijeme faze aplikacije

- **TotalMemoryInMB** – ukupna memorija

- **UIRaaSDownloadLanguagePackageBoot** – informacije koje se odnose na preuzimanje jezičnog paketa

- **UserDialogInterruptionDuringBoot** – Booleova vrijednost za bilo koji dijaloški okvir za blokiranje prikazan tijekom pokretanja


#### <a name="officeappleappleappbootmac"></a>Office.Apple.Apple.AppBoot.Mac

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za prikupljanje vremena potrebnog za pokretanje aplikacije, kao i nekih detalja o vrsti izvedenog pokretanja. Taj nam događaj pomaže da pratimo našu izvedbu i osiguramo poboljšanja performansi.

Prikupljaju se sljedeća polja:

- **Data_ Data_EvtBootTimerDocStageReady** – vrijeme proteklo do postizanja određene točke u kôdu.

- **Data_DocumentRecoveryInvoked** – je li oporavak dokumenta pozvan tijekom pokretanja.

- **Data_EvtBootTimerBootIdle** – vrijeme proteklo do postizanja određene točke u kôdu.

- **Data_EvtBootTimerFinishLaunchEnd** – vrijeme proteklo do postizanja određene točke u kôdu.

- **Data_EvtBootTimerLaunchDidFinish** – vrijeme proteklo do postizanja određene točke u kôdu.

- **Data_EvtBootTimerLaunchStart** – vrijeme proteklo do postizanja određene točke u kôdu.

- **Data_EvtBootTimerMainStart** – vrijeme proteklo do postizanja određene točke u kôdu.

- **Data_EvtBootTimerStaticInit** – vrijeme proteklo do postizanja određene točke u kôdu.

- **Data_EvtDockStageReady** – vrijeme proteklo do postizanja određene točke u kôdu.

- **Data_IsFileOpenAttempted** – je li pokušano otvaranje datoteke tijekom pokretanja.

- **Data_IsFirstRunAttempted** – je li pokretanje aplikacije prošlo kroz prvo iskustvo pokretanja.

- **Data_SentToBackground** – je li aplikacija poslana u pozadinu tijekom pokretanja.

#### <a name="officeapplediskruleresultserializererroronstreamop"></a>Office.Apple.DiskRuleResultSerializerErrorOnStreamOp

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za nadziranje stanja naše telemetrijske infrastrukture. Ovaj događaj označava da je došlo do pogreške.

Prikupljaju se sljedeća polja:

- **Data_ActualBytesModified** – broj izmijenjenih bajtova.

- **Data_BytesRequested** – broj bajtova koje želite obraditi.

- **Data_IsWriteOp** – bilo da se radi o izvršavanju operacije pisanja

#### <a name="officeapplemacbootresourceusage"></a>Office.Apple.MacBootResourceUsage

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za prikupljanje više pokazatelja oko resursa koji se potroše tijekom pokretanja aplikacija sustava Office. Taj nam događaj pomaže da pratimo našu izvedbu i osiguramo poboljšanja performansi.

Prikupljaju se sljedeća polja:

- **Data_BlockInputOperations** – broj blokiranih operacija ulaza

- **Data_BlockOutputOperations** – broj blokiranih operacija izlaza

- **Data_InvoluntaryContextSwitches** – broj nehotičnih kontekstnih sklopki

- **Data_MainThreadCPUTime** – mjera proteklog vremena

- **Data_MaxResidentSize** – mjera veličine memorije

- **Data_MessagesReceived** – broj primljenih poruka

- **Data_MessagesSent** – broj poslanih poruka

- **Data_PageFaults** – broj povrata stranica

- **Data_PageReclaims** – broj povrata stranica

- **Data_ProcessCPUTime** – mjera proteklog vremena

- **Data_SharedTextMemorySize** – mjera veličine memorije

- **Data_SignalsReceived** – broj primljenih signala

- **Data_Swaps** – broj zamjene podataka

- **Data_SystemCPUTime** – mjera proteklog vremena

- **Data_SystemUpTime** – mjera proteklog vremena

- **Data_UnsharedDataSize** – mjera veličine podataka

- **Data_UnsharedStackSize** – mjera veličine stoga

- **Data_UserCPUTime** – mjera proteklog vremena

- **Data_VoluntaryContextSwitchesNvcsw** – broj nehotičnih kontekstnih sklopki

#### <a name="officeapplemauvalidation"></a>Office.Apple.MAU.Validation

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za nadziranje stanja komponente Microsoftova automatskog ažuriranja koja se koristi za distribuciju i instaliranje ažuriranja aplikacija. Prikupljeni podaci koriste se za otkrivanje pogrešaka i istraživanje uzroka neuspjeha.

Prikupljaju se sljedeća polja:

- **Data_EventID** – prikupljamo niz koji predstavlja kôd pogreške.

- **Data_Message** – prikupljamo niz koji sadrži opis pogreške.

#### <a name="officeapplembuinstrumenthangdetectionspincontrol"></a>Office.Apple.MbuInstrument.Hang.Detection.Spin.Control

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se bilježi kad god se čini da neka aplikacija ne reagira. Taj nam događaj pomaže da pratimo našu izvedbu i osiguramo poboljšanja performansi.

Prikupljaju se sljedeća polja:

- **Data_CountSpinControlStart** – marker koji označava da je aplikacija prestala da reagira (ili da sporo reagira)

#### <a name="officeapplembuinstrumentvmondocumentclose"></a>Office.Apple.MbuInstrument.VMOnDocumentClose

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za prikupljanje snimka stanja memorije tijekom zatvaranja dokumenta. Taj nam događaj pomaže da pratimo našu izvedbu i osiguramo poboljšanja performansi.

Prikupljaju se sljedeća polja:

- **Data_CollectionTime** – vremenska oznaka od momenta kada su podaci prikupljeni

- **Data_ResidentMemory** – zapažena vrijednost ugrađene memorije

- **Data_VirtualMemory** – zapažena vrijednost virtualne memorije

#### <a name="officeapplembuinstrumentvmonshutdown"></a>Office.Apple.MbuInstrument.VMOnShutdown

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za prikupljanje snimka stanja memorije tijekom isključivanja aplikacije. Taj nam događaj pomaže da pratimo našu izvedbu i osiguramo poboljšanja performansi.

Prikupljaju se sljedeća polja:

- **Data_CollectionTime** – vremenska oznaka od momenta kada su podaci prikupljeni

- **Data_ResidentMemory** – zapažena vrijednost ugrađene memorije

- **Data_VirtualMemory** – zapažena vrijednost virtualne memorije

#### <a name="officeapplembuinstrumentvmonstart"></a>Office.Apple.MbuInstrument.VMOnStart

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za prikupljanje snimka stanja memorije tijekom pokretanja aplikacije. Taj nam događaj pomaže da pratimo našu izvedbu i osiguramo poboljšanja performansi.

Prikupljaju se sljedeća polja:

- **Data_CollectionTime** – vremenska oznaka od momenta kada su podaci prikupljeni

- **Data_ResidentMemory** – zapažena vrijednost ugrađene memorije

- **Data_VirtualMemory** – zapažena vrijednost virtualne memorije

#### <a name="officeapplemsoappdelegatebootperf"></a>Office.Apple.MsoAppDelegate.BootPerf

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za prikupljanje vremena i memorije utrošene tijekom pokretanja aplikacija sustava Office, kao i neke pojedinosti o vrsti pokretanja. Taj nam događaj pomaže da pratimo našu izvedbu i osiguramo poboljšanja performansi.

Prikupljaju se sljedeća polja:

- **Data_AppLaunchDurationMicroSec** – trajanje postupka pokretanja

- **Data_AppLaunchFinishSystemTime** – vremenska oznaka na određenom markeru kôda za pokretanje

- **Data_AppLaunchStartSystemTime** – vremenska oznaka na određenom markeru kôda za pokretanje

- **Data_ResidentMemory** – snimka raspoložive ugrađene memorije tijekom pokretanja

- **Data_VirtualMemory** – snimka raspoložive virtualne memorije tijekom pokretanja

#### <a name="officeappleungracefulappexithangsinprevioussession"></a>Office.Apple.UngracefulAppExitHangsInPreviousSession

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za nadziranje stanja aplikacija sustava Office kao i za ispitivanje uzroka pogrešaka. Prikupljamo podatak koliko je puta aplikacija djelovala kao da ne reagira prije no što je došlo do izlaza iz aplikacije s poteškoćama.

Prikupljaju se sljedeća polja:

- **Data_HangsDetected** – podatak koliko se puta činilo da aplikacija ne reagira prije no je uočen izlaz iz aplikacije s poteškoćama.

- **Data_LastSessionId** – identifikator sesije u kojoj je uočen izlaz iz aplikacije s poteškoćama.

- **Data_SessionBuildNumber** – sporedna verzija aplikacije u kojoj je uočen izlaz iz aplikacije s poteškoćama.

- **Data_SessionVersion** – glavna verzija aplikacije u kojoj je uočen izlaz iz aplikacije s poteškoćama.

#### <a name="officeapplewhatsnewerrorandwarning"></a>Office.Apple.WhatsNewErrorAndWarning

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za nadziranje stanja značajke Novosti. Ovaj događaj označava da je došlo do pogreške /upozorenja prilikom analize sadržaja Novosti, što ukazuje na potencijalne probleme stvaranja sadržaja.

Prikupljaju se sljedeća polja:

- **Data_ContentKey** – pokazivač na odjeljak sadržaja koji je vjerojatno uzrokovao pogrešku.

- **Data_ErrorCode** – uočeni kôd pogreške (ako je dostupno)

- **Data_ErrorDescription** – opis pogreške (ako je dostupno)

- **Data_EventID** – prikupljamo niz koji predstavlja vrstu uočene pogreške.

- **Data_IncludesHTMLTag** – bilo da sadržaj ima obogaćeni html

- **Data_IncludesItemsTag** – bilo da sadržaj ima hijerarhiju stavki

- **Data_LengthOfRawData** – veličina sadržaja

- **Data_RequestURL** – URL s kojeg je sadržaj preuzet

- **Data_ServerLanguageTag** – jezik na kojem je sadržaj.

- **Data_StatusCode** – status pogreške (ako je dostupno)

#### <a name="officeextensibilityrichapimethodinvocation"></a>Office.Extensibility.RichApiMethodInvocation

Kada korisnik koristi dodatak sustava Office i pozove Rich API za pružanje usluge, ovaj će se događaj pokrenuti. Koristi se za mjerenje pouzdanosti usluga, performansi i upotrebe pozivanja načina Rich API.
 
Prikupljaju se sljedeća polja:

- **Api** – puno ime API-ja

- **DispFlag** – zastavica bita koja opisuje vrstu poziva načina (primjer: 0x1 = METHOD, 0x2 = PROPERTYGET, 0x4 = PROPERTYPUT, 0x8 = PROPERTYPUTREF)

- **DispId** – ID isporuke za način koji se poziva

- **HResult** – HResult za poziv načina

- **Latency** – latencija za poziv, u mikrosekundama

- **ReqId** – GUID za skupni zahtjev kojem ovaj način pripada

- **TypeId** – GUID za sučelje na kojem se ovaj način poziva

#### <a name="officeiospaywallfailedscreenretrybuttontap"></a>Office.iOS.Paywall.FailedScreen.RetryButtonTap

Ova se telemetrija uporabe prikuplja kako bi se znalo kada Kupnja/Dodjela resursa/Aktivacija nije uspjela, a korisnik je dodirnuo gumb „Pokušaj ponovno".  Upotrebljava se za rješavanje scenarija pogreške prilikom kupnje koji vode do ponovnog pokušaja i poboljšanja pouzdanosti procesa.

Prikupljaju se sljedeća polja:

- **failureReason** – niz – označava koji je neuspjeh korisnik ponovio. Kao što je „provisioningFailed”, „purchaseFailed”, „activationFailed”.

- **productId** – niz – ID proizvoda trgovine App Store za koji korisnik ponovno pokušava neuspjeli zahtjev


#### <a name="officemanageabilityserviceapplypolicy"></a>Office.Manageability.Service.ApplyPolicy

Ključna telemetrija za praćenje neuspjeha\\uspjeha primjene postavki pravilnika za oblak na registar. LastError govori zašto i gdje primjena pravilnika na registar nije uspjela.

Prikupljaju se sljedeća polja:

  - **Data.ApplyLogMsg** – poruka o iznimci ako je bilo iznimaka tijekom primjene pravilnika

  - **Data.Cid** – dinamički generiran korelacijski identifikator koji se šalje servisu prilikom pozivanja servisa radi dohvaćanja pravilnika za oblak. Koristi se za utvrđivanje korelacije s pozivom koji uzrokuje problem tijekom primjene pravilnika na oblak.

  - **Data.Last Error** – jedna od pet vrijednosti niza (enumeratora) koja se koristi da bi se zabilježilo koja se faza primjene pravilnika izvršavala u trenutku kada je došlo do iznimke

#### <a name="officeonenoteandroidsyncprovisioningcompleted"></a>Office.OneNote.Android.Sync.ProvisioningCompleted

*[Ovaj je događaj prethodno imenovan OneNote.Sync.ProvisioningCompleted.]*

Kritični signal koji se koristi za osiguravanje da se, nakon što se korisnik prijavi u aplikaciju OneNote za platformu Android, bilježnice pravilno dodijele kako bi im se moglo jednostavno pristupiti. To se koristi za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge

Prikupljaju se sljedeća polja: 

- **AppSuspendedDuringEvent** – vraća Booleovu vrijednost koja označava je li aplikacija obustavljena tijekom dodjele resursa

- **NetworkConnection** – vrsta mrežne povezivosti uređaja koji se koristi

- **NetworkDataExchange** – bilježi broj bajtova razmijenjenih tijekom dodjele resursa.

- **ServerType** – vraća vrstu poslužitelja koji nudi uslugu

- **TimeTakenInMilliSeconds** – vraća vrijeme koje je potrebno za dovršavanje dodjele resursa u milisekundama

#### <a name="officeonenoteandroidsyncprovisioningerror"></a>Office.OneNote.Android.Sync.ProvisioningError

Kritični signal koji se koristi za osiguravanje da se, nakon što se korisnik prijavi u aplikaciju OneNote za platformu Android, bilježnice pravilno dodijele kako bi im se moglo jednostavno pristupiti. To se upotrebljava za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge.

Prikupljaju se sljedeća polja:

- **AppSuspendedDuringEvent**: vraća Booleovu vrijednost koja označava je li aplikacija obustavljena tijekom dodjele resursa

- **ErrorCode** – vraća šifru pogreške odgovorne za neuspjeh dodjele resursa. 

- **NetworkConnection**: vrsta mrežne povezivosti uređaja koji se koristi

- **NetworkDataExchange** – bilježi broj bajtova razmijenjenih tijekom dodjele resursa.

- **ServerType**: vraća vrstu poslužitelja koji nudi uslugu

- **TimeTakenInMilliSeconds**: vraća vrijeme koje je potrebno za dovršavanje dodjele resursa u milisekundama


#### <a name="officeonenoteandroidsyncprovisioningstarted"></a>Office.OneNote.Android.Sync.ProvisioningStarted

*[Ovaj je događaj prethodno imenovanOneNote.Sync.ProvisioningStarted.]*

Kritični signal koji se koristi za osiguravanje da se, nakon što se korisnik prijavi u aplikaciju OneNote za platformu Android, bilježnice pravilno dodijele kako bi im se moglo jednostavno pristupiti.  To se koristi za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge

Prikupljaju se sljedeća polja: 

- **NetworkConnection** – vrsta mrežne povezivosti uređaja koji se koristi

- **ServerType** – vraća vrstu poslužitelja koji nudi uslugu

#### <a name="officeonenotesystembootdialogssafebootdialogpending"></a>Office.OneNote.System.BootDialogs.SafeBootDialogPending 

Ključni znak koji se upotrebljava za praćenje kada odlučimo prikazati korisniku dijaloški okvir za sigurno pokretanje pri sljedećem pokretanju jer smo se neprekidno rušili više puta. To se upotrebljava za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. Ako korisnici vide dijaloški okvir za sigurno pokretanje, imamo kritičnu pogrešku rušenja sigurnog pokretanja i ta će nam informacija pomoći da znamo koliko se korisnika suočava s tim problemom i koliko će korisnika ponovno pokrenuti aplikaciju da bi zapravo vidjeli dijaloški okvir za sigurnu pokretanje naspram broja korisnika koji se neće vratiti.

Prikupljaju se sljedeća polja:

 - Nijedno

#### <a name="officeoutlookdesktopbootperfmetrics"></a>Office.Outlook.Desktop.BootPerfMetrics

Prikuplja podatke o trajanju pokretanja programa Outlook. Trajanje pokretanja programa Outlook aktivno se nadzire radi otkrivanja i dijagnostike nazadovanja. Koristi se i za dijagnosticiranje eskalacija od strane korisnika, i za poboljšavanje performansi pokretanja s vremenom.

Prikupljaju se sljedeća polja:

  - **AddinElapsedTotal** – ukupno vrijeme utrošeno na učitavanje dodataka

  - **CredPromptCount** – broj prikazanih upita za vjerodajnice

  - **ElapsedTotal** – ukupno vrijeme utrošeno na pokretanje

  - **IsLoggingEnabled** – je li omogućeno bilježenje u zapisnik

  - **ShowChooseProfileDlg** – je li se prikazao dijaloški okvir Odabir profila

  - **ShowFirstRunDlg** – je li se Outlook pokretao po prvi put

  - **ShowIMAPSrchfldWarningDlg** – upozorenja u slučaju da imamo IMAP račun s ANSI PST datotekom

  - **ShowNeedSupportDlg** – neuspjelo pokretanje potaknulo je otvaranje dijaloškog okvira za podršku

  - **ShowSafeModeDlg** – je li se sesija otvorila u sigurnom načinu rada

  - **ShowScanPstDlg** – provjera popravka pohrane prikazala je poruku o pogrešci


#### <a name="officeoutlookmacbootperf"></a>Office.Outlook.Mac.BootPerf

Prikuplja podatke o trajanju pokretanja programa Outlook. Trajanje pokretanja programa Outlook aktivno se nadzire radi otkrivanja i dijagnostike nazadovanja. Koristi se i za dijagnosticiranje eskalacija od strane korisnika, i za poboljšavanje performansi pokretanja s vremenom.

Prikupljaju se sljedeća polja:

- **MacOLKBootPerfDuration** – ukupno vrijeme utrošeno na pokretanje

- **MacOLKBootPerfID** – identifikator za vrijeme utrošeno na pokretanje


#### <a name="officeoutlookmacperformanceunresponsive"></a>Office.Outlook.Mac.PerformanceUnresponsive

Koristi se za identificiranje problema u programu Outlook koje utječu na korisnike i koje se mogu manifestirati kao smanjena kvaliteta performansi. 

Prikupljaju se sljedeća polja:

- **Duration** – vrijeme proteklo od smanjene kvalitete performansi

- **EventType** – vrsta događaja koji bilježi smanjenu kvalitetu performansi


#### <a name="officeperformanceboot"></a>Office.Performance.Boot

Prikuplja se tijekom pokretanja aplikacije sustava Office. Obuhvaća utvrđivanje je li pokretanje pokrenuto otvaranjem datoteke ili pokretanjem putem izbornika Start, je li to bilo prvo pokretanje aplikacije, koliko memorije aplikacija koristi te je li korisniku prikazano blokirajuće korisničko sučelje. Koristi se za mjerenje brzine pokretanja aplikacija sustava Office i koliko memorije one koriste tijekom pokretanja kako bi se osigurao prihvatljiv korisnički doživljaj.

Prikupljaju se sljedeća polja:

- **ActivationKind** – je li aplikacija pokrenuta pokretanjem putem izbornika Start, otvaranjem datoteke ili putem OLE automatizacije.
  
- **BootTostart** – je li korisnik odabrao prikazivanje početnog zaslona kada se aplikacija pokrene.

- **ColdBoot** – je li aplikacija sustava Office pokrenuta prvi put nakon ponovnog pokretanja sustava ili se binarni podaci aplikacije moraju učitati s diska.

- **DeviceModel** – model uređaja.

- **DocLocation** – kod otvaranja dokumenta označava koji je servis dobavio dokument (OneDrive, File Server, SharePoint itd.).

- **DurationUntilMso20Initialization** – trajanje u mikrosekundama između pokretanja procesa sustava Office i učitavanja mso20win32client.dll-a.

- **Embedding** – je li aplikacija otvorena za OLE ulaganje.

- **FirstBoot** – je li ovo bilo prvo pokretanje aplikacije.

- **InitializationDuration** – trajanje u mikrosekundama koje je bilo potrebno za prvo pokretanje procesa sustava Office.

- **InterruptionMessageId** – je li pokretanje prekinuo dijaloški okvir koji je tražio korisnički unos, ID dijaloškog okvira.

- **LegacyDuration** – koliko je dugo trebalo da se aktivnost izvrši, izmjereno koristeći različite početne i završne točke u odnosu na Activity.Duration.

- **OpenAsNew** – je li aplikacija pokrenuta otvaranjem postojećeg dokumenta kao predloška za novi dokument.

- **TotalWorkingSetMB** – količina memorije u megabajtima u radnom skupu procesa.

- **VirtualSetMB** – količina memorije u megabajtima u virtualnom skupu procesa. (samo za MacOS / iOS)

- **WorkingSetPeakMB** – najveća količina memorije u megabajtima koja se ikad dosad nalazila u radnom skupu procesa.


#### <a name="officepowerpointpptandroidrehearseview"></a>Office.PowerPoint.PPT.Android.RehearseView

Ovaj događaj označava da je korisnik prekinuo sesiju probe. U kombinaciji s Office.PowerPoint.PPT.Android.RehearseView.StartSession ovo će biti prvi indikator bilo kojeg zaustavljanja ili pogreški s kojima se korisnik suočava.

Prikupljaju se sljedeća polja:

- **ConnectionCreationTime** – vrijeme potrebno za stvaranje veza na strani poslužitelja.

- **CountDownAlertTime** – vrijeme za koje je prikazano upozorenje za odbrojavanje.

- **CountdownInitTime –** vrijeme između dovršetka učitavanja dijaprojekcije i početka odbrojavanja.

- **CritiqueSummary** – sažetak onoga što će svi korisnici-kritičari vidjeti na svojim brojačima.

- **ExitEventCode** – kôd za prepoznavanje u kojem scenariju korisnik izlazi iz sesije vježbanja, bez obzira na to je li riječ o scenariju pogreške ili uspješnom izlazu. 

- **FRETime** – Vrijeme između početka prikazivanja zaslona s početnim sučeljem i vremena dok ga korisnik nije odbacio. 

- **MikrophonePermissionTime** – vrijeme tijekom kojeg je prikazano upozorenje o dozvolama mikrofona dok korisnik ne odabere jednu od mogućnosti.

- **PauseRehearsingCount** – koliko je puta korisnik kliknuo na pauziranje probe.

- **RehearsalInitTime** vrijeme koje je probi bilo potrebno za inicijalizaciju.

- **ResumeRehearsingCount** – koliko je puta korisnik kliknuo na nastavak probe.

- **Sessionid** – Ovo je ID sjednice govornog ulaza. Koristi se za ispravljanje pogrešaka u zapisnicima servisa.

- **SlideshowViewLoadTime** – vrijeme učitavanja dijaprojekcije.


#### <a name="officepowerpointpptandroidrehearseviewrehearsalsummarypage"></a>Office.PowerPoint.PPT.Android.RehearseView.RehearsalSummaryPage 

Događaj se aktivira prilikom učitavanja stranice sažetka. Taj nam događaj pomaže pri snimanju izvedbe stranice sažetka. Govori nam koliko je vremena potrebno da se stranica servisa sa sažetkom probe učita na klijentu. Potrebno je održavati performanse značajke. 

Prikupljaju se sljedeća polja:

- **PayloadCreationTime** – vrijeme koje je potrebno u milisekundama za stvaranje opterećenja. 

- **PostUrlCallTime** – vrijeme koje je potrebno u milisekundama za slanje naknadnog URL poziva. 

- **RehearseSessionid** – to je ID sesije ulaznih vrata govora. Može se koristiti za ispravljanje pogrešaka u zapisnicima servisa.

- **RequestPayloadSize** – to je veličina zatraženog opterećenja. 

- **ResourcesLoadTime** – to je vrijeme u milisekundama koje je potrebno za učitavanje resursa (js, css). 

- **SummaryPageErrorReceived** – to je Booleova vrijednost koja pokazuje je li primljena stranica sažetka ili je došlo do pogreške.

- **SummaryPageHtmlLoadTime** – to je vrijeme u milisekundama koje je potrebno za učitavanje summarypageHtml. 

- **SummaryPageLoadStartTime** – to je vrijeme u milisekundama za primanje prvog odgovora s poslužitelja. 

- **SummaryPageLoadTime** – vrijeme (u ms) potrebno za učitavanje stranice sažetka. To obuhvaća vrijeme stvaranja opterećenja 

- **ThumbnailsCount** – to je ukupan broj minijatura koje će biti dio stranice sažetka. 

#### <a name="officepowerpointpptandroidrehearseviewstartsession"></a>Office.PowerPoint.PPT.Android.RehearseView.StartSession

Događaj se aktivira kada korisnik klikne na sesiju početka. Taj nam događaj pomaže pri snimanju broja korisnika koji upotrebljavaju značajku trenera za prezentacije na uređaju sa sustavom Android. U kombinaciji s Office.PowerPoint.PPT.Android.RehearseView reći će nam koliko je korisnika uspješno dovršilo sesiju probe i koliko ih nije moglo to napraviti. To je naš prvi indikator rušenja ili pogrešaka u značajci.
 
Prikupljaju se sljedeća polja:

 - Nijedno


#### <a name="officepowerpointpptsharedrehearseviewerrors"></a>Office.PowerPoint.PPT.Shared.RehearseView.Errors

*[Ovaj je događaj prethodno imenovan Office.PowerPoint.PPT.Android.RehearseView.Errors]*

Događaj koji se aktivira kada se pojavi bilo koja pogreška. Taj će nam događaj pomoći da znamo pogreške s kojima se korisnik suočio i pomoći će performansama trenera za prezentacije na mobilnom uređaju.

Prikupljaju se sljedeća polja:

- **Session ID** – ID sesije probe

- **RehearsalEventCode** – kod pogreške probe


#### <a name="officepowerpointrehearsalsessionmetrics"></a>Office.PowerPoint.Rehearsal.SessionMetrics 

Događaj koji se aktivira prilikom zaustavljanja sesije govora trenera za prezentacije. Taj nam događaj pomaže pri hvatanju nekih metričkih podataka za sesiju vježbe u treneru za prezentacije. To će pripomoći održavanje visoke kvalitete usluge za tu značajku.

Prikupljaju se sljedeća polja:

- **ActualRehearseBootTimeInMs** – to je stvarno utrošeno vrijeme za stvaranje veza.

- **AdaptationTextSize** – to je veličina teksta koji se šalje u servis.

- **AuthDurationInMs** – to je vrijeme u milisekundama potrebno za provjeru autentičnosti (osvježavanje tokena za provjeru autentičnosti).

- **AuthError** – opisuje pogrešku provjere autentičnosti koja se dogodila (ako se dogodila).

- **AvgFragmentLatencyInMs** – to je prosječno vrijeme povratnog putovanja mrežne govorne poruke.

- **ConnectDurationInMs** – to je vrijeme u milisekundama potrebno da sesija dovrši povezivanje. 

- **FirstAudioDelayInMs** – to je vrijeme u milisekundama potrebno za primanje prvih audiopodataka.

- **FRetriedOnOpenConnection** – to je Booleova vrijednost koja pokazuje je li došlo do ponovnog pokušaja za openconnection ili nije.

- **InitMediaCaptureLayerDurationInMs** – to je vrijeme u milisekundama potrebno za inicijalizaciju sloja za snimanje medijskih sadržaja / audiozapisa.

- **LocallyDroppedMessageCount** – to je ukupan broj lokalno ispuštenih poruka.

- **NumReconnectAttemptsDuringSession** – to pokazuje koliko je puta pokušano ponovno povezivanje na speechservice.

- **NumTriesDuringEachReconnectAttempt** – to je polje koje pokazuje broj izvršenih pokušaja tijekom svakog pokušaja ponovnog povezivanja.

- **OpenFrontDoorConnectionDurationInMs** – to je vrijeme u milisekundama potrebno za otvaranje veze sa servisom FrontDoor.

- **SendAdaptationTextDurationInMs** – to je vrijeme u milisekundama potrebno za slanje adaptacijskog teksta servisu.

- **ServiceDroppedMessageCount** – to je ukupan broj poruka koje je servis ispustio.

- **SessionDurationInMs** – to je vrijeme trajanja cijele sesije od kada je korisnik kliknuo za početak do kada je kliknuo za kraj.

- **Sessionid** – to je ID sjednice govornog ulaza. Može se koristiti za ispravljanje pogrešaka u zapisnicima servisa.

- **SpeechClientResultEventsWithTimestamps** – to je polje kodova pogrešaka primljenih zajedno s vremenskim oznakama, koji vam mogu pomoći pri otklanjanju pogrešaka.

- **SpeechHResultsWithTimestamps** – to je polje kodova pogrešaka primljenih zajedno s vremenskim oznakama, koji vam mogu pomoći pri otklanjanju pogrešaka.

- **StartSpeechCaptureDurationInMs** – to je vrijeme u milisekundama potrebno za početak snimanja govora.

- **StartSpeechServiceDurationInMs** – to je polje vremena koliko je potrebno da sesija govora započne svaki put kada dođe do ponovnog povezivanja, uključujući trajanje prve pokrenute sesije govora. 

- **TotalMessageCount** – to je ukupan broj audioporuka poslanih servisu.

- **WebSocketConnectDurationInMs** – to je vrijeme u milisekundama potrebno za dovršenje povezivanja s web-utičnicom.


#### <a name="officeuxofficeinsidercanshowofficeinsiderslab"></a>Office.UX.OfficeInsider.CanShowOfficeInsiderSlab

Praćenje aktivnosti za utvrđivanje može li se ploča Office Insider prikazati korisniku u kartici Račun u korisničkom sučelju Backstage sustava Office.

Prikupljaju se sljedeća polja:

  - **Data_CanShow** – označava može li se ploča Office Insider prikazati korisniku u kartici Račun u korisničkom sučelju Backstage sustava Office.
  
  - **Data_Event** – neiskorišteno

  - **Data_EventInfo** – neiskorišteno

  - **Data_Reason** – neiskorišteno
 

#### <a name="officeuxofficeinsiderregistercurrentinsider"></a>Office.UX.OfficeInsider.RegisterCurrentInsider

Kritični signal za praćenje uspjeha ili pogreške prilikom registracije korisnika pomoću međuverzija sustava Office Insider koji prije nisu registrirani kao sudionici sustava Office Insider. Glavni scenarij za to su trenutačni sudionici programa Office Insider koji su se uključili u program Office Insider prije no što je dodana registracija programa Office Insider.

Prikupljaju se sljedeća polja:

- **Data_RegisterInsider** – stanje registracije programa Office Insider

- **Data_RegisterInsiderHr** – kod rezultata za registraciju programa Office Insider

- **Data_RegistrationStateCurrent** – trenutno stanje registracije

- **Data_RegistrationStateDesired** – zatraženo stanje registracije


#### <a name="officeuxofficeinsidershowofficeinsiderdlg"></a>Office.UX.OfficeInsider.ShowOfficeInsiderDlg

Ključni signal koji prati interakciju korisnika s dijaloškim okvirom Join Office Insider. Koristi se za prepoznavanje svih problema u provedbi promjena koje je pokrenuo korisnik kao što su pridruživanje ili napuštanje programa Office Insider i promjena razine programa Office Insider.

Prikupljaju se sljedeća polja:

- **Data_AcceptedContactMeNew** – označava je li korisnik prihvatio da ga Microsoft kontaktira nakon pridruživanja programu Office Insider

- **Data_InsiderLevel** – razina programa Insider tijekom otvaranja dijaloškog okvira „Pridruživanje programu Office Insider”

- **Data_InsiderLevelNew** – razina programa Insider tijekom zatvaranja dijaloškog okvira „Pridruživanje programu Office Insider”

- **Data_IsInternalUser** – označava pokreće li se aplikacija putem vjerodajnica Microsoftova poslovnog računa.

- **Data_IsInternalUser** – označava može li kod utvrditi pokreće li se aplikacija putem vjerodajnica Microsoftova poslovnog računa.

- **Data_OpenNewsletterWebpage** – označava je li poveznica za pretplatu na bilten programa Office Insider aktivirana pod uvjetom da se korisnik pridružio programu Office Insider, da je značajka pretplate na bilten omogućena i da korisnik nije otkazao otvaranje web-mjesta pretplate na bilten programa Office Insider.
    
- **Data_RegisterInsider** – stanje registracije programa Office Insider

- **Data_RegisterInsiderHr** – kod rezultata za registraciju programa Office Insider

- **Data_RegistrationStateCurrent** – trenutno stanje registracije

- **Data_RegistrationStateDesired** – zatraženo stanje registracije


#### <a name="officevisiosharedvisiofilerender"></a>Office.Visio.Shared.VisioFileRender

Taj događaj bilježi trajanje vizualizacije datoteke. Taj nam događaj pomaže paziti na performanse vizualizacije datoteka.

Prikupljaju se sljedeća polja:

  - **Data\_AvgTime: integer** – prosječno trajanje vizualizacije crteža programa Visio u sesiji

  - **Data\_CompositeSurfEnabled: bool** – istinito znači da je omogućen kombinirani način vizualizacije

  - **Data\_Count: integer** – broj vizualizacija crteža u sesiji programa Visio

  - **Data\_FirstRenderTime: long** – trajanje vizualizacije datoteke prilikom prvog pokretanja, u milisekundama

  - **Data\_MaxTime: integer** – maksimalno trajanje vizualizacije crteža programa Visio u sesiji


#### <a name="officevisiovisiofileopenreliability"></a>Office.Visio.VisioFileOpenReliability

Taj događaj prikuplja podatke o performansama otvaranja datoteka za Visio Dev16. Taj se događaj koristi za praćenje performansi otvaranja datoteka u programu Visio Dev16 i njihovo povezivanje sa svojstvima datoteke kao što je njezina veličina. Svojstva datoteke omogućuju nam brže ispravljanje pogrešaka i otkrivanje korijenskih uzroka problema.

Prikupljaju se sljedeća polja:

  - **Data\_CorrelationId: string –** korelacijski identifikator dokumenta

  - **Data\_DocIsEnterpriseProtected: bool –** istinito ako je dokument zaštićen zaštitom podataka u sustavu Windows

  - **Data\_DocumentId: string –** GUID puta datoteke

  - **Data\_DurationToCompleteInMilliseconds:double –** trajanje spremanja u milisekundama

  - **Data\_DurationToCompleteInMillisecondsSquared: double –** kvadrat vrijednosti DurationToCompleteInMilliseconds

  - **Data\_ErrorCode: integer –** interni kod pogreške pri neuspjelom otvaranju datoteke

  - **Data\_Extension\_Docs: string –** datotečni nastavak otvorenog dijagrama

  - **Data\_FileIOBytesRead: int –** ukupan broj bajtova pročitanih prilikom spremanja

  - **Data\_FileIOBytesReadSquared: int –** kvadrat vrijednosti Data\_FileIOBytesRead

  - **Data\_FileIOBytesWritten: int –** ukupan broj bajtova zapisanih prilikom spremanja

  - **Data\_FileIOBytesWrittenSquared: int–** kvadrat vrijednosti Data\_FileIOBytesWritten

  - **Data\_FileName:binary** – binarno raspršivanje naziva datoteke

  - **Data\_FileOpenDownloadDurationInMs: long –** trajanje preuzimanja datoteke u milisekundama

  - **Data\_FileOpenEndDurationInMs: long: –** trajanje otvaranja datoteke u milisekundama

  - **Data\_FileOpenTimeStamp: time: –** vremenska oznaka u trenutku početka otvaranja datoteke

  - **Data\_FilePathHash: binary –** GUID puta datoteke

  - **Data\_FileSize: long –** veličina dokumenta u bajtovima

  - **Data\_FileType: string –** datotečni nastavak otvorenog dijagrama

  - **Data\_IsInternalFile: bool –** istinito ako je datoteka interna datoteka. Na primjer, Šablona

  - **Data\_IsIRM:bool –** istinito ako je datoteka zaštićena pravima na informacije

  - **Data\_IsReadOnly: bool –** istinito ako je datoteka samo za čitanje

  - **Data\_IsSuccess: bool –** istinito kada je otvaranje datoteke uspješno

  - **Data\_Location: string –** lokacija datoteke, kao što je lokalno, SharePoint, OneDrive, WopiConsumer, WopiBusiness, GenericThirdPartyConsumer

  - **Data\_NetworkIOBytesRead: int –** ukupan broj mrežnih bajtova pročitanih prilikom spremanja

  - **Data\_NetworkIOBytesReadSquared: int –** kvadrat vrijednosti Data\_NetworkIOBytesRead

  - **Data\_NetworkIOBytesWritten: int –** ukupan broj mrežnih bajtova zapisanih prilikom spremanja

  - **Data\_NetworkIOBytesWrittenSquared: int –** kvadrat vrijednosti NetworkIOBytesWritten

  - **Data\_OpenLocation: integer –** lokacija s koje je datoteka otvorena: 0, lokalno, 1, mreža, 2, SharePoint, 3 – web

  - **Data\_Size\_Docs: integer –** veličina dokumenta u bajtovima

  - **Data\_Tag: string –** jedinstveni identifikator za prepoznavanje događaja „Spremi kao”

  - **Data\_WasSuccessful: bool –** istinito ako je otvaranje bilo uspješno


#### <a name="onenoteappsafebootdialogactiontaken-officeonenoteandroidsafebootdialogactiontaken-officeandroidearlytelemetrysafebootdialogactiontaken"></a>OneNote.App.SafeBootDialogActionTaken, Office.OneNote.Android.SafeBootDialogActionTaken, Office.Android.EarlyTelemetry.SafeBootDialogActionTaken

Ključni znak koji se koristi za praćenje korisnikovog odgovora kada korisnik vidi dijalog sigurnog pokretanja. Dijaloški se okvir sigurnog pokretanja prikazuje kada uzastopno pokretanje nije moguće. Odabir se korisnika za sigurno pokretanje upotrebljava u obliku dozvole za brisanje podataka u aplikaciji radi uspješnog pokretanja. To se upotrebljava za osiguravanje prepoznavanja ključne regresije za aplikaciju OneNote i stanje usluge. Korisnik vidi kada će naići na kritičnu pogrešku rušenja sigurnog pokretanja. S pomoću te informacije ćemo moći pratiti je li uzrok zatvaranja riješen i može li korisnik uspješno pokrenuti aplikaciju ili ne.

Prikupljaju se sljedeća polja: 

- **DIALOG_ACTION** – na koji je gumb dijaloškog okvira korisnik kliknuo – pozitivni gumb ili negativni gumb


#### <a name="perfevent"></a>perf.event

Koristi se za praćenje mogućih negativnih utjecaja na funkciju učitavanja različitih dijelova aplikacije, primjerice za osiguravanje da se vaša ulazna pošta što brže učitava tijekom prvog otvaranja aplikacije.

Prikupljaju se sljedeća polja: 

- **app_start_show_message_list** – to znači da je došlo do problema s funkcijom u okviru pokretanja aplikacije, što je dovelo do dugačkog učitavanja popisa poruka vaše ulazne pošte

- **Prosječna** – sakuplja iznos ponovnih učitavanja koji se događaju u razgovoru podijeljen s količinom poruka u tom razgovoru.  

- **event_type** – govori nam vrstu događaja funkcije koji je doveo do problema s funkcijom kako bi nam pomogao prepoznati probleme u vezi s određenom vrstom.   

- **extra_params** – razvojni inženjer ovdje može dodati dodatne parametre kako bi nam pomogao pružiti više pojedinosti o tome što bi moglo uzrokovati ovaj problem s funkcijom, odnosno, kada je ova radnja započela i završila itd. 

-   **has_work_profile** – označava radi li aplikacija pod Android Work Profile ili sličnom konfiguracijom kako bi se analiza izvedbe povezala s tim okruženjima.

- **profiling_summary** – omogućuje informacije o grupi zadataka, broju zadataka i prosječnom vremenu za te grupe da biste bolje razumjeli potencijalne regresije u pojedinim područjima prilikom učitavanja aplikacije.

- **runtime_performance_monitoring_data** – pruža podatke o izvedbi (vrijeme učitavanja, brojanje zapisa) prilikom učitavanja podataka u različitim dijelovima aplikacije.
  - **average_cost_time_ns** –prosječno vrijeme troška mjereno u nanosekundama.
  - **cost_type** – govori nam je li taj događaj namijenjen za mjerenje izvršenja sloja prostora za pohranu ili cjelokupno trajanje.
  - **hx_object_type** – pruža detaljni tip objekta mjerenja.
  - **is_main_thread** – govori nam mjeri li ovaj događaj samo vrijeme izvršenja glavne niti.
  - **record_count** – broj zapisa koje vraća pozadinski sloj za pohranu.
  - **scope_name** – predstavlja naziv stranice/komponenti korisničkog sučelja kojoj taj događaj pripada.
  - **average_cost_time_ns** – ukupno vrijeme troška mjereno u nanosekundama. 

- **total_time_elapsed** – govori nam koliko je događaj funkcije trajao kako bi nam pomogao razumjeti ozbiljnost problema s funkcijom

#### <a name="performancerecord"></a>performance.record

Ovim se događajem prikuplja metrika performansi aplikacije. Omogućuje nam otkrivanje i rješavanje situacija kada iskorištenost memorije aplikacije i CPU postanu kritično visoki ili postoje neki drugi problemi s performansama, što može dovesti do usporavanja vašeg uređaja.

Prikupljaju se sljedeća polja: 

- **app_exit_metric** – javlja nam metriku o broju različitih vrsti performansi za prednji i pozadinski izlaz iz aplikacije, kao pomoć u razumijevanju neočekivanog izlaska iz aplikacije s razlozima negativnih performansi.

- **average_suspended_memory** – javlja nam prosječnu količinu memorije koju aplikacija upotrebljava kada je obustavljena kako bismo imali vrijednost za usporedbu i kako bismo razumjeli negativan učinak na funkciju.

- **category** – govori nam je li aplikacija u određenom trenutku u prvom planu ili pozadini. Moguće vrijednosti uključuju prvi plan ili pozadinu.

- **cpu_usage** – govori nam koliko je CPU-a aplikacija koristila kako bismo imali vrijednost za usporedbu i kako bismo razumjeli negativan učinak na funkciju

- **cumulative_CPU_time** – govori nam koliko ukupno CPU-a aplikacija koristi s mjerenjem trajanja kako bismo imali vrijednost za usporedbu i kako bismo razumjeli negativan učinak na funkciju.

- **cumulative_GPU_time** – govori nam koliko ukupno GPU vremena aplikacija koristi kako bismo imali vrijednost za usporedbu i kako bismo razumjeli negativan utjecaj vijeka trajanja baterije.

- **is_watch_app_installed** – govori nam koristi li korisnik trenutno uređaj Apple Watch te je li on instaliran kako bi nam pomogao razumjeti negativan utjecaj na funkciju zbog uređaja Watch

- **is_watch_paired** – govori nam koristi li korisnik trenutno uređaj Apple Watch te je li on uparen s uređajem kako bi nam pomogao razumjeti negativan utjecaj na funkciju zbog uređaja Watch

- **is_watch_supported_and_active** – govori nam koristi li korisnik trenutno uređaj Apple Watch te je li on aktivan kako bi nam pomogao razumjeti negativan utjecaj na funkciju zbog uređaja Watch

- **memoAry_used_percentage** – govori nam koji je postotak memorije aplikacija koristila kako bismo imali vrijednost za usporedbu i kako bismo razumjeli negativan učinak na funkciju

- **memory_used** – govori nam koliko je memorije aplikacija koristila kako bismo imali vrijednost za usporedbu i kako bismo razumjeli negativan učinak na funkciju

- **peak_memory_usage** – govori nam koliko je najviše memorije aplikacija koristila kako bismo imali vrijednost za usporedbu i kako bismo razumjeli negativan učinak na funkciju.

- **scroll_hitch_time_ratio** – govori nam koji je omjer vremena proveden u zastoju tijekom kretanja kroz korisničko sučelje kako bismo razumjeli negativan utjecaj na učinak korisničkog sučelja.


### <a name="application-activity-error-subtype"></a>*Podvrsta pogreške aktivnosti aplikacije*

Pogreške u funkcioniranju značajke ili korisničkog okruženja.

#### <a name="assertion"></a>assertion

Ovaj nam događaj omogućuje otkrivanje kada su nastupile kritične pogreške aplikacije koje bi uzrokovale rušenje vaše aplikacije ili iskustvo ozbiljnih problema, primjerice prikaz praznih redaka u vašoj ulaznoj pošti.

Prikupljaju se sljedeća polja:

- **count** – ukupan broj stavki povezanih s pogreškom; primjerice, broj kalendara koji imaju pogreške

- **has_hx** – govori nam da račun koristi naš novi servis sinkronizacije kako bi nam pomogao prepoznati probleme uzrokovane našim servisom sinkronizacije

- **host_name** – naziv glavnog računala servisa koji je bio uključen u grešku kako bi nam pomogao prepoznati probleme u vezi s određenim glavnim računalom

- **host_type** – vrsta glavnog računala koje je bilo uključeno u pogrešku kako bi nam pomogao prepoznati probleme u vezi s vrstom određenog glavnog računala

- **message** – prilagođena poruka za označavanje da se koristi za dijagnozu problema 

- **origin** – podrijetlo pogreške u kodu koji nam pomaže prepoznavanje problema u vezi s određenim dijelom koda

- **stacktrace** – snop praćenja u kojem je označavanje nastupilo kako bi nam pomogao prepoznati probleme u vezi s određenim dijelom koda

- **type** – vrsta pogreške označavanja koja je nastupila, na primjer, null_folder_name, compose_selected_null_account, kako bi nam pomogao prepoznati probleme u vezi s određenim dijelom koda

#### <a name="editcontacterror"></a>edit.contact.error

Omogućuje nam otkrivanje i rješavanje situacija u okviru kojih su pogreške uzrokovane kada pokušavate vidjeti ili uređivati kontakte putem aplikacije.

Prikupljaju se sljedeća polja: 

- **errorType** – vrsta pogreške koja je nastupila kako bi nam pomogao dijagnosticirati problem

- **field** – polje kontakta koje je korisnik pokušao uređivati kako bi nam pomogao dijagnosticirati problem

- **version** – verzija servisa kartice kontakta koji koristimo kako bi nam pomogao dijagnosticirati problem

#### <a name="errorreport"></a>error.report

Ovaj nam događaj omogućuje prepoznati kada su nastupile kritične pogreške korištene aplikacije da bismo mogli spriječiti probleme koji mogu prouzročiti rušenje aplikacije ili vam onemogućiti čitanje e-pošte. 

Prikupljaju se sljedeća polja: 

- **client-request-id** – identifikator zahtjeva klijenta za zahtjev koji je uzrokovao pogrešku
 
- **date** – datumska oznaka zahtjeva koji je uzrokovao pogrešku

- **error** – vrsta pogreške, npr. get_mailbox_location_failed
 
- **error_body** – tijelo poruke o pogrešci
 
- **is_x_mailbox_anchor_set** – je li na zahtjevu bilo postavljeno svojstvo X-AnchorMailbox
 
- **reason** – razlog za pogrešku, odnosno, poruka o pogrešci
 
- **request-id** – identifikator zahtjeva poslužitelja za zahtjev koji je uzrokovao pogrešku
 
- **source** – izvor pogreške unutar infrastrukture modela objekta, u pravilu „BE” ili „FE”


#### <a name="officeairspacebackendwin32graphicsdriversofthang"></a>Office.AirSpace.Backend.Win32.GraphicsDriverSoftHang 

Pomaže Microsoftu razdvojiti duge blokade upravljačkog programa grafičke kartice od onih kratkih, što pak olakšava donošenje odluka o tome s kojim upravljačkim programima grafičkih kartica možda ima problema. Upravljački program grafičke kartice uzrokovao je blokadu sustava Office, ali utjecaj te blokade još nije poznat

Prikupljaju se sljedeća polja:

  - **Data\_InDeviceCall** – metoda primijenjena na grafičkoj kartici koja je uzrokovala blokadu

  - **Data\_Timeout** – trajanje blokade

  #### <a name="officeandroidadalsigninuiprompts"></a>Office.Android.ADALSignInUIPrompts

Tim se događajem označava da je upit za prijavu stigao korisniku, za školski ili poslovni račun.  Ovaj događaj pomaže u razumijevanju stanja prijava u našim aplikacijama i poduzima odgovarajuće radnje kada uočimo neočekivane ponovne upite za prijavu. 

Prikupljaju se sljedeća polja:

- **LastLoginDelta** – delta vremena od posljednje uspješne prijave.

- **PreviousIdentityCredProviderState** – označava stanje računa.

- **PreviousIdentityState** – označava stanje računa, poput isteka sesije. 

- **SignInResultCode** – označava kôd rezultata za kraj upita za prijavu.

- **UseCache** – označava smo li prisilno zatražili korisniku da ponovno unese lozinku.

- **UserType** – upućuje na to je li riječ o postojećem računu ili novom računu

#### <a name="officeandroidandroidappdocsfileoperationends"></a>Office.Android.AndroidAppDocsFileOperationEnds

Ključna dokumenta samo za Android (AppDocs) podaci telemetrije za kraj operacija Datoteka/Novo/Spremi kao. Ovo bilježi kodove pogrešaka za neuspjehe tih AppDocs operacija.  Microsoft to koristi za identificiranje kvarova u različitim operacijama datoteka i točnog sloja na kojem se kvar dogodio u programu Word, Excel ili PowerPoint.

Prikupljaju se sljedeća polja:

- **AccessMode** – vrijednost enumeracije za način pristupa datoteci. Vrijednost – nema, samo za čitanje, samo za čitanje koja se može nadograditi, za čitanje i pisanje

- **BlockingUIShown** – Booleova vrijednost koja označava je li blokiranje korisničkog sučelja bilo prikazano bilo gdje u protoku.

- **ContentUriAuthority** – autoritet URL-a za sadržaj iz SAF-a

- **Correlation** – GUID za ID korelacije koji se odnosi na operaciju

- **DocId** – ID dokumenta koji je generirao AppDocs

- **DocInstanceId** – DocInstanceId ID instance dokumenta koji generira AppDocs koji je obuhvaćen instancom operacije u dokumentu

- **DocIsEnterpriseProtected** – Booleova vrijednost koja označava je li dokument zaštićen.

- **DocUserId** – korisnički ID iz MS sloja za autorizaciju

- **DocUserIdProvider** – enumeracija koja predstavlja davatelja korisničkog ID-a, 0 = Nepoznato, 1 = LiveId, 2 = OrgId, 3 = SSPI, 4 = ADAL

- **DurationInMs** – vrijeme u milisekundama do završetka operacije datoteke

- **EndReason** – vrijednost enumeracije za krajnji razlog.  Vrijednosti – nema, uspjeh, neuspjeh, odustani

- **ErrorCode** – kôd pogreške za operaciju datoteke

- **Extension** – proširenje datoteke koja se otvara.

- **FileSourceLocation** – vrijednost enumeracije lokacije datoteke. Moguće vrijednosti: Nema, Lokalno, UncOrMappedNetworkDrive, SkyDrive, App, SharePoint, Nepoznati poslužitelj

- **FILETIME** – vrijeme događaja

- **FirstBCSClientError_Info** – informacije o kodu pogreške povezane s pretvorbama datoteka

- **HttpStatusCode** – http kôd odgovora za zahtjev web usluge

- **InitalizationReason** – ulazna točka za otvaranje datoteke

- **K2FileIOHresult** – Hresult kôd za kraj operacije otvaranja datoteke

- **LastBCSClientError_TagId** – posljednja pogreška BSC (usluga binarne pretvorbe) klijenta

- **OfficeWebServiceApiStatusFlag** – zastavica statusa za zahtjev web usluge

- **OpEndEventId** – oznaka koja predstavlja mjesto gdje je operacija zapravo završila

- **OpFlags** – zastavice parametra operacije dokumenta koje koristi sloj AppDocs.

- **OpSeqNum** – broj koji predstavlja redoslijed poziva datoteka povezanih sa operacijom datoteke u sloju AppDocs

- **OpType** – enumeracija vrste operacija. Vrijednosti: "None", "CreateDocument", "OpenDocument", "CopyDocument", "CloseDocument", "SaveDocument", "OpenVersion", "CloseVersion"

- **PreFetchState**– enumeracija stanja pretpreuzimanja predložaka za operacije stvaranja nove datoteke.

- **ProviderApp** – naziv paketa aplikacije iz koje se datoteka otvara

- **ScopeInstanceId**– ID opsega instance koji se koristi za pridruživanje podatkovnog konteksta aktivnostima

- **Size** – veličina datoteke

- **State** – vrijednosti enumeracije za stanje datoteke. Vrijednosti: None, Creating, Created, CreateFailed, Opening, Opened, OpenFailed, Copying, Copied, CopyFailed, Closing, Closed, CloseFail

- **TemplateName** – naziv binarnog predloška dokumenta iz usluge predloška, npr. TF10002009.dotx

- **UriScheme** – shema URL-a

#### <a name="officeandroidandroidautherror"></a>Office.Android.AndroidAuthError

Ovaj događaj označava osnovne pogreške u provjeri autentičnosti za vrijeme tihog osvježavanja tokena, učitavanje stranice za prijavu iz usluge i tako dalje.  Ovaj događaj pomaže u razumijevanju stanja prijava u našim aplikacijama, pokušajima prijave i poduzima odgovarajuće radnje kada uočimo neočekivane ponovne upite za prijavu. 

Prikupljaju se sljedeća polja:

- **ADALErrorCode** – označava kôd pogreške prilikom prikazivanja upita za prijavu ili pokušaja dohvaćanja tihog tokena za poslovni račun.

- **ADALRawErrorCode** – označava kôd neobrađene pogreške prilikom prikazivanja upita za prijavu ili pokušaja dohvaćanja tihog tokena za poslovni račun.

- **ErrorGroup** – označava vrstu računa kao što je osobni račun ili poslovni račun ili lokalni poslovni račun.

- **IDCRLErrorCode** – označava kôd pogreške prilikom prikazivanja upita za prijavu za osobni račun.

- **IDCRLRawErrorCode** – označava kôd neobrađene pogreške prilikom prikazivanja upita za prijavu za osobni račun.

- **LiveOAuthErrorCode** – označava kôd pogreške prilikom pokušaja osvježavanja tihog tokena za osobni račun.

- **LiveOAuthRawErrorCode** – označava kôd neobrađene pogreške prilikom pokušaja osvježavanja tihog tokena za osobni račun.

- **NTLMErrorCode** – označava kôd pogreške prilikom prikazivanja upita za prijavu za lokalni poslovni račun.

#### <a name="officeandroidandroidfileasyncsavestatus"></a>Office.Android.AndroidFileAsyncSaveStatus

Snima asinkronu datoteku, sprema podatke o statusu i razne kodove pogrešaka iz različitih komponenti.  Microsoft koristi ove podatke kako bi analizirao postoji li gubitak korisničkih podataka u aplikaciji tijekom spremanja datoteka u aplikacijama Word, Excel ili PowerPoint.

Prikupljaju se sljedeća polja:

- **FileExtension** – datotečni nastavak

- **FileIOSaveHResult** – HResult za operaciju spremanja datoteke

- **FileIOSaveIsCopy** – Booleova vrijednost da naznači sprema li operacija kopiju.

- **FileSize** – veličina datoteke

- **FileSourceLocation** – enumeracija lokacije izvora datoteke. Vrijednosti: Nema, Lokalno, UncOrMappedNetworkDrive, SkyDrive, App, SharePoint, Nepoznati poslužitelj

#### <a name="officeandroidandroidfileopenreliability"></a>Office.Android.AndroidFileOpenReliability

To bilježi podatke o statusu otvaranja datoteke i različite kodove pogrešaka kako bi se utvrdilo koje se pogreške prilikom otvaranja datoteke očekuju, a koje ne i koji ih dio koda prijavljuje.  Microsoft upotrebljava ove podatke kako bi analizirao razloge neuspjeha otvaranja datoteka i izračunao ključnu metriku poput stope uspjeha otvaranja datoteke u aplikacijama Word, Excel ili PowerPoint.

Prikupljaju se sljedeća polja:

- **AccessMode** – enumeracija načina pristupa

- **AppDocsFileOpenErrorCode** – AppDocs kôd pogreške za neuspjeh otvaranja datoteke

- **ContentUriAuthority** – autoritet URL-a za sadržaj iz SAF-a

- **DownloadCsiError** – preuzimanje poruke o pogrešci sa CSI-ja

- **FileExtension** – datotečni nastavak

- **FileOpenEndErrorCode** – kôd pogreške za neuspjeh otvaranja datoteke

- **FileOpenStatus** – enumeracija statusa otvaranja datoteke

- **FileSize** – veličina datoteke

- **FileSourceLocation** – enumeracija lokacije datoteke

- **FirstBCSClientError_Info** – posljednja pogreška BSC (usluga binarne pretvorbe) klijenta

- **IfWordFileOpenCancelled** – ako je otvaranje datoteke otkazao korisnik u programu Word

- **InitializationReason** – enumeracija za ulaznu točku za otvaranje datoteke

- **IsAutoSaveDisabled** – je li automatsko spremanje onemogućeno tijekom otvaranja datoteke

- **IsFileEmpty** – Booleova vrijednost koja označava je li datoteka prazna

- **K2FileIOHresult** – Hresult za završetak operacije datoteke

- **OpenCsiError** – poruka o pogrešci otvaranja datoteke u CSI sloju

- **OpEndEventId** – oznaka gdje je operacija zapravo završila

- **PPTHresult** – Hresult u PPT-u

- **PPTIsExpectedError** – PPT klasifikacija pogrešaka za očekivani/neočekivani neuspjeh pri otvaranju datoteke 

- **PPTTag** – oznaka pogreške u PPT-u

- **ProviderApp** – naziv paketa aplikacije iz koje se datoteka otvara

- **ProviderFileSize** – veličina datoteke snimljena tijekom otvaranja datoteke putem aktivacije datoteke

- **State** – enumeracija statusa otvaranja datoteke

- **UriScheme** – shema URL-a

- **WordErrortag** – oznaka pogreške u programu Word

- **WordFileCorruptionReason** – razlog za oštećenje zbog kojeg se datoteka programa Word ne može otvoriti

- **WordFileOpenErrorCode** – kôd pogreške specifičan za otvaranje datoteke u programu Word.

- **WordFileTypeFromDod** – vrsta datoteke koja se određuje pomoću programa Word na temelju stvarnog oblika datoteke

- **WordFileTypeFromExtension** – vrsta datoteke koja se određuje pomoću programa Word na temelju datotečnog nastavka

#### <a name="officeandroidandroidfilesavestatus"></a>Office.Android.AndroidFileSaveStatus

Ključno za snimanje podataka o statusu spremanja datoteke i razne kodove pogrešaka iz različitih komponenti.  Microsoft koristi ove podatke kako bi analizirao postoji li gubitak korisničkih podataka u aplikaciji tijekom spremanja datoteka u aplikacijama Word, Excel ili PowerPoint.

Prikupljaju se sljedeća polja:

- **AccessMode** – Vrijednosti** – nema, samo za čitanje, samo za čitanje koja se može nadograditi, za čitanje i pisanje.

- **AppDocsEndReason** – enumeracija za spremanje datoteke Appdoc EndReason.  Vrijednosti – nema, uspjeh, neuspjeh, odustani.

- **AppDocsErrorCode** – krajnji kôd pogreške za neuspjeh pri spremanju datoteke

- **AppDocsTriggeringSaveDetails** – polje koje označava pokreće li AppDocs spremanje

- **DocInstanceId** – DocInstanceId ID instance dokumenta koji generira AppDocs koji je obuhvaćen instancom operacije u dokumentu

- **ExcelFileSaveResult** – HResult specifičan za program Excel

- **FileExtension** – proširenje datoteke.

- **FileIOSaveErrorCode** – kôd pogreške Ulaza/Izlaza datoteke

- **FileIOSaveHResult** – Hresult Ulaza/Izlaza datoteke

- **FileIOSaveIsCopy** – Booleova vrijednost koja označava je li ovo operacija kopiranja

- **FileSize** – veličina datoteke

- **FileSourceLocation** – enumeracija lokacije datoteke.  Vrijednosti: Nema, Lokalno, UncOrMappedNetworkDrive, SkyDrive, App, SharePoint, Nepoznati poslužitelj

- **OpFlags** – zastavice operacije za spremanje

- **PPTFileSaveFailHresult** – PPT hresult za neuspjeh spremanja

- **PPTFileSaveFailTag** – PPT oznaka za neuspjeh spremanja

- **State** – enumeracija statusa otvaranja datoteke. 

- **Values** – None, Creating, Created, CreateFailed, Opening, Opened, OpenFailed, Copying, Copied, CopyFailed, Closing, Closed, CloseFail

- **WordFileCopyErrorTrackbackTag** – oznaka evidentirane povratne veze za neuspjeh u fazi „CopyDocument“ u programu Word

- **WordFileSaveCancelReason** – oznaka evidentirane povratne veze za otkazivanje u programu Word

- **WordFileSaveEid** – kôd pogreške specifičan za program Word

- **WordFileSaveErrorTrackbackTag** – oznaka evidentirane povratne veze za spremanje neuspjeha

- **WordFileSaveOpResult** – enumeracija stanja rezultata 0 ako je uspjelo, 1 ako nije uspjelo, 2 ako je otkazano

- **WordFileSaveSuccess** – enumeracija detalja specifičnih za program Word za uspjeh operacije spremanja datoteke.

#### <a name="officeandroidandroidofficeactivationlatency"></a>Office.Android.AndroidOfficeActivationLatency

Ključni podaci za prikupljanje sveobuhvatnog vremena otvaranja datoteka za sva otvaranja datoteka u aplikacijama sustava Windows, Excel i PowerPoint.  To koristi Microsoft da bi saznao metriku performansi otvaranja datoteke naših aplikacija

Prikupljaju se sljedeća polja:

- **Appbootingocod** – Booleova vrijednost da biste provjerili je li dovršeno pokretanje aplikacije

- **ApplicationBootTime** – vrijeme potrebno tijekom određene faze pokretanja aplikacije

- **AppSuspendedDuringBoot** – Booleova vrijednost koja provjerava je li aplikacija obustavljena tijekom pokretanja

- **BlockingUIShownDuringFileOpen** – Booleova vrijednost koja označava je li postojao bilo koji dijaloški okvir blokiranja tijekom operacije otvaranja datoteke

- **CachedInfoAvailable** – Booleova vrijednost za traženje predmemoriranih informacija koje su specifične za otvaranje datoteke

- **DocumentRecoveryInvoked** – Booleova vrijednost koja označava je li dokument na čekanju za oporavak

- **EndToEndActivationTime** – vrijeme potrebno za prikazivanje datoteke za datoteke otvorene izvan aplikacije

- **EndToEndFileOpenTime** – vrijeme potrebno za prikazivanje datoteke za datoteke otvorene unutar aplikacije

- **FileOpenPhaseDurationInMs** – vrijeme operacije otvaranja datoteke koje koriste specifične faze

- **FileSourceLocation** – vrijednost enumeracije za lokaciju datoteke kao što su Nema, Lokalno, UncOrMappedNetworkDrive, SkyDrive, App, SharePoint, UnknownServer

- **InitalizationReason** – ulazna točka za otvaranje datoteke

- **InitialBootPhaseTime** – vrijeme potrebno tijekom određene faze pokretanja aplikacije

- **IsThisFirstLaunch** – Booleova vrijednost koja označava je li ovo prvo pokretanje aplikacije

- **MinimumLibraryLoadPhaseTime** – vrijeme potrebno tijekom određene faze pokretanja aplikacije

- **MinimumLibraryLoadPhaseTime** – vrijeme potrebno tijekom određene faze pokretanja aplikacije

- **MinimumLibraryLoadPhaseTime** – vrijeme potrebno tijekom određene faze pokretanja aplikacije

- **PostAppInitTimeInMs** – vrijeme potrebno tijekom određene faze pokretanja aplikacije

- **PPTRenderPhase** – vrijeme povezano s određenom fazom u PPT renderiranju

- **PreAppInitTimeInMs** – vrijeme potrebno tijekom određene faze pokretanja aplikacije

- **ProviderApp** – naziv paketa aplikacije iz koje se datoteka otvara

- **TelemetryReason** – slično je vrijednosti InitialisationReason, no to je vrijednost enumeracije s više detalja koje se odnose na ulaznu točku za otvaranje datoteke.

- **UserDialogInterruptionDuringBoot** – Booleova vrijednost koja označava je li postojao bilo koji dijaloški okvir za blokiranje tijekom pokretanja

- **XLRenderPhase** – vrijeme koje se odnosi na specifičnu fazu prikazivanja u programu Excel.

#### <a name="officeandroidappdocsfileoperationends"></a>Office.Android.AppDocsFileOperationEnds

Ključna dokumenta samo za Android (AppDocs) podaci telemetrije za kraj operacija Datoteka/Novo/Spremi kao. Ovo bilježi kodove pogrešaka za neuspjehe tih AppDocs operacija.  Microsoft to koristi za identificiranje kvarova u različitim operacijama datoteka i točnog sloja na kojem se kvar dogodio u programu Word, Excel ili PowerPoint.

Prikupljaju se sljedeća polja:

- **AccessMode** – vrijednost enumeracije za način pristupa datoteci.  Vrijednost: nema, samo za čitanje, samo za čitanje koja se može nadograditi, za čitanje i pisanje

- **BlockingUIShown** – Booleova vrijednost koja označava je li blokiranje korisničkog sučelja bilo prikazano bilo gdje u protoku.

- **ContentUriAuthority** – autoritet URL-a za sadržaj iz SAF-a

- **Correlation** – GUID za ID korelacije koji se odnosi na operaciju

- **DocId** – ID dokumenta koji je generirao AppDocs

- **DocInstanceId** – DocInstanceId ID instance dokumenta koji generira AppDocs koji je obuhvaćen instancom operacije u dokumentu

- **DocIsEnterpriseProtected** – Booleova vrijednost koja označava je li dokument zaštićen.

- **DocUserId** – korisnički ID iz MS sloja za autorizaciju

- **DocUserIdProvider** – enumeracija koja predstavlja davatelja korisničkog ID-a, 0 = Nepoznato, 1 = LiveId, 2 = OrgId, 3 = SSPI, 4 = ADAL

- **DurationInMs** – vrijeme u milisekundama do završetka operacije datoteke

- **EndReason** – vrijednost enumeracije za krajnji razlog.  Vrijednosti: nema, uspjeh, neuspjeh, odustani.

- **ErrorCode** – kôd pogreške za operaciju datoteke

- **Extension** – prva četiri znaka proširenja datoteke koja se otvara.

- **FileSourceLocation** – vrijednost enumeracije lokacije datoteke. Moguće vrijednosti: Nema, Lokalno, UncOrMappedNetworkDrive, SkyDrive, App, SharePoint, Nepoznati poslužitelj

- **FILETIME** – vrijeme događaja

- **FirstBCSClientError_Info** – informacije o kodu pogreške povezane s pretvorbama datoteka

- **HttpStatusCode** – HTTP kôd odgovora za zahtjev web usluge

- **InitalizationReason** – ulazna točka za otvaranje datoteke

- **K2FileIOHresult** – Hresult kôd za kraj operacije otvaranja datoteke

- **LastBCSClientError_TagId** – posljednja pogreška BSC (usluga binarne pretvorbe) klijenta

- **OfficeWebServiceApiStatusFlag** – zastavica statusa za zahtjev web usluge

- **OpEndEventId** – oznaka koja predstavlja mjesto gdje je operacija zapravo završila

- **OpFlags** – zastavice parametra operacije dokumenta koje koristi sloj AppDocs.

- **OpSeqNum** – broj koji predstavlja redoslijed poziva datoteka povezanih sa operacijom datoteke u sloju AppDocs

- **OpType** – enumeracija vrste operacija. Vrijednosti: "None", "CreateDocument", "OpenDocument", "CopyDocument", "CloseDocument", "SaveDocument", "OpenVersion", "CloseVersion"

- **PreFetchState**– enumeracija stanja pretpreuzimanja predložaka za operacije stvaranja nove datoteke.

- **ProviderApp** – naziv paketa aplikacije iz koje se datoteka otvara

- **ScopeInstanceId**– ID opsega instance koji se koristi za pridruživanje podatkovnog konteksta aktivnostima

- **Size** – veličina datoteke

- **State** – vrijednosti enumeracije za stanje datoteke. Vrijednosti: None, Creating, Created, CreateFailed, Opening, Opened, OpenFailed, Copying, Copied, CopyFailed, Closing, Closed, CloseFail

- **TemplateName** – naziv binarnog predloška dokumenta iz usluge predloška, npr. TF10002009.dotx

- **UriScheme** – shema URL-a

#### <a name="officeandroidauthaceerrors"></a>Office. Android. AuthACEErrors

Taj događaj koristi Microsoftov račun (MSA) za određivanje korisnika koji se pokušava prijaviti u aplikaciju te tijekom čega se telemetrija u raspravi pokreće kao dio neuspješnog pokušaja.  

Ovaj događaj omogućuje analizu raspodjele pogrešaka kod prijave na MSA, što pomaže u razumijevanju razloga neuspješne prijave na MSA.

Prikupljaju se sljedeća polja:

- **ExceptionsName** – označava klase iznimki koje se javljaju za vrijeme tijeka prijave na Microsoftov račun.

- **ExceptionsTag** – upućuje na to koje se iznimke prisutne u uniji pojavljuju za tijek prijave na MSA.

- **IDCRLACEEErrorCode** – prikazuje kôd pogreške koji se pojavljuje za vrijeme tijeka prijave na MSA. Različiti kodovi pogrešaka navedeni na %SRCROOT%\identity\coreapi\public\IdentityData.h

- **IDCRLAuthenticationStatusErrorCode** – označava kôdove pogrešaka za nevaljani status rezultata provjere autentičnosti koji dolazi sa Microsoftova računa (MSA).

- **IDCRLUserInteractionMissingError** – upućuje na to je li tijek prijave na Microsoftov račun (MSA) pozvan sa zastavicom showUI kao lažan koji uzrokuje pozitivni rezultat.


#### <a name="officeandroidbcserrors"></a>Office.Android.BCS.Errors

Telemetrija binarnih pogrešaka pretvorbe za ispis i zajedničko korištenje u obliku PDF-a.  Microsoft to upotrebljava za prepoznavanje točaka neuspjeha tijekom BCS pretvorbe u aplikacijama Word, Excel ili PowerPoint.

Prikupljaju se sljedeća polja:

- **DocumentFileSize** – veličina datoteke.

- **FileExtension** – prva četiri znaka proširenja datoteke.

- **IsFileDirty** – Booleova vrijednost koja označava je li u datoteci bilo nespremljenih promjena.

- **Location** – enumeracija lokacije datoteke.  Vrijednosti: OneDrive, SharePoint, Dropbox, itd.

- **PDFConversionError** – Oznaka pri kojoj dolazi do pogreške za pretvorbu PDF-a

- **PdfConversionErrorCode** – kôd pogreške za pretvorbu PDF dokumenata

- **PdfConversionHRStatus** – kôd statusa pretvorbe PDF-a

- **PdfConversionResult** – enumeracija rezultata PDF pretvorbe.  Vrijednosti: „Success"; „Failed" i „Canceled"

- **PdfFileSize** – veličina PDF-a

#### <a name="officeandroidclientsideiap"></a>Office.Android.ClientSideIAP

Telemetrija ključne pogreške za pogreške u bazi podataka tijekom pregledavanja datoteka i dodavanje mjesta.  Microsoft to upotrebljava za prepoznavanje problema s oštećenjem DB-a u aplikacijama koje mogu ometati korisnika da dodaje mjesta ili ih pregledava unutar aplikacije u aplikacijama Word, Excel ili PowerPoint.

Prikupljaju se sljedeća polja:

- **ClientTransactionId**– GUID proslijeđen DSC-u za specifičan zahtjev aktivacije.

- **CollectionTime** – vrijeme dovršetka kupnje pretplate

- **CountryCode** – kôd države klijenta koji se šalje DSC-u za zahtjev klijenta za aktivaciju

- **GoPremiumEntryPoint** – ulazna točka za pokretanje kupnje 

- **IsActivateExistingSubscription** – Booleova vrijednost upućuje na to je li postojala pretplata koja je aktivirana

- **IsErrorRetriable** – Booleova vrijednost upućuje na to može li se ponoviti aktivacija

- **IsPreviousPurchase** – Booleova vrijednost da naznači je li se aktiviranje dogodilo s prethodnom kupnjom pretplate

- **IsProvisioningTriggeredByRetry** – Booleova vrijednost upućuje na to je li uključen ponovni pokušaj

- **LanguageCode** – kôd jezika klijenta koji se šalje DSC-u za zahtjev klijenta za aktivaciju

- **ProductIdentifier** – naziv SKU-a koji klijent pokušava kupiti

- **ProvisioningHttpStatusCode** – dodjeljivanje http statusnog koda

- **ProvisioningStatusCode** – dodjeljivanje statusnog koda

- **PurchaseOrderId** – identifikator narudžbenice iz Google/Samsung trgovine

- **RedemptionTaskHR** – HResult za zadatak aktivacije pretplate

- **SubscriptionProvisioningSucceeded** – Booleova vrijednost za uspješan rezultat dodjele pretplate

- **SubscriptionPurchaseHR** – Hresult za zadatak kupnje pretplate

- **SubscriptionType** – enumeracija za vrstu pretplate ili SKU-e.

- **TCID** – klik na ikonu aktivira tijek pretplate

#### <a name="officeandroiddbfailurecause"></a>Office.Android.DBFailureCause

Telemetrija ključne pogreške za pogreške u bazi podataka tijekom pregledavanja datoteka i dodavanje mjesta.  Microsoft to upotrebljava za prepoznavanje problema s oštećenjem DB-a u aplikacijama koje mogu ometati korisnika da dodaje mjesta ili ih pregledava unutar aplikacije u aplikacijama Word, Excel ili PowerPoint.

Prikupljaju se sljedeća polja:

- **ErrorAt** – Vrijednost oznake: informacije o mjestu na kojem je došlo do pogreške

- **ExceptionErrorMessage** – opširna poruka o pogrešci

#### <a name="officeandroidearlytelemetryexpansionfileserrors"></a>Office.Android.EarlyTelemetry.ExpansionFilesErrors

Ekspanzijske datoteke za komplet datoteka sustava Android (APK) za mobilnu aplikaciju Office jesu dopunske datoteke resursa koje razvojni programeri aplikacija na sustavu Android mogu objaviti zajedno sa svojom aplikacijom. Da bismo svoj mehanizam preuzimanja ekspanzijskih datoteka učinili pouzdanijim, bilježimo razlog pogrešaka koje nastupe bilo tijekom preuzimanja ekspanzijskih datoteka ili čitanja preuzetih ekspanzijskih datoteka.

Prikupljaju se sljedeća polja:

- **Data_ClassName** – tekst koji predstavlja naziv datoteke izvornog koda u kojem je došlo do pogreške.

- **Data_ErrorMessage** – tekst koji predstavlja operaciju koja nije uspjela.

- **Data_ExceptionMessage** – neobavezno tekstno polje koje predstavlja razlog iznimke.

- **Data_ExceptionType** – neobavezno tekstno polje koje predstavlja naziv iznimke izbačene iz izvornog koda.

- **Data_MethodName** – tekst koji predstavlja naziv metode u izvornom kodu u kojem je došlo do pogreške.

#### <a name="officeandroidearlytelemetryextractionerror"></a>Office.Android.EarlyTelemetry.ExtractionError

Da biste smanjili veličinu aplikacija sustava Office i Android, primjenjujemo kompresiju na resurse u konačnom paketu. Za vrijeme izvođenja te resurse prvo izdvojimo prije nego što ih upotrijebimo. Ponekad ima neočekivanih pogrešaka tijekom izdvajanja, što dovodi do rušenja aplikacije. 

Kroz ovaj događaj prikupljamo neke dijagnostičke informacije vezane uz izdvajanje, kao što je naziv resursa koji se izdvaja, put gdje je izdvojen, itd., besplatni raspoloživi prostor na disku itd. Ti se podaci prikupljaju samo kada se pojave pogreške u izdvajanju.

Ove podatke upotrebljavamo kako bismo shvatili uzrok neuspjelih izdvajanja te unaprijedili korisnički doživljaj naših aplikacija.

Prikupljaju se sljedeća polja:

- **Data_ArchiveName** – naziv resursa koji se izdvaja.

- **Data_ArchivePath** – put gdje se resurs privremeno predmemorira.

- **Data_ArchiveSizeKB** – naziv resursa koji se izdvaja.
 
- **Data_ClassName** – naziv datoteke u izvornom kodu gdje je došlo do pogreške.

- **Data_ErrorDetail** – tekst koji opisuje dodatne pojedinosti o uzroku pogreške, kao što je kôd pogreške, itd.

- **Data_ErrorMessage** – tekst koji opisuje vrstu pogreške koja se pojavljuje tijekom izdvajanja.

- **Data_ExtractionDestinationPath** – put gdje će se resurs spremiti nakon izdvajanja.

- **Data_FreeDiskSpaceMB** – količina slobodnog diskovnog prostora dostupnog na uređaju mjerenog u mega bajtovima. 

- **Data_ItemToExtract** – naziv resursa koji se izdvaja.

- **Data_MethodName** – naziv postupka u izvornom kodu gdje je došlo do pogreške.


#### <a name="officeandroidearlytelemetryregistryerrors"></a>Office.Android.EarlyTelemetry.RegistryErrors

Taj događaj bilježi pogreške do kojih je došlo tijekom pristupanja registru sustava Android. Ti nam podaci o događajima omogućuju razumijevanje korisničkih pogrešaka i poboljšavanje značajke registra.

Prikupljaju se sljedeća polja:

- **App** – proces aplikacije koji šalje događaj.

- **AppVersionLong** – verzija aplikacije.

- **Data_StackTrace** – stacktrace pogreške.

#### <a name="officeandroidearlytelemetrysharedlibraryloadersearchandloadlibraryerror"></a>Office.Android.EarlyTelemetry.SharedLibraryLoadersearchAndloadLibraryError 

Taj događaj bilježimo u slučaju da postoje pogreške tijekom učitavanja zajedničkih biblioteka. Moguće su pogreške u učitavanju biblioteke iz dva razloga 1) Instalirani Apk nije kompatibilan s uređajem. 2) biblioteka koju pokušavamo učitati može biti oštećena, zbog pogrešaka pri izdvajanju zbog malog prostora na disku ili male memorije.

Prikupljaju se sljedeća polja:

- **Data_ExceptionMessage** – poruka o iznimci koju je izbacio Android API System.loadlibrary

- **Data_FreeSpaceInMB** – slobodan prostor dostupan na uređaju

- **Data_nickName** – naziv biblioteke koja se nije mogla učitati.

#### <a name="officeandroidintuneintunejavacopyfailedattempts"></a>Office.Android.Intune.IntuneJavaCopyFailedAttempts

Telemetrija ključne pogreške za praćenje pogrešaka za pojedine Intune API-je; Ova telemetrija evidentira se u slučaju pogrešaka za spremanje lokalne kopije Intune zaštićenih dokumenata u oblaku.  Microsoft koristi ove podatke za prepoznavanje pogrešaka tijekom i nakon Intune upisa u aplikaciju, nakon što se prijavi u aplikaciju s poslovnim računom

Prikupljaju se sljedeća polja:

- **Data_FileCreationFailedErrorCode** – kôd pogreške povezan s protokom

#### <a name="officeandroidintuneintunejavaexceptionadaltokenformam"></a>Office.Android.Intune.IntuneJavaExceptionADALTokenForMAM

Telemetrija ključne pogreške za praćenje pogrešaka za pojedine Intune API-je; Ova telemetrija evidentira se u slučaju pogrešaka za dobivanje ADAL tokena za Intune resurse.  Microsoft upotrebljava ove podatke za prepoznavanje pogrešaka tijekom i nakon Intune upisa u aplikaciju, nakon što se prijavi u aplikaciju s poslovnim računom

Prikupljaju se sljedeća polja:

- **Data_ErrorCode** – kôd pogreške povezan s protokom

#### <a name="officeandroidintuneintunejavaexceptionapppolicy"></a>Office.Android.Intune.IntuneJavaExceptionAppPolicy

Telemetrija ključne pogreške za praćenje pogrešaka za pojedine Intune API-je; Ova telemetrija evidentira se u slučaju pogrešaka pri pozivanju Intune API-ja koje se odnose na pravila dohvaćanja identiteta za trenutni proces.  Microsoft koristi ove podatke za prepoznavanje pogrešaka tijekom i nakon Intune upisa u aplikaciju, nakon što se prijavi u aplikaciju s poslovnim računom

Prikupljaju se sljedeća polja:
 
- Nijedno

#### <a name="officeandroidintuneintunejavaexceptionapppolicyforcontext"></a>Office.Android.Intune.IntuneJavaExceptionAppPolicyForContext

Telemetrija ključne pogreške za praćenje pogrešaka za pojedine Intune API-je; Ova telemetrija evidentira se u slučaju pogrešaka pri pozivanju Intune API-ja koje se odnose na pravila dohvaćanja identiteta za trenutnu aktivnost.  Microsoft koristi ove podatke za prepoznavanje pogrešaka tijekom i nakon Intune upisa u aplikaciju, nakon što se prijavi u aplikaciju s poslovnim računom

Prikupljaju se sljedeća polja:
 
- Nijedno

#### <a name="officeandroidintuneintunejavaexceptionauthenticationcallback"></a>Office.Android.Intune.IntuneJavaExceptionAuthenticationCallback

Telemetrija ključne pogreške za praćenje pogrešaka za pojedine Intune API-je; Ova telemetrija evidentira se u slučaju pogrešaka pri pozivanju Intune API-ja koje se odnose na registraciju za povratne pozive za provjeru autentičnosti za upravljane račune.  Microsoft koristi ove podatke za prepoznavanje pogrešaka tijekom i nakon Intune upisa u aplikaciju, nakon što se prijavi u aplikaciju s poslovnim računom

Prikupljaju se sljedeća polja:

- Nijedno

#### <a name="officeandroidintuneintunejavaexceptiongetaccountstatesync"></a>Office.Android.Intune.IntuneJavaExceptionGetAccountStateSync

Telemetrija ključne pogreške za praćenje pogrešaka za pojedine Intune API-je; Ova telemetrija evidentira se u slučaju pogrešaka pri pozivanju Intune API-ja koje se odnose na upravljani račun.  Microsoft koristi ove podatke za prepoznavanje pogrešaka tijekom i nakon Intune upisa u aplikaciju, nakon što se prijavi u aplikaciju s poslovnim računom

Prikupljaju se sljedeća polja:
 
- Nijedno

#### <a name="officeandroidintuneintunejavaexceptiongetissavetolocationallowed"></a>Office.Android.Intune.IntuneJavaExceptionGetIsSaveToLocationAllowed

Telemetrija ključne pogreške za praćenje pogrešaka za pojedine Intune API-je; Ova telemetrija evidentira se u slučaju pogrešaka za dohvaćanje pravila vezanih uz spremanje na lokalno.  Microsoft koristi ove podatke za prepoznavanje pogrešaka tijekom i nakon Intune upisa u aplikaciju, nakon što se prijavi u aplikaciju s poslovnim računom

Prikupljaju se sljedeća polja:

- Nijedno

#### <a name="officeandroidintuneintunejavaexceptiongetpolicyforidentity"></a>Office.Android.Intune.IntuneJavaExceptionGetPolicyForIdentity

Telemetrija ključne pogreške za praćenje pogrešaka za pojedine Intune API-je; Ova telemetrija evidentira se u slučaju pogrešaka pri pozivanju Intune API-ja koje se odnose na pravila dohvaćanja identiteta.  Microsoft koristi ove podatke za prepoznavanje pogrešaka tijekom i nakon Intune upisa u aplikaciju, nakon što se prijavi u aplikaciju s poslovnim računom

Prikupljaju se sljedeća polja:

- Nijedno

#### <a name="officeandroidintuneintunejavaexceptiongetprotectioninfofromdescriptor"></a>Office.Android.Intune.IntuneJavaExceptionGetProtectionInfoFromDescriptor

Telemetrija ključne pogreške za praćenje pogrešaka za pojedine Intune API-je; Ova telemetrija evidentira se u slučaju pogrešaka pri pozivanju Intune API-ja koje se odnose na podatke o zaštiti.  Microsoft koristi ove podatke za prepoznavanje pogrešaka tijekom i nakon Intune upisa u aplikaciju, nakon što se prijavi u aplikaciju s poslovnim računom

Prikupljaju se sljedeća polja:
  
- Nijedno

#### <a name="officeandroidintuneintunejavaexceptiongetprotectioninfofrompath"></a>Office.Android.Intune.IntuneJavaExceptionGetProtectionInfoFromPath

Telemetrija ključne pogreške za praćenje pogrešaka za pojedine Intune API-je; Ova telemetrija evidentira se u slučaju pogrešaka pri pozivanju Intune API-ja koje se odnose na podatke o zaštiti.  Microsoft koristi ove podatke za prepoznavanje pogrešaka tijekom i nakon Intune upisa u aplikaciju, nakon što se prijavi u aplikaciju s poslovnim računom

Prikupljaju se sljedeća polja:

- Nijedno

#### <a name="officeandroidintuneintunejavaexceptiongetuipolicyidentity"></a>Office.Android.Intune.IntuneJavaExceptionGetUIPolicyIdentity

Telemetrija ključne pogreške za praćenje pogrešaka za pojedine Intune API-je; Ova telemetrija evidentira se u slučaju pogrešaka pri pozivanju Intune API-ja koje se odnose na dohvaćanje pravila korisničkog sučelja za upravljani račun.  Microsoft koristi ove podatke za prepoznavanje pogrešaka tijekom i nakon Intune upisa u aplikaciju, nakon što se prijavi u aplikaciju s poslovnim računom

Prikupljaju se sljedeća polja:

- Nijedno

#### <a name="officeandroidintuneintunejavaexceptionisidentitymanaged"></a>Office.Android.Intune.IntuneJavaExceptionIsIdentityManaged

Telemetrija ključne pogreške za praćenje pogrešaka za pojedine Intune API-je; Ova telemetrija evidentira se u slučaju pogrešaka pri pozivanju Intune API-ja koje se odnose na identificiranje upravlja li se računom.  Microsoft koristi ove podatke za prepoznavanje pogrešaka tijekom i nakon Intune upisa u aplikaciju, nakon što se prijavi u aplikaciju s poslovnim računom.

Prikupljaju se sljedeća polja:

- Nijedno

#### <a name="officeandroidintuneintunejavaexceptionnullenrollmentmanager"></a>Office.Android.Intune.IntuneJavaExceptionNullEnrollmentManager

Telemetrija ključne pogreške za praćenje pogrešaka za pojedine Intune API-je; Ova telemetrija evidentira se u slučaju pogrešaka pri pozivanju Intune API-ja koje se odnose na registraciju komponenti za povratni poziv.  Microsoft koristi ove podatke za prepoznavanje pogrešaka tijekom i nakon Intune upisa u aplikaciju, nakon što se prijavi u aplikaciju s poslovnim računom

Prikupljaju se sljedeća polja:

- Nijedno

#### <a name="officeandroidintuneintunejavaexceptionprotect"></a>Office.Android.Intune.IntuneJavaExceptionProtect

Telemetrija ključne pogreške za praćenje pogrešaka za pojedine Intune API-je; Ova telemetrija evidentira se u slučaju pogrešaka pri pozivanju Intune API-ja koje se odnose na zaštitu upravljanog dokumenta.  Microsoft koristi ove podatke za prepoznavanje pogrešaka tijekom i nakon Intune upisa u aplikaciju, nakon što se prijavi u aplikaciju s poslovnim računom.

Prikupljaju se sljedeća polja:

- Nijedno

#### <a name="officeandroidintuneintunejavaexceptionprotectfromdescriptorifrequired"></a>Office.Android.Intune.IntuneJavaExceptionProtectFromDescriptorIfRequired

Telemetrija ključne pogreške za praćenje pogrešaka za pojedine Intune API-je; Ova telemetrija evidentira se u slučaju pogrešaka pri pozivanju Intune API-ja koje se odnose na zaštitu upravljanog dokumenta.  Microsoft koristi ove podatke za prepoznavanje pogrešaka tijekom i nakon Intune upisa u aplikaciju, nakon što se prijavi u aplikaciju s poslovnim računom

Prikupljaju se sljedeća polja:

- Nijedno

#### <a name="officeandroidintuneintunejavaexceptionregisteraccountsync"></a>Office.Android.Intune.IntuneJavaExceptionRegisterAccountSync

Telemetrija ključne pogreške za praćenje pogrešaka za pojedine Intune API-je; Ova telemetrija evidentira se u slučaju pogrešaka pri pozivanju Intune API-ja koje se odnose na registraciju računa Intune Management.  Microsoft koristi ove podatke za prepoznavanje pogrešaka tijekom i nakon Intune upisa u aplikaciju, nakon što se prijavi u aplikaciju s poslovnim računom

Prikupljaju se sljedeća polja:

- Nijedno

#### <a name="officeandroidintuneintunejavaexceptionsetuipolicyidentitysync"></a>Office.Android.Intune.IntuneJavaExceptionSetUIPolicyIdentitySync

Telemetrija ključne pogreške za praćenje pogrešaka za pojedine Intune API-je; Ova telemetrija evidentira se u slučaju pogrešaka pri pozivanju Intune API-ja koje se odnose na postavljanje pravila za upravljani račun.  Microsoft koristi ove podatke za prepoznavanje pogrešaka tijekom i nakon Intune upisa u aplikaciju, nakon što se prijavi u aplikaciju s poslovnim računom

Prikupljaju se sljedeća polja:

- Nijedno

#### <a name="officeandroidintuneintunejavaexceptionunregisteraccountsync"></a>Office.Android.Intune.IntuneJavaExceptionUnregisterAccountSync

Telemetrija ključne pogreške za praćenje pogrešaka za pojedine Intune API-je; Ova telemetrija evidentira se u slučaju pogrešaka pri pozivanju Intune API-ja koje se odnose na scenarije daljinskog brisanja za Intune Management.  Microsoft koristi ove podatke za prepoznavanje pogrešaka tijekom i nakon Intune upisa u aplikaciju, nakon što se prijavi u aplikaciju s poslovnim računom

Prikupljaju se sljedeća polja:

- Nijedno

#### <a name="officeandroidintuneintunejavaexceptionupdatetoken"></a>Office.Android.Intune.IntuneJavaExceptionUpdateToken

Telemetrija ključne pogreške za praćenje pogrešaka za pojedine Intune API-je; Ova telemetrija evidentira se u slučaju pogrešaka pri pozivanju Intune API-ja koje se odnose na ažuriranje tokena autorizacije za upravljani račun.  Microsoft koristi ove podatke za prepoznavanje pogrešaka tijekom i nakon Intune upisa u aplikaciju, nakon što se prijavi u aplikaciju s poslovnim računom

Prikupljaju se sljedeća polja:

- Nijedno

#### <a name="officeandroidlicenseactivationfailure"></a>Office.Android.LicenseActivationFailure

Telemetrija kritične pogreške za praćenje neuspjeha u aktiviranju licenci za račune sustava Office 365 u aplikacijama Word, Excel ili PowerPoint.  Microsoft to upotrebljava za analiziranje neuspjeha pri aktiviranju kupljene licence Office 365.

Prikupljaju se sljedeća polja:

- **EntryPoint** – enumeracija ulazne točke za pokretanje tijeka aktivacije licence

- **HResult** – kôd pogreške za neuspjeh

- **IsGallatin** – Booleova vrijednost da provjerite je li to Gallatin račun

- **MessageCode** – enumeracija za označavanje mjesta neuspjeha za aktiviranje

- **PreviousEntryPoint** – enumeracija ulazne točke za pokretanje tijeka aktivacije licence

- **StateAfterActivation** – enumeracija koja upućuje na stanje licenciranja aplikacije prije nego što je započeo tijek aktivacije

- **StateBeforeActivation** – enumeracija koja upućuje na stanje licenciranja aplikacije prije nego što je započeo tijek aktivacije

- **UserAccountType** – enumeracija koja upućuje na to je li u pitanju osobni račun ili račun velike tvrtke.

#### <a name="officeandroidmsasigninuiprompts"></a>Office.Android.MSASignInUIPrompts

Tim se događajem označava da je upit za prijavu stigao korisniku, za osobni račun.  Ovaj događaj pomaže u razumijevanju stanja prijava u našim aplikacijama i poduzima odgovarajuće radnje kada uočimo neočekivane ponovne upite za prijavu. 

Prikupljaju se sljedeća polja:

- **ExternalCacheRefreshError** – kôd pogreške pokušaja osvježavanja tokena prije prikazivanja upita za prijavu.

- **LastLoginDelta** – delta vremena od posljednje uspješne prijave.

- **MSAserverUAID** – ID korelacije s telemetrijskim podacima usluge.

- **PreviousIdentityState** – označava stanje računa, poput isteka sesije. 

- **SignInResultCode** – označava kôd rezultata za kraj upita za prijavu.

- **UseCache** – označava smo li prisilno zatražili korisniku da ponovno unese lozinku.

- **UserType** – upućuje na to je li riječ o postojećem računu ili novom računu

- **WasIdentitySignedOut** – upućuje na to je li račun bio u odjavljenom stanju.


#### <a name="officeapplelicensingmacdractivationfailures"></a>Office.Apple.Licensing.Mac.DRActivationFailures

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za snimanje neuspjeha aktivacije tvrtke Digital River (događaj bilježi ključ i proizvod koji su korišteni za aktiviranje, i primljeni kôd pogreške).  Ovaj se događaj koristi za prepoznavanje i pomoć pri otklanjanju poteškoća pri neuspjelim aktivacijama (problemi tvrtke Digital River)

Prikupljaju se sljedeća polja:

- **Data_DigitalRiverID** – ID proizvoda tvrtke Digital River koji se preslikava na proizvod sustava Office – SKY

- **Data_Error** – niz koji predstavlja kôd pogreške aktivacije.

- **Data_ProductKey** – Ključ proizvoda koji je pokušao biti aktiviran

- **Data_ProductKeyHash** – aktiviran je kodirani ključ proizvoda

#### <a name="officeapplelicensingmacgetmachinestatuserrors"></a>Office.Apple.Licensing.Mac.GetMachineStatusErrors

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj prikuplja kôd pogreške vraćen tijekom povremene provjere valjanosti licence pretplate. Kôd pogreške može značiti nedostupnost poslužitelja, ali i isteka licence, ograničenje broja računala, nevažeći ID hardvera itd. Ovaj se događaj koristi za nadziranje stanja servisa za licenciranje sustava Office, ali i za istraživanje problema povezanih s upravljanjem računalima s pretplatom.

Prikupljaju se sljedeća polja:

- **Data_Error** – prikupljamo niz koji predstavlja kôd pogreške.

#### <a name="officeextensibilitysandboxodperrornotification"></a>Office.Extensibility.Sandbox.ODPErrorNotification

Prati različite obavijesti o pogreškama dobivene iz testnog okruženja. Koristi se za prepoznavanje scenarija pogrešaka u testnom okruženju i njihovo popravljanje za poboljšanje korisnikove produktivnosti
 
Prikupljaju se sljedeća polja:

- **AppId** – ID aplikacije

- **AppUrl** – pročišćeni URL aplikacije 

- **Result** – kod pogreške rezultata

#### <a name="officefirstrunapplemaconiolkfirstrunstarted"></a>Office.FirstRun.Apple.MacONIOLKFirstRunStarted

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj nam daje do znanja da je korisnik ušao u iskustvo prvog pokretanja. Ovaj događaj koristimo kako bismo saznali je li iskustvo prvog pokretanja (FRE) uspješno pokrenuto.

Prikupljaju se sljedeća polja:

- **Data_FirstRunCollectionTime** – vremenska oznaka koja bilježi vrijeme pokretanja protoka.

#### <a name="officegraphicsarcexceptions"></a>Office.Graphics.ARCExceptions 

Ta informacija za izvješćivanje o iznimkama važna je za procjenu ukupnog stanja grafičkog stoga i identifikaciju dijelova koda u kojima često dolazi do neuspjeha kako bi se odredili prioriteti istrage. Ta informacija za izvješćivanje o iznimkama važna je za procjenu ukupnog stanja grafičkog stoga i identifikaciju dijelova koda u kojima često dolazi do neuspjeha. To inženjeru pomaže utvrditi koji neuspjesi pri vizualizaciji zahvaćaju najveći broj korisnika te nam omogućuje odrediti prioritete istrage da bismo riješili one probleme od kojih će korisnici imati najviše koristi.

Prikupljaju se sljedeća polja:

  - **Data\_HResult** – kod pogreške koji je neuspjeh vratio

  - **Data\_TagCount** – broj svih neuspjeha do kojih je došlo

  - **Data\_TagID** – identifikator neuspjeha do kojeg je došlo

#### <a name="officeoutlookdesktopcalendaracceptcalsharenavigatetosharedfoldererror"></a>Office.Outlook.Desktop.Calendar.AcceptCalShareNavigateToSharedFolder.Error

Prikuplja informacije kada dođe do bilo kakvog neuspjeha tijekom navigacije u zajedničkom kalendaru. Ti se podaci koriste za nadgledanje ispravnosti API-ja za dijeljenje kalendara i interakcije s izgledima s dijeljenim kalendarima.

Prikupljaju se sljedeća polja:

  - **FailedCaseHResult** – kod pogreške koji je neuspjeh vratio

#### <a name="officeoutlookdesktopedpedpopenstorefailure"></a>Office.Outlook.Desktop.EDP.EDPOpenStoreFailure

Uspješnost ili neuspješnost otvaranja spremišta pošte zaštićenog zaštitom korporativnih podataka na temelju rezultata poziva API-ju za Windows radi pribavljanja ključa za dešifriranje spremišta. Tu dijagnozu koristimo za jedan od najvećih problema sa zaštitom korporativnih podataka, koji može spriječiti pokretanje programa Outlook. Primarni uzrok pogreške je interakcija programa Outlook s Windows API-jima koji se koriste za dešifriranje ključa spremišta.

Prikupljaju se sljedeća polja:

  - **HVA Activity** **-** s prilagođenim podatkovnim poljima

  - **IsFlightOn** – označava je li omogućena testna verzija koja podržava EDPDecryption

#### <a name="officeoutlookdesktopndbcorruptionresult"></a>Office.Outlook.Desktop.NdbCorruptionResult

Office.Outlook.Desktop.NdbCorruptionResult i Office.Outlook.Desktop.NDBCorruptStore.Warning prikupljaju se kada otkrijemo oštećenje u korisnikovoj PST/OST datoteci. Kada prepoznamo oštećenje, Microsoft prikuplja oblik baze podataka, mjesto na kojem ga je otkrio i malu količinu konteksta oštećenja. Oštećenje OST-a/PST-a korisnicima onemogućuje pristup njihovoj e-pošti. Aktivno nadziremo ima li u tim podacima neuobičajenih aktivnosti. Nastojimo istražiti i dijagnosticirati probleme da bismo ograničili gubitak korisničkih podataka.

Prikupljaju se sljedeća polja:

  - **0 –** naziv procesa koji je prijavio oštećenje

  - **1 –** Booleova vrijednost koja označava je li korisnik odabrao novu datoteku

  - **2 –** broj drugih procesa koji su otvorili bazu podataka

#### <a name="officeoutlookdesktopndbcorruptstorewarning"></a>Office.Outlook.Desktop.NDBCorruptStore.Warning

Office.Outlook.Desktop.NdbCorruptionResult i Office.Outlook.Desktop.NDBCorruptStore.Warning prikupljaju se kada otkrijemo oštećenje u korisnikovoj PST/OST datoteci. Kada prepoznamo oštećenje, Microsoft prikuplja oblik baze podataka, mjesto na kojem ga je otkrio i malu količinu konteksta oštećenja. Oštećenje OST-a/PST-a korisnicima onemogućuje pristup njihovoj e-pošti. Aktivno nadziremo ima li u tim podacima neuobičajenih aktivnosti. Nastojimo istražiti i dijagnosticirati probleme da bismo ograničili gubitak korisničkih podataka.

Prikupljaju se sljedeća polja:

  - **CollectionTime** – vrijeme prikupljanja

  - **Context** – kontekst oštećenog spremišta, gdje je oštećenje otkriveno

  - **CreatedWithVersion** – (neobavezno) polje s verzijom spremišta

  - **Details** – pojedinosti o rušenju

  - **NdbType** – vrsta spremišta, može biti 0 = NdbUndefined, 1 = NdbSmall, 2 = NdbLarge, 3 = NdbTardis

  - **ProcessName** – naziv procesa koji je uzrokovao oštećenje spremišta

  - **PstVersion** – verzija datoteke MSPST32.DLL

  - **Version** – verzija oblika datoteke spremišta

#### <a name="officeoutlookdesktopoutlookcalendarusageerrmeetrcptforwardactionsruleo16"></a>Office.Outlook.Desktop.OutlookCalendarUsageErr.MeetRcpt.ForwardActions.Rule.O16

Prikuplja podatke o uspjehu i neuspjehu akcija Proslijedi, Proslijedi kao privitak i Proslijedi kao iCalendar za jednokratne, ponavljajuće i iznimne odgovore na sastanke u prikazima Pošta, Kalendar i Provjera u programu Outlook. Aktivno se prati ima li neobičnosti u stopi neuspjeha akcija Proslijedi, Proslijedi kao privitak i Proslijedi kao iCalendar. Statistički podaci koji sadrže neobičnosti ukazuju na nesposobnost programa Outlook da izvrši osnovne operacije s kalendarima. Ovi se podaci također koriste za dijagnosticiranje drugih problema povezanih s kalendarom koji se mogu otkriti.

Prikupljaju se sljedeća polja:

  - **CountExceptionForward** – broj iznimaka vezanih uz proslijeđene sastanke

  - **CountExceptionForwardAsiCal** – broj iznimaka vezanih uz sastanke proslijeđene kao iCal

  - **CountExceptionForwardInSplit** – broj iznimaka vezanih uz sastanke proslijeđene s podijeljenog izbornika na vrpci

  - **CountExceptionForwardWithAttach** – broj iznimaka vezanih uz sastanke proslijeđene kao privitak

  - **CountRecurringForward** – broj proslijeđenih ponavljajućih sastanaka

  - **CountRecurringForwardAsiCal** – broj ponavljajućih sastanaka proslijeđenih kao iCal

  - **CountRecurringForwardInSplit** – broj ponavljajućih sastanaka proslijeđenih s podijeljenog izbornika na vrpci

  - **CountRecurringForwardWithAttach** – broj ponavljajućih sastanaka proslijeđenih kao privitak

  - **CountSingleForward** – broj proslijeđenih jednokratnih sastanaka

  - **CountSingleForwardAsiCal** – broj jednokratnih sastanaka proslijeđenih kao iCal

  - **CountSingleForwardInSplit** – broj jednokratnih sastanaka proslijeđenih s podijeljenog izbornika na vrpci

  - **CountSingleForwardWithAttach** – broj jednokratnih sastanaka proslijeđenih kao privitak

  - **HResult** – kod pogreške

  - **OlkViewName** – označava prikaz Pošta, Kalendar ili Provjera

#### <a name="officeoutlookdesktopoutlookcalendarusageerrmeetrcptreplyactionsruleo16"></a>Office.Outlook.Desktop.OutlookCalendarUsageErr.MeetRcpt.ReplyActions.Rule.O16

Prikuplja podatke o uspjehu i neuspjehu akcija Odgovori, Odgovori svima, Odgovori izravnom porukom i Odgovori svima izravnom porukom za jednokratne, ponavljajuće i iznimne odgovore na sastanke u prikazima Pošta, Kalendar i Provjera u programu Outlook. Aktivno se prati ima li neobičnosti u stopi neuspjeha akcija Odgovori, Odgovori svima, Odgovori izravnom porukom i Odgovori svima izravnom porukom. Statistički podaci koji sadrže neobičnosti ukazuju na nesposobnost programa Outlook da izvrši osnovne operacije s kalendarima. Ovi se podaci također koriste za dijagnosticiranje drugih problema povezanih s kalendarom koji se mogu otkriti.

Prikupljaju se sljedeća polja:

  - **CountExceptionReply** – broj iznimaka vezanih uz akciju Odgovori u vezi sastanaka

  - **CountExceptionReplyAll** – broj iznimaka vezanih uz akciju Odgovori svima u vezi sastanaka

  - **CountExceptionReplyAllWithIM** – broj iznimaka vezanih uz akciju Odgovori svima izravnom porukom u vezi sastanaka

  - **CountExceptionReplyWithIM** – broj iznimaka vezanih uz akciju Odgovori izravnom porukom u vezi sastanaka

  - **CountRecurringReply** – broj akcija Odgovori u vezi ponavljajućih sastanaka

  - **CountRecurringReplyAll** – broj akcija Odgovori svima u vezi ponavljajućih sastanaka

  - **CountRecurringReplyAllWithIM** – broj akcija Odgovori svima izravnom porukom u vezi ponavljajućih sastanaka

  - **CountRecurringReplyWithIM** – broj akcija Odgovori izravnom porukom u vezi ponavljajućih sastanaka

  - **CountSingleReply** – broj akcija Odgovori u vezi jednokratnih sastanaka

  - **CountSingleReplyAll** – broj akcija Odgovori svima u vezi jednokratnih sastanaka

  - **CountSingleReplyAllWithIM** – broj akcija Odgovori svima izravnom porukom u vezi jednokratnih sastanaka

  - **CountSingleReplyWithIM** – broj akcija Odgovori izravnom porukom u vezi jednokratnih sastanaka

  - **HResult** – kod pogreške

  - **OlkViewName** – označava prikaz Pošta, Kalendar ili Provjera

#### <a name="officeoutlookdesktopoutlookprivsdlgsingleuserloadfail"></a>Office.Outlook.Desktop.OutlookPrivsDlgSingleUser.LoadFail

To pravilo prikuplja pogreške pri zajedničkom korištenju kalendara prilikom dodavanja novog korisnika (vrste EX ili SMTP) iz adresara. Ti se podaci koriste za dijagnosticiranje i rješavanje problema otkrivenih u dijaloškom okviru Zajedničko korištenje kalendara

Prikupljaju se sljedeća polja:

  - **CountAccountWizardEnd** – koliko se puta zatvorio naslijeđeni dijaloški okvir čarobnjaka

  - **CountCreatePIMAccount** – koliko je puta korisnik stvorio PIM profil

#### <a name="officeoutlookmacmacolkasserts"></a>Office.Outlook.Mac.MacOLKAsserts

Koristi se za identificiranje problema u programu Outlook koje utječu na korisnike i koje se mogu manifestirati kao rušenja ili smanjena kvaliteta funkcionalnosti. 

Prikupljaju se sljedeća polja:

- **Category** – vrsta pretpostavke

- **CollectionTime** – vrijeme kada se pretpostavka prikuplja


#### <a name="officeoutlookmacmacolkerrors"></a>Office.Outlook.Mac.MacOLKErrors

Koristi se za identificiranje problema u programu Outlook koje utječu na korisnike i koje se mogu manifestirati kao rušenja ili smanjena kvaliteta funkcionalnosti. 

Prikupljaju se sljedeća polja:

- **Category** – vrsta pogreške

- **CollectionTime** – vrijeme kada se pogreška prikuplja

- **ThreadId** – identifikator za niz


#### <a name="officesystemsystemhealthasserts"></a>Office.System.SystemHealthAsserts

Događaji koje identificira ovaj događaj pomažu nam shvatiti kada je korisnički doživljaj narušen. Mnoge od tih ShipAssert operacija dovode do rušenja, a ovi podaci omogućuju rješavanje mnogih od njih. Prikuplja ShipAsserts iz proizvoda, što pomaže u prepoznavanju pogrešaka.

Prikupljaju se sljedeća polja:

 - **Count** – broj svih prijavljenih pretpostavki

  - **EndTime** – vrijeme kada je načinjena zadnja prijavljena pretpostavka

  - **ErrorGroup** – identifikator grupiranja za svaku pretpostavku

  - **FirstTimeStamp** – prvi put kada je pretpostavka izrečena

  - **Trackback** – jedinstveni identifikator za određenu pretpostavku

#### <a name="officesystemsystemhealtherrorsetwshim"></a>Office.System.SystemHealthErrorsEtwShim

Koristi se za identifikaciju problema u pokrenutoj aplikaciji koji utječu na korisnike te se mogu manifestirati u obliku rušenja ili smanjene funkcionalnosti. Bilježi pogreške do kojih je došlo tijekom izvođenja procesa.

Prikupljaju se sljedeća polja:

  - **EndTime** – vrijeme kada je došlo do zadnje prijavljene pogreške

  - **Trackback** – jedinstveni identifikator određene pogreške

  - **ErrorGroup** – identifikator grupiranja za svaku pogrešku

  - **Count** – broj pojavljivanja svake od pogrešaka

  - **FirstTimeStamp** – prvi put kada je došlo do pogreške

#### <a name="officesystemsystemhealtherrorsulsandasserts"></a>Office.System.SystemHealthErrorsUlsAndAsserts

Koristi se za identifikaciju problema u pokrenutoj aplikaciji koji utječu na korisnike te se mogu manifestirati u obliku rušenja ili smanjene funkcionalnosti. Bilježi pogreške do kojih je došlo tijekom izvođenja procesa.

Prikupljaju se sljedeća polja:

  - **EndTime** – vrijeme kada je došlo do zadnje prijavljene pogreške

  - **Trackback** – jedinstveni identifikator određene pogreške

  - **ErrorGroup** – identifikator grupiranja za svaku pogrešku

  - **Count** – broj pojavljivanja svake od pogrešaka

  - **FirstTimeStamp** – prvi put kada je došlo do pogreške

#### <a name="officesystemsystemhealtherrorsulsworkaround"></a>Office.System.SystemHealthErrorsUlsWorkaround

Koristi se za identifikaciju problema u pokrenutoj aplikaciji koji utječu na korisnike te se mogu manifestirati u obliku rušenja ili smanjene funkcionalnosti. Bilježi pogreške do kojih je došlo tijekom izvođenja procesa

Prikupljaju se sljedeća polja:

  - **EndTime** – vrijeme kada je došlo do zadnje prijavljene pogreške

  - **Trackback** – jedinstveni identifikator određene pogreške

  - **ErrorGroup** – identifikator grupiranja za svaku pogrešku

  - **Count** – broj pojavljivanja svake od pogrešaka

#### <a name="officesystemsystemhealtherrorswithouttag"></a>Office.System.SystemHealthErrorsWithoutTag

Koristi se za identifikaciju problema u pokrenutoj aplikaciji koji utječu na korisnike te se mogu manifestirati u obliku rušenja ili smanjene funkcionalnosti. Bilježi pogreške do kojih je došlo tijekom izvođenja procesa.

Prikupljaju se sljedeća polja:

Count – broj pojavljivanja svake od pogrešaka

  - **EndTime** – vrijeme kada je došlo do zadnje prijavljene pogreške

  - **ErrorCode** – identifikator pogreške

  - **ErrorGroup** – identifikator grupiranja za svaku pogrešku

  - **ErrorId** – identifikator pogreške

  - **FirstTimeStamp** – prvi put kada je došlo do pogreške

  - **Trackback** – jedinstveni identifikator određene pogreške

#### <a name="officesystemsystemhealtherrorswithtag"></a>Office.System.SystemHealthErrorsWithTag

Koristi se za identifikaciju problema u pokrenutoj aplikaciji koji utječu na korisnike te se mogu manifestirati u obliku rušenja ili smanjene funkcionalnosti. Bilježi pogreške do kojih je došlo tijekom izvođenja procesa.

Prikupljaju se sljedeća polja:

  - **Count** – broj pojavljivanja svake od pogrešaka

  - **EndTime** – vrijeme kada je došlo do zadnje prijavljene pogreške

  - **ErrorCode** – identifikator pogreške

  - **ErrorGroup** – identifikator grupiranja za svaku pogrešku

  - **ErrorId** – identifikator pogreške

  - **FirstTimeStamp** – prvi put kada je došlo do pogreške

  - **Trackback** – jedinstveni identifikator određene pogreške

#### <a name="renewidentityfailure"></a>RenewIdentityFailure

Prikuplja se kada korisnik pokuša otvoriti dokument zaštićen IRM-om ili primijeniti zaštite IRM-a. Sadrži informacije potrebne za pravilno istraživanje i dijagnosticiranje problema do kojih dolazi kada obnavljanje korisničkih certifikata nije bilo uspješno.

Prikupljaju se sljedeća polja:

- **AppInfo.ClientHierarchy** – hijerarhija klijenata koja označava da aplikacija radi u proizvodnom okruženju ili okruženju za razvojne inženjere

- **AppInfo.Name** – naziv aplikacije.

- **AppInfo.Version** – verzija aplikacije

- **Failure.Category** – kategorija pogreške „UnhandledError”

- **Failure.Detail** – detaljne informacije o pogrešci

- **Failure.Id** – identifikacijski broj pogreške

- **Failure.Signature** – potpis pogreške koji je jednak nazivu događaja

- **iKey** – identifikacijski broj poslužitelja pružatelja usluge zapisivanja

- **RMS.HRESULT** – rezultat obnavljanja korisničkog certifikata

- **RMS.ScenarioId** – identifikacijski broj scenarija koji definira klijent usluge upravljanja pravima

- **RMS.SDKVersion** – verzija klijenta usluge upravljanja pravima

#### <a name="saveerror"></a>save.error

Omogućuje nam otkrivanje i rješavanje situacija u kojima je došlo do pogreške kada ste pokušali spremiti datoteku.  On prati pogreške uzrokovane neuspješnim spremanjem datoteke, uključujući opisnu poruku o pogrešci kako bi nam pomogao riješiti problem.

Prikupljaju se sljedeća polja: 

- **error** – vrsta pogreške koja je nastupila kako bi nam pomogao otkriti i riješiti probleme u vezi s određenom vrstom pogreške

- **file_type** – vrsta datoteke koju je korisnik pokušao spremiti (primjerice .doc)

- **origin** – odakle pokušaj spremanja potječe (primjerice iz poruke e-pošte) kako bismo mogli prepoznati probleme u vezi sa spremanjem datoteke s određenog mjesta u aplikaciji

- **token_type** – vrsta tokena korištenog za provjeru autentičnosti radi spremanja datoteka koji nam pomaže prepoznati probleme s provjerom autentičnosti u vezi sa spremanjem datoteke

#### <a name="wkwebviewerror"></a>wkwebview.error

Ovaj nam događaj omogućuje utvrđivanje kada su se pogreške s web-prikazom pojavile pri sastavljanju ili čitanju poruke e-pošte kako bismo mogli izbjeći probleme koji bi mogli uzrokovati nemogućnost sastavljanja ili čitanja poruke e-pošte aplikacije. 

Prikupljaju se sljedeća polja: 

- **description** – opis pogreške

- **error_code** – kôd pogreške za WKError

- **function_name** – naziv JavaScript funkcije kada dođe do pogreške

- **js_exception_column_number** – broj stupca u kojemu se pojavila iznimka JavaScripta 

- **js_exception_line_number** – broj retka u kojemu se pojavila iznimka JavaScripta

- **js_exception_message** – poruka o iznimci kada se iznimka JavaScripta pojavila

- **js_exception_source_url** – izvorišni URL u kojemu se iznimka JavaScripta pojavila  

- **scenario** – gdje se pogreška pojavila. To je numeracija. Possible values are old_renderer, react_renderer, and composing.

#### <a name="wkwebviewterminate"></a>wkwebview.terminate

Taj nam događaj omogućuje prepoznavanje kada je sustav prekinuo web-prikaz. Ti nam podaci omogućuju praćenje pogreške koje je korisnik naišao prilikom sastavljanja ili čitanja poruke e-pošte. 

Prikupljaju se sljedeća polja: 

- **is_foreground** – bez obzira na to je li aplikacija u prvom planu kada se događaj dogodi.

- **Scenario** – gdje se pogreška pojavila, prilikom prikazivanja ili sastavljanja.


## <a name="device-connectivity-and-configuration-data-events"></a>Događaji koji se odnose na povezivost i konfiguracijske podatke

Ovo su podvrste podataka u toj kategoriji:

- [Povezivost i konfiguracija uređaja](#device-connectivity-and-configuration-subtype)


### <a name="device-connectivity-and-configuration-subtype"></a>*Podvrsta događaja koji se odnose na povezivost i konfiguraciju uređaja*

Stanje mrežne veze i postavke uređaja, kao što je memorija.

#### <a name="applicationdidreceivememorywarning"></a>application.did.receive.memory.warning

Ovaj se događaj šalje kada nam Apple kaže da aplikaciji ponestaje memorije. On nam govori da smo uveli problem s upravljanjem memorijom na vašem uređaju.

Prikupljaju se sljedeća polja: 

- **current_memory_used** – govori nam količinu memorije koju je aplikacija koristila u trenutku kad je aplikaciji ponestalo memorije.

- **current_memory_used_percentage** – govori nam postotak memorije koju je aplikacija koristila među ukupnom dostupnom memorijom u trenutku kad je aplikaciji ponestalo memorije.

- **currentVC** – govori nam prikaz koji se trenutno prikazuje kad aplikaciji ponestane memorije.

- **has_hx** – govori nam da račun koristi naš novi servis sinkronizacije kako bi nam pomogao prepoznati probleme uzrokovane našim servisom sinkronizacije

- **is_watch_app_installed** – govori nam koristi li korisnik trenutno uređaj Apple Watch te je li on instaliran kako bi nam pomogao razumjeti negativan utjecaj na funkciju zbog uređaja Watch

- **is_watch_paired** – govori nam koristi li korisnik trenutno uređaj Apple Watch te je li on uparen s uređajem kako bi nam pomogao razumjeti negativan utjecaj na funkciju zbog uređaja Watch

- **is_watch_supported_and_active** – govori nam koristi li korisnik trenutno uređaj Apple Watch te je li on aktivan kako bi nam pomogao razumjeti negativan utjecaj na funkciju zbog uređaja Watch

- **rn_initialized** – govori nam je li stavka React Native bila pokrenuta u trenutku kad je aplikaciji ponestalo memorije.

- **running_time** – govori nam količinu vremena koju je aplikacija provela na pokretanje u trenutku kad je aplikaciji ponestalo memorije.

#### <a name="conversationmemoryleak"></a>conversation.memory.leak

Omogućuje nam otkrivanje situacija u kojima naš razgovor poruka e-pošte uzrokuje korištenje više memorije na vašem uređaju od očekivanog.

Prikupljaju se sljedeća polja:

- Ne prikupljaju se nikakva polja ni dodatni podaci. Prikupljaju se samo zapisnici ako postoji curenje memorije u vezi s niti razgovora.

#### <a name="coredatacorruption"></a>core.data.corruption

Omogućuje nam otkrivanje situacija u kojima vam ne možemo prikazati vaše poruke e-pošte ili kalendar jer je mjesto na kojem spremamo e-poštu na vašem uređaju postalo oštećeno.

Prikupljaju se sljedeća polja:

- **errorSource** – označava je li došlo iz radnje spremanja ili kreiranja

- **sqlError** – numerički kod pogreške naveden u https://www.sqlite.org/c3ref/c_abort.html

#### <a name="coredatacorruptionuserreset"></a>core.data.corruption.user.reset

Omogućuje nam prepoznavanje situacija u kojima ste izbrisali ili vratili izvorne postavke svog računa u našoj aplikaciji i kada je to bilo uzrokovano oštećenjem podataka e-pošte koje smo pohranili na vašem uređaju.

Prikupljaju se sljedeća polja:

- **errorSource** – navodi gdje se oštećenje dogodilo, bilo tijekom spremanja ili brisanja

#### <a name="coredatadiagnostics"></a>core.data.diagnostics 

Omogućuje nam otkrivanje i rješavanje situacija u kojima naš prostor za pohranu poruka e-pošte koristi previše prostora za pohranu vašeg uređaja

Prikupljaju se sljedeća polja:

- **db_size_megabytes** – prati veličinu baze podataka osnovnih podataka zaokruženu na najbližih 25 megabajta i s najvećom veličinom od 500 megabajta

#### <a name="generalpropertieslog"></a>general.properties.log

Ovaj događaj prikuplja informacije koje nam omogućuju kategoriziranje i razvrstavanje problema unutar aplikacije Outlook koji su povezani s postavkama pristupačnosti i uređaja.  Ova je kategorizacija potrebna za određivanje prioriteta utjecaja problema na klijente.

Sljedeća se polja prikupljaju samo za iOS:

- **bold_text** – govori nam je li na uređaju uključen podebljan tekst kako bi nam pomogao prepoznati probleme u vezi s podebljanim tekstom

- **closed_captioning** – govori nam je li korisnik uključio titlanje na svojem uređaju kako bi nam pomogao prepoznati probleme u vezi s titlanjem

- **darker_system_colors** – govori nam je li korisnik uključio zatamnjenje boja sustava na svojem uređaju kako bi nam pomogao prepoznati probleme u vezi s tom postavkom

- **gray_scale** – govori nam je li korisnik uključio sive tonove na svojem uređaju kako bi nam pomogao prepoznati probleme u vezi s tom postavkom

- **guided_access** – govori nam je li korisnik uključio vođeni pristup na svojem uređaju kako bi nam pomogao prepoznati probleme u vezi s tom postavkom

- **invert_colors** – govori nam je li korisnik uključio postavku za obrtanje boja na svojem uređaju kako bi nam pomogao prepoznati probleme u vezi s tom postavkom

- **mono_audio** – govori nam je li korisnik uključio postavku za monozvuk na svojem uređaju kako bi nam pomogao prepoznati probleme u vezi s tom postavkom

- **reduce_motion** – govori nam je li korisnik uključio postavku za smanjenje kretnji na svojem uređaju kako bi nam pomogao prepoznati probleme u vezi s tom postavkom

- **reduce_transparency** – govori nam je li korisnik uključio postavku za smanjenje prozirnosti na svojem uređaju kako bi nam pomogao prepoznati probleme u vezi s tom postavkom

- **speak_screen** – govori nam je li korisnik uključio postavku za monozvuk na svojem uređaju kako bi nam pomogao prepoznati probleme u vezi s tom postavkom

- **speak_selection** – govori nam je li korisnik uključio postavku za izgovaranje odabira na svojem uređaju kako bi nam pomogao prepoznati probleme u vezi s tom postavkom

- **switch_control** – govori nam je li korisnik uključio postavku za promjenu kontrola na svojem uređaju kako bi nam pomogao prepoznati probleme u vezi s tom postavkom

- **voice_over** – govori nam je li korisnik uključio postavku za značajku VoiceOver na svojem uređaju kako bi nam pomogao prepoznati probleme u vezi s tom postavkom

Sljedeća se polja prikupljaju samo za Android:

- **braille** – govori nam je li korisnik uključio postavku za obrtanje boja na svojem uređaju kako bi nam pomogao prepoznati probleme u vezi s tom postavkom

- **caption** – govori nam je li korisnik uključio titlanje na svojem uređaju kako bi nam pomogao prepoznati probleme u vezi s titlanjem

- **color_inversion** – govori nam je li korisnik uključio postavku za obrtanje boja na svojem uređaju kako bi nam pomogao prepoznati probleme u vezi s tom postavkom

- **high_contrast** – govori nam je li korisnik uključio postavku za visoki kontrast na svojem uređaju kako bi nam pomogao prepoznati probleme u vezi s tom postavkom

- **large_text** – govori nam je li na uređaju uključen veliki tekstni znak kako bi nam pomogao prepoznati probleme u vezi s tom postavkom

- **oem_preinstall** – govori nam je li naša aplikacija bila unaprijed instalirana na uređaju (to se odnosi samo na uređaje Samsung)

- **supported_abis** – govori nam koju vrsta binarnih sučelja aplikacije (ABI-ova) platforma uređaja podržava kako bi nam pomogao prepoznati probleme u vezi s tom postavkom

- **switch_access** – govori nam je li korisnik uključio postavku za promjenu pristupa na svojem uređaju kako bi nam pomogao prepoznati probleme u vezi s tom postavkom

- **talkback** – govori nam je li korisnik uključio postavku za značajku TalkBack na svojem uređaju kako bi nam pomogao prepoznati probleme u vezi s tom postavkom

- **theme_color** – prilagođena tematska boja (koju je odabrao korisnik) koju aplikacija trenutačno upotrebljava

- **webview_kernel_version**: verzija jezgre sustava Chromium web-prikaza na uređaju koja nam pomaže prepoznati probleme s kompatibilnošću povezane s verzijom web-prikaza.

- **webview_package_name**: naziv paketa web-prikaza na uređaju koji nam pomaže prepoznati probleme s kompatibilnošću povezane s verzijom web-prikaza.

- **webview_package_version**: verzija paketa web-prikaza na uređaju koji nam pomaže prepoznati probleme s kompatibilnošću povezane s verzijom web-prikaza.

#### <a name="lowstoragewarning"></a>low.storage.warning

Ovo je potrebno za nadzor toga zauzima li naša aplikacija iznenada većinu prostora za pohranu na vašem uređaju zbog visoke upotrebe memorije, što upućuje na to da uređaju ponestaje prostor za pohranu

Prikupljaju se sljedeća polja: 

- **free_bytes** – količina slobodnog prostora za pohranu dostupnog na uređaju

#### <a name="officeairspaceairspacelocalblocklistdriverupdated"></a>Office.AirSpace.AirSpaceLocalBlocklistDriverUpdated

Korisnik je ažurirao upravljački program grafičke kartice koji je prije uzrokovao rušenje sustava Office te se zbog toga više ne koristi za vizualizaciju. Obavještava Microsoft da su korisnici koji su jednom bili u neoptimalnom stanju prikazivanja ponovno u preporučenom stanju prikazivanja.

Prikupljaju se sljedeća polja:

  - **Data\_BlockedDriverVersion** – verzija upravljačkog programa koja je na popisu za blokiranje.

  - **Data\_DeviceId** – identifikator uređaja grafičke kartice koji je na popisu za blokiranje.

  - **Data\_UpdatedDriverVersion** – verzija ažuriranog upravljačkog programa

#### <a name="officeairspaceairspacelocalblocklistinfo"></a>Office.AirSpace.AirSpaceLocalBlocklistInfo

Pojedinosti o upravljačkom programu korisnikove grafičke kartice koji je uzrokovao veći broj nedavnih rušenja aplikacija sustava Office. Office neće koristiti tu grafičku karticu u ovoj sesiji sustava Office (umjesto nje koristit će softversku vizualizaciju) dok se upravljački program ne ažurira. Obavještava Microsoft o upravljačkim programima grafičke kartice koji uzrokuju probleme u sustavu Office radi prepoznavanja trendova i analize utjecaja takvih upravljačkih programa na korisnika. Microsoftu govori koliko je korisnika u tom suboptimalnom stanju.

Prikupljaju se sljedeća polja:

  - **Data\_AllAppsBlocked** – jesu li sve aplikacije sustava Office na popisu za blokiranje

  - **Data\_BlockedDeviceId** – identifikator uređaja grafičke kartice koji je na popisu za blokiranje.

  - **Data\_BlockedDriverVersion** – verzija upravljačkog programa koja je na popisu za blokiranje

  - **Data\_CrashHistory** – niz koji predstavlja povijest upravljačkog programa grafičke kartice koji je uzrokovao rušenje, za potrebe analize

  - **Data\_SecsBetweenCrashes** – koliko često dolazi do rušenja upravljačkog programa kartice

#### <a name="officeairspaceairspacewincompisenabled"></a>Office.AirSpace.AirSpaceWinCompIsEnabled

Koristi li se najnovija platforma niske razine za vizualizaciju u sustavu Office, koja se temelji na platformi Windows Composition.

Dok se najnovija platforma niske razine za vizualizaciju u sustavu Office razvija i počinje distribuirati korisnicima, to Microsoftu omogućuje uvid u broj korisnika koji koriste pojedinu verziju kako se na platformi ne bi pojavile programske pogreške.

Prikupljaju se sljedeća polja:

  - **Data\_WinCompEnabled** – koristi li se pozadinski sustav utemeljen na platformi Windows Composition

#### <a name="officeairspacebackendwin32graphicsdriverhangdetectorblocklistapp"></a>Office.AirSpace.Backend.Win32.GraphicsDriverHangDetectorBlocklistApp

Otkriveno je da korisnikova grafička kartica uzrokuje dugačke ili nepopravljive blokade. Office neće koristiti tu grafičku karticu u ovoj sesiji sustava Office (umjesto nje koristit će softversku vizualizaciju) dok se upravljački program ne ažurira. Obavještava Microsoft o upravljačkim programima grafičke kartice koji uzrokuju probleme u sustavu Office radi prepoznavanja trendova i analize utjecaja takvih upravljačkih programa na korisnika. Također, pridonosi informiranju o broju korisnika u tom suboptimalnom stanju.

Prikupljaju se sljedeća polja:

  - **Data\_AppName** – u kojoj je aplikaciji došlo do blokade upravljačkog programa grafičke kartice

#### <a name="officeairspacebackendwin32graphicsdriverhangdetectorregistrywrite"></a>Office.AirSpace.Backend.Win32.GraphicsDriverHangDetectorRegistryWrite

Office je utvrdio da je korisnikov upravljački program grafičke kartice uzrokovao blokadu koju treba analizirati prilikom sljedećeg pokretanja aplikacije sustava Office. Koristi se da bi se utvrdilo bi li korištenje drugog upravljačkog programa ili prilagodnika grafičke kartice nudilo bolji korisnički doživljaj. Kada opazi uzorke, Microsoft će možda provesti određene prilagodbe da bi doživljaj korištenja sustava Office ostao što je moguće ugodniji.

Prikupljaju se sljedeća polja:

  - **Data\_HangDetected** – je li otkrivena blokada

  - **Data\_InDeviceCall** – koji je vizualizacijski poziv Office uputio grafičkoj kartici kada je došlo do blokade

  - **Data\_Timeout** – trajanje blokade ako je došlo do oporavka

  - **Data\_UnrecoverableCommand** – je li obično moguće oporaviti se od blokade u ovoj vizualizacijskoj naredbi.

#### <a name="officeairspacebackendwin32localblocklistactivity"></a>Office.AirSpace.Backend.Win32.LocalBlocklistActivity

Pojedinosti o upravljačkom programu korisnikove grafičke kartice koji je uzrokovao veći broj nedavnih rušenja aplikacija sustava Office. Office neće koristiti tu grafičku karticu u ovoj sesiji sustava Office (umjesto nje koristit će softversku vizualizaciju) dok se upravljački program ne ažurira. Obavještava Microsoft o upravljačkim programima grafičke kartice koji uzrokuju probleme u sustavu Office radi prepoznavanja trendova i analize utjecaja takvih upravljačkih programa na korisnika. Microsoftu govori koliko je korisnika u tom suboptimalnom stanju.

Prikupljaju se sljedeća polja:

  - **Data.AllAppsBlocked** – jesu li sve aplikacije sustava Office na popisu za blokiranje

  - **Data.BlockedDeviceId** – identifikator uređaja grafičke kartice koji je blokiran

  - **Data.BlockedDriverVersion** – verzija upravljačkog programa koja je na popisu za blokiranje

  - **Data.CrashHistory System.String** – niz koji predstavlja povijest upravljačkog programa grafičke kartice koji je uzrokovao rušenje, za potrebe analize

  - **Data.SecsBetweenCrashes** – koliko često dolazi do rušenja upravljačkog programa kartice

#### <a name="officeairspacebackendwin32localblocklistdriverupdatedactivity"></a>Office.AirSpace.Backend.Win32.LocalBlocklistDriverUpdatedActivity

Korisnik je ažurirao upravljački program grafičke kartice koji je prije uzrokovao rušenje sustava Office te se zbog toga više ne koristi za vizualizaciju. Obavještava Microsoft da su korisnici koji su jednom bili u neoptimalnom stanju prikazivanja ponovno u preporučenom stanju prikazivanja.

Prikupljaju se sljedeća polja:

  - **Data\_BlockedDeviceId** – identifikator uređaja grafičke kartice koji je na popisu za blokiranje.

  - **Data\_BlockedDriverVersion** – verzija upravljačkog programa koja je na popisu za blokiranje

  - **Data\_UpdatedDriverVersion** – verzija ažuriranog upravljačkog programa

#### <a name="officegraphicsspritememcorrupt"></a>Office.Graphics.SpriteMemCorrupt

Izvješćuje o svim otkrivenim pogreškama u telemetriji obračuna memorije sprajtova. Ključno za procjenu stanja telemetrije korištenja grafičke memorije. Taj je podatak potreban za provjeru ispravnosti naše telemetrije za SpriteMem.

Prikupljaju se sljedeća polja:

  - **Data\_CurrentSpriteMem** – ukupna količina memorije aktivno dodijeljene čuvanju sprajtova (slika) iz kojih nastaje sadržaj zaslona.

  - **Data\_Function** – naziv funkcije koja pokušava osloboditi memoriju za sprajtove.

  - **Data\_SpriteMemToRemove** – količina memorije koja više neće biti dodijeljena sprajtovima.

#### <a name="officepowerpointpptsharednointernetconnectivity"></a>Office.PowerPoint.PPT.Shared.NoInternetConnectivity

Prikuplja se kad god PowerPoint otkrije da nema internetske veze. Microsoft koristi te podatke da bi prikupio dijagnostičke podatke o korisnikovoj internetskoj vezi i razumio kako to utječe na povezivanje sa servisima sustava Office.

Prikupljaju se sljedeća polja:

- **Data\_IsNexusDetected:bool** – pokazuje jesmo li stanje internetske veze dobili prilikom pozivanja servisa Nexus (vrijednost „istinito”) ili API poziva generičkom web-servisu (vrijednost „neistinito”)

#### <a name="officeserviceabilitymanagerofficesvcmgrprofile"></a>Office.ServiceabilityManager.OfficeSvcMgrProfile

Taj se događaj aktivira kada se pokrene upravitelj uslužnosti sustava Office i presudan je za pružanje točnih uvida u vezi sa statusom implementacije i rušenjem aplikacija i dodataka unutar sustava kupca omogućujući nam generiranje uvida u to da IT administrator može pouzdano uvoditi ažuriranja za njihove poslovne strojeve.  

Prikupljaju se sljedeća polja:

- **DeviceIdJoinToken** – koristi se za spajanje podataka telemetrije iz stanja sustava i stanja implementacije s drugim funkcionalnim podacima koji se prikupljaju putem cjevovoda za usluge.

- **TenantAssociationKeyStamped** – Booleova zastavica koja se koristi za određivanje broja upravljanih uređaja u sustavu Office.
