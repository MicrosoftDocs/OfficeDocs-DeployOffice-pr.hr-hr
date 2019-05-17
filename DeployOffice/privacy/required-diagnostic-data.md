---
title: Obavezni dijagnostički podaci za Office
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.audience: ITPro
ms.topic: reference
ms.service: o365-proplus-itpro
localization_priority: Priority
ms.collection: Ent_O365
ms.custom:
- Ent_Office_ProPlus
- Ent_Office_Privacy
description: Administratorima sustava Office nudi informacije o obaveznim dijagnostičkim podacima u sustavu Office, a sadrži i popis događaja i podatkovnih polja.
hideEdit: true
ms.openlocfilehash: 9b22b428999c51b46e6f6ce662fad99f5a727b4c
ms.sourcegitcommit: 6145cfe372725bedab7bc6a80adab100561f74fd
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/17/2019
ms.locfileid: "34106916"
---
# <a name="required-diagnostic-data-for-office"></a>Obavezni dijagnostički podaci za Office

> [!IMPORTANT]
> Informacije u ovom članku odnose se na verziju 1904 ili noviju verziju sljedećeg klijentskog softvera sustava Office instaliranog na računalu sa sustavom Windows:
> - Office 365 ProPlus i Office 365 Business
> - Office 365 Personal, Office 365 Home ili druge verzije sustava Office koje su dio pretplate na Office 365.
> - Project i Visio koji se isporučuju s nekim pretplatničkim tarifama, kao što su Project Online Professional ili Visio Online Plan 2.

Dijagnostički podaci koriste se da bi Office uvijek bio siguran i ažuran, kao i radi otkrivanja, dijagnosticiranja i rješavanja problema te poboljšavanja proizvoda. Ti podaci ne sadrže korisnikovo ime ili adresu e-pošte, sadržaj korisnikovih datoteka ni informacije o aplikacijama koje nisu povezane sa sustavom Office.

To su dijagnostički podaci o klijentskom softveru sustava Office koji se koristi na računalima sa sustavom Windows, a koji se prikupljaju i šalju Microsoftu. Neki su dijagnostički podaci obavezni, a neki nisu. Omogućujemo vam da odaberete hoćete li nam slati obavezne ili dijagnostičke podatke putem kontrola zaštite privatnosti, kao što su postavke pravilnika za tvrtke i ustanove. Dijagnostičke podatke koji nam se šalju možete pogledati pomoću preglednika dijagnostičkih podataka.

***Obavezni dijagnostički podaci*** minimalni su podaci potrebni da bi Office bio siguran i ažuran te da bi na uređaju na kojem je instaliran funkcionirao na očekivan način.

Obavezni dijagnostički podaci omogućuju da otkrijete probleme sa sustavom Office koji mogu biti povezani s konfiguracijom uređaja ili softvera. Na primjer, pomoću njih možete utvrditi ruši li se značajka sustava Office češće u određenoj verziji operacijskog sustava, zbog tek uvedenih značajki ili kada se onemoguće određene značajke sustava Office. Obavezni dijagnostički podaci omogućuju nam da otkrijemo, dijagnosticiramo i brže riješimo te probleme kako bi se smanjio utjecaj na korisnike ili tvrtke i ustanove.

Dodatne informacije o dijagnostičkim podacima potražite u ovim člancima:

- [Neobavezni dijagnostički podaci za Office](optional-diagnostic-data.md)
- [Korištenje preglednika dijagnostičkih podataka sa sustavom Office](https://support.office.com/article/cf761ce9-d805-4c60-a339-4e07f3182855)

Ako ste administrator za tvrtku ili ustanovu, možda će vas zanimati i sljedeći članci:

- [Pregled kontrola za zaštitu privatnosti za Office 365 ProPlus](overview-privacy-controls.md)
- [Korištenje postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Office 365 ProPlus](manage-privacy-controls.md)

## <a name="categories-data-subtypes-events-and-data-fields-for-required-diagnostic-data"></a>Kategorije, podvrste podataka, događaji i podatkovna polja za obavezne dijagnostičke podatke

Obavezni dijagnostički podaci organizirani su u kategorije i podvrste podataka. U svakoj su podvrsti podataka događaji koji sadrže podatkovna polja specifična tom događaju.

U sljedećoj su tablici navedene kategorije za obavezne dijagnostičke podatke. Navedene su podvrste podataka u svakoj kategoriji i opis fokusa za tu podvrstu podataka. Prikazat će se veze na odgovarajući odjeljak podvrste podataka u kojem ćete naći sljedeće informacije:

- popis događaja u toj podvrsti podataka
- opis svakog događaja
- popis podatkovnih polja u svakom događaju
- opis svakog podatkovnog polja

| **Kategorija**       | **Podvrsta podataka**| **Opis**    |
| ---------- | ------------- | ---- |
| **Instalacija softvera i instalirani softver** | [Instalacija sustava Office i instalirani softver](#office-setup-and-inventory-subtype)   | Instalirani proizvod, njegova verzija i njegov status instalacije.  |
| | [Konfiguracija dodatka za Office](#office-add-in-configuration-subtype)  | Softverski dodaci i njihove postavke.     |
| | [Sigurnost](#security-subtype)  | Uvjeti za pogreške u dokumentima, značajkama i dodacima koji mogu ugroziti sigurnost, uključujući spremnost proizvoda za ažuriranje.  |
| **Korištenje proizvoda i usluga**    | [Uspjeh značajki aplikacije](#application-feature-success-subtype)   | Uspješno funkcioniranje aplikacije. Ograničeno na otvaranje i zatvaranje aplikacije i dokumenata, uređivanje datoteka i zajedničko korištenje dokumenata (suradnju). |
| | [Status i pokretanje aplikacije](#application-status-and-boot-subtype)    | Utvrđivanje je li došlo do određenih događaja povezanih sa značajkama, kao što je pokretanje ili zaustavljanje, te utvrđivanje je li značajka pokrenuta.   |
| | [Konfiguracija pristupačnosti za Office](#office-accessibility-configuration-subtype)  | Značajke pristupačnosti u sustavu Office       |
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

  - **UserCategory ―** određuje vrstu korisnika koji daje pristanak. Jedan MSAUser, AADUser ili LocalDeviceUser

  - **DiagnosticConsentLevel** – označava razinu pristanka za dijagnostičke podatke koju je korisnik dao

  - **DiagnosticConsentSourceLocation** – označava način na koji je korisnik dao pristanak za dijagnostičke podatke

  - **DiagnosticConsentConsentTime** – označava kada je korisnik dao pristanak za dijagnostičke podatke

  - **ServiceConnectionState** – označava je li korisnik odlučio koristiti ili ne koristiti sva povezana iskustva

  - **ServiceConnectionStateSourceLocation** – označava način na koji je korisnik odlučio želi li koristiti sva povezana iskustva

  - **ServiceConnectionStateConsentTime** – označava kada je korisnik odlučio želi li koristiti sva povezana iskustva

  - **ControllerConnectedServicesState** – označava ima li korisnik pristup neobaveznim povezanim iskustvima

  - **ControllerConnectedServicesStateSourceLocation** – označava kako je napravljen korisnikov odabir za neobavezna povezana iskustva

  - **ControllerConnectedServicesStateConsentTime** – označava kada je korisnik odabrao status neobaveznih povezanih iskustava

  - **UserContentDependentState** – označava je li korisnik odlučio omogućiti ili onemogućiti povezana iskustva koja analiziraju sadržaj

  - **UserContentDependentStateSourceLocation** – označava kako je napravljen korisnikov odabir omogućivanja ili onemogućivanja povezanih iskustava koja analiziraju sadržaj

  - **UserContentDependentStateConsentTime** – označava kada je korisnik odlučio omogućiti ili onemogućiti povezana iskustva koja analiziraju sadržaj

  - **DownloadContentState** – označava je li korisnik odlučio omogućiti ili onemogućiti povezana iskustva koja preuzimaju internetski sadržaj

  - **DownloadContentStateSourceLocation** – označava kako je korisnik napravio odabir omogućivanja ili onemogućivanja povezanih iskustava koja preuzimaju internetski sadržaj

  - **DownloadContentStateConsentTime** – označava kada je korisnik napravio odabir omogućivanja ili onemogućivanja povezanih iskustava koja preuzimaju internetski sadržaj.

#### <a name="device"></a>Uređaj 

Informacije o operacijskom sustavu i međuverziji.

Ova kategorija sadrži sljedeća polja:

  - **OsBuild** – broj međuverzije operacijskog sustava instaliranog na uređaju. Omogućuje da utvrdimo utječu li problemi na pojedinačne servisne pakete ili verzije određenog operacijskog sustava drugačije od drugih kako bismo mogli odrediti prioritete problema.

  - **OsVersion** – glavna verzija operacijskog sustava instaliranog na uređaju. Omogućuje da utvrdimo utječu li problemi na određenu verziju operacijskog sustava više od drugih kako bismo mogli odrediti prioritete problema.

#### <a name="legacy"></a>Starije verzije 

Pruža Id aplikacije i verziju OS-a zbog kompatibilnosti s postojećim praksama prikupljanja za starije verzije.

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

  - **ID** – jedinstveno označava određenu sesiju podataka. Omogućuje utvrđivanje utjecaja problema procjenom broja zahvaćenih sesija te postoje li zajedničke značajke tih sesija.

  - **ImpressionId** – označava skup međuverzija koje se izvode u određenoj sesiji. Omogućuje prepoznavanje pojedinačnih međuverzija koje se izvode u sesiji kako bismo utvrdili je li međuverzija izvor problema koji utječe na korisnike.

  - **MeasuresEnabled** – zastavica koja označava jesu li podaci trenutne sesije uzorkovani. Omogućuje da utvrdimo kako statistički procijeniti podatke prikupljene iz određene sesije.

  - **SamplingClientId** – ID klijenta kojim se utvrđuje je li dio uzorkovanja. Omogućuje da utvrdimo zašto je pojedinačna sesija uključena ili isključena iz uzorkovanja.

#### <a name="user"></a>Korisnik

Pruža informacije o klijentu za SKU-ove komercijalnog softvera.

Ova kategorija sadrži sljedeća polja:

  - **PrimaryIdentityHash** – identifikator u obliku pseudonima koji predstavlja trenutnog korisnika.

  - **PrimaryIdentitySpace** – vrsta identiteta sadržana u identifikatoru PrimaryIdentityHash. MASCID, OrgIdCID ili UserObjectId.

  - **TenantGroup** – vrsta klijenta kojem pripada pretplata. Omogućuje klasifikaciju problema i utvrđivanje je li problem rasprostranjen ili ograničen na skup korisnika.

  - **TenantId** – klijent s kojim je povezana pretplata. Omogućuje klasifikaciju problema i utvrđivanje je li problem rasprostranjen ili ograničen na skup korisnika ili određenog klijenta.

### <a name="information-that-specifically-supports-diagnostic-data-collection"></a>*Informacije koje izričito podržavaju prikupljanje dijagnostičkih podataka*

Informacije koje izričito podržavaju prikupljanje dijagnostičkih podataka prikupljaju se u sljedećim kategorijama.

#### <a name="activity"></a>Aktivnost

Informacije za shvaćanje uspješnosti samog događaja prikupljanja.

Ova kategorija sadrži sljedeća polja:

  - **AggMode** – govori sustavu kako prikupiti rezultate aktivnosti. Omogućuje da smanjimo količinu podataka prenesenih s korisnikovog računala prikupljanjem rezultata aktivnosti u jedan događaj koji se šalje povremeno.

  - **Count** – broj izvršavanja aktivnosti ako je broj iz skupnog događaja. Omogućuje da odredimo koliko je često aktivnost uspjela na temelju načina prikupljanja aktivnosti.

  - **CV** – vrijednost koja određuje odnos između aktivnosti i segmenata aktivnosti. Omogućuje ponovno stvaranje odnosa između ugniježđenih aktivnosti.

  - **Trajanje** – vrijeme potrebno za izvršavanje aktivnosti. Omogućuje prepoznavanje problema s performansama koji negativno utječu na korisničko okruženje.

  - **Rezultat**.** Kod** – kod koji je definirala aplikacija za prepoznavanje određenih rezultata. Omogućuje da utvrdimo specifične pojedinosti o određenoj pogrešci, primjerice kod pogreške koji može se koristiti za klasifikaciju i rješavanje problema.

  - **Result.Tag** – oznaka cijelog broja koja označava mjesto u kodu u kojem je generiran rezultat. Omogućuje jasno utvrđivanje mjesta u kodu na kojem je rezultat generiran što omogućuje klasifikaciju pogrešaka.

  - **Rezultat**.**Vrsta** – vrsta koda rezultata. Određuje vrstu poslanog koda rezultata kako bi se vrijednost ispravno tumačila.

  - **Uspjeh** – zastavica koja označava je li aktivnost uspjela. Omogućuje da utvrdimo uspijevaju li radnje koje korisnik izvršava u proizvodu. Time se omogućuje prepoznavanje problema koji utječu na korisnika.

#### <a name="application"></a>Aplikacija 

Informacije o instalaciji aplikacije iz koje se prikupljaju događaji.

Ova kategorija sadrži sljedeća polja:

  - **Arhitektura** – arhitektura aplikacije. Omogućuje nam da klasificiramo pogreške koje mogu biti specifične za arhitekturu aplikacije.

  - **Click2RunPackageVersion** – broj verzije paketa Klikom do cilja koji je instalirao aplikaciju. Omogućuje da utvrdimo verziju instalacijskog programa korištenu za instalaciju sustava Office kako bismo prepoznali probleme vezane uz postavljanje.

  - **DistributionChannel** – kanal u kojem je aplikacija implementirana. Omogućuje da podijelimo dolazne podatke kako bismo utvrdili utječu li problemi na ciljne skupine.

  - **InstallMethod** – određuje je li sustav nadograđen na trenutnu međuverziju sustava Office sa starije međuverzije, vraćen na nju ili je u pitanju nova instalacija.

  - **IsClickToRunInstall** – zastavica koja označava radi li se o instalaciji „klikom do cilja“. Omogućuje da prepoznamo probleme koji mogu biti specifični za mehanizam instalacije Klikom do cilja.

  - **IsDebug** – zastavica koja označava radi li se o međuverziji sustava Office za ispravljanje pogrešaka. Omogućuje da utvrdimo potječu li problemi iz međuverzija za ispravljanje pogrešaka koje se ponašaju drugačije.

  - **IsInstalledOnExternalStorage** – zastavica koja označava je li Office instaliran na vanjskom uređaju za pohranu. Omogućuje nam da odredimo mogu li se problemi povezati s mjestom za vanjsku pohranu.

  - **IsOEMInstalled** – zastavica koja označava je li Office instalirao proizvođač originalne opreme (OEM). Omogućuje nam da odredimo je li aplikaciju instalirao OEM, što nam može olakšati klasifikaciju i prepoznavanje problema.

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

  - **Naziv** – naziv događaja. Omogućuje prepoznavanje događaja koji šalje klijent.

  - **Pravilo** – identifikator pravila koje je generiralo podatke ako ih je generiralo pravilo. Omogućuje prepoznavanje izvora dijela podataka tako da možemo provjeriti parametre tog događaja i njima upravljati

  - **RuleId** – identifikator pravila koje je generiralo podatke ako ih je generiralo pravilo. Omogućuje prepoznavanje izvora dijela podataka tako da možemo provjeriti parametre tog događaja i njima upravljati.

  - **RuleInterfaces** – sučelja koja određeno pravilo implementira. Omogućuje klasifikaciju i uvoz podataka na temelju njihove strukture što pojednostavnjuje obradu podataka.

  - **RuleVersion** – identifikator pravila koje je generiralo podatke ako ih je generiralo pravilo. Omogućuje prepoznavanje izvora dijela podataka tako da možemo provjeriti parametre tog događaja i njima upravljati.

  - **SampleRate** – oznaka postotka korisnika koji šalju taj dio podataka. Time se omogućuje statistička analiza podataka i veoma česte točke podataka ne zahtijevaju da to šalju svi korisnici.

  - **SchemaVersion** – verzija sheme koja se koristi za generiranje dijagnostičkih podataka. Obavezno za upravljanje podacima koje šalje klijent. Time se omogućuju promjene podataka koje šalje svaki klijent tijekom vremena.

  - **Slijed** – brojač koji navodi redoslijed kojim je događaj generiran na klijentu. Omogućuje numeriranje primljenih podataka kako bismo prepoznali korake koji su doveli do problema koji utječe na klijente.

  - **Izvor** – izvorni kanal upotrijebljen za prijenos podataka. Obavezno za praćenje svih kanala za prijenos radi ukupnog stanja i prepoznavanja problema s kanalom za prijenos. Time se omogućuje praćenje pojedinačnih kanala za prijenos kako bi bili usklađeni.

  - **Vrijeme** – vrijeme generiranja događaja na klijentu. Omogućuje sinkroniziranje i provjeru valjanosti redoslijeda događaja generiranih na klijentu kao i uspostavu parametara za mjerenje performansi za korisničke upute. 

#### <a name="host"></a>Glavno računalo

Informacije o aplikaciji koja hostira ugrađenu aplikaciju

Ova kategorija sadrži sljedeća polja:

  - **Id** – jedinstveni identifikator koji ugrađena aplikacija pripisuje glavnoj aplikaciji.

  - **SessionId** – globalno jedinstveni identifikator za sesiju glavnog računala.

  - **Verzija** – identifikator verzije primarne izvršne datoteke glavnog računala.

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

  - **SamplingKey** – ključ koji određuje je li sesija uzorkovana. Omogućuje da utvrdimo kako pojedine sesije odlučuju hoće li biti uzorkovane.

  - **SamplingMethod** – metoda koja se koristi za utvrđivanje pravila uzorkovanja. Omogućuje da utvrdimo koji podaci dolaze iz sesije.

  - **Slijed** – jedinstveni numerički identifikator za sesiju. Omogućuje određivanje redoslijeda sesija za analizu problema koji su se pojavili.

  - **Pokretanje** – vrijeme pokretanja sesije postupka. Omogućuje da utvrdimo kada je sesija pokrenuta.

  - **TimeZoneBiasInMinutes** – razlika u minutama između UTC-a i lokalnog vremena. Omogućuje normalizaciju UTC-a na lokalno vrijeme.

  - **SamplingClientIdValue** – vrijednost ključa za određivanje uzorkovanja. Omogućuje da utvrdimo zašto je sesija uzorkovana.

  - **SamplingDeviceIdValue** – vrijednost ključa za određivanje uzorkovanja. Omogućuje da utvrdimo zašto je sesija uzorkovana.

  - **SamplingSessionKValue** – napredni metapodaci uzorkovanja. Koristi se za procjenu statističkog značenja primljenih podataka.

  - **SamplingSessionNValue** – napredni metapodaci uzorkovanja. Koristi se za procjenu statističkog značenja primljenih podataka.

  - **TelemetryPermissionLevel** – vrijednost koja označava razinu dijagnostičkih podataka koje je korisnik odabrao. Omogućuje da utvrdimo razinu dijagnostičkih podataka koja se može očekivati od sesije.

## <a name="software-setup-and-inventory-data-events"></a>Događaji koji se odnose na instalaciju softvera i podatke o instaliranom softveru

Ovo su podvrste podataka u toj kategoriji:
- [Instalacija sustava Office i instalirani softver](#office-setup-and-inventory-subtype)
- [Konfiguracija dodatka za Office](#office-add-in-configuration-subtype)
- [Sigurnost](#security-subtype)  

### <a name="office-setup-and-inventory-subtype"></a>*Instalacija sustava Office i podvrsta instaliranog softvera*

Instalirani proizvod, njegova verzija i njegov status instalacije.

#### <a name="officeclicktorunupdatestatus"></a>Office.ClickToRun.UpdateStatus

Odnosi se na sve aplikacije win32. Omogućuje nam da utvrdimo status postupka ažuriranja paketa sustava Office (uspjeh ili neuspjeh s detaljima o pogrešci)

Prikupljaju se sljedeća polja:

- **međuverzija** – trenutno instalirana verzija sustava Office

- **kanal** – kanal putem kojeg je Office distribuiran

- **errorCode** – kod pogreške koji označava pogrešku

- **errorMessage** – dodatne informacije o pogrešci

- **status** – trenutni status ažuriranja

- **targetBuild** – verzija na koju se ažurira Office

#### <a name="officecorrelationmetadatautccorrelationmetadata"></a>Office.CorrelationMetadata.UTCCorrelationMetadata

Prikuplja metapodatke sustava Office putem UTC-a radi usporedbe s odgovarajućim podacima prikupljenim kroz kanal za telemetriju radi provjere ispravnosti i potpunosti podataka.

Prikupljaju se sljedeća polja:

- **abConfigs** – popis ID-ova značajki radi utvrđivanja koje su značajke na klijentu omogućene ili prazna vrijednost kada se ti podaci ne prikupljaju.

- **abFlights** – „NoNL:NoFlights“ kada izdvojene međuverzije nisu postavljene. U suprotnom „holdoutinfo = Nepoznato“.

- **AppSessionGuid** – identifikator određene sesije aplikacije koja počinje od vremena postupka stvaranja i traje do završetka postupka. Oblikovan je kao standardni 128-bitni GUID, ali se sastoji od 4 dijela. Ta četiri dijela redoslijedom su (1) 32-bitni ID procesa (2) 16-bitni ID sesije (3) 16-bitni ID pokretanja (4) 64-bitno vrijeme stvaranja postupka u 100ns UTC-a

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

- **osEnvironment** – cijeli broj koji označava operacijski sustav (Windows, Android, iOS, Mac, itd).

- **osVersionString** – verzija operacijskog sustava

- **sessionID** – nasumično generirani guid za prepoznavanje sesije aplikacije

- **UTCReplace_AppSessionGuid** – konstantna Booleova vrijednost. Uvijek istinito.

#### <a name="officetargetedmessagingensurecached"></a>Office.TargetedMessaging.EnsureCached 

Prati je li preuzet paket za dinamičko radno područje. Smatra se softverskom konfiguracijom jer se paket mora uspješno preuzeti da bi klijent mogao omogućiti pravo iskustvo. Osobito je važno u korisničkim pretplatama u kojima obavještavamo korisnika putem radnog područja da je licenca istekla. Koristi se za praćenje metapodataka paketa dinamičnog sadržaja kojeg je preuzeo i predmemorirao proizvod, kao i rezultate radnji izvršenih na paketu: neuspjela preuzimanja, neuspjela raspakiranja, pogreške provjere dosljednosti, pronalaženje objekata u predmemoriji, načini korištenja paketa, izvori preuzimanja.

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

#### <a name="officeextensibilityappcommandsappcmdprojectionstatus"></a>Office.Extensibility.AppCommands.AppCmdProjectionStatus

Prikuplja informacije radi praćenja koje su instalacije dodatka za Office uspješno ažurirale vrpcu, a koje nisu.

Koristi se za rješavanje uobičajenih problema s registracijom kada dodaci nisu pravilno instalirani i nikad se ne prikazuju, zbog čega su neupotrebljivi.

Prikupljaju se sljedeća polja:

  - Ne koristi

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

Podaci o uspjehu ili neuspjehu dohvaćanja potrebnih ažuriranih podataka dodataka za administratore klijenta za Office 365. Koristi se za metriku stanja, grafikone i analizu korisničkih problema. ExchangeGetLastUpdate uvijek se pokreće pri pokretanju u sklopu koda glavnog računala i utvrđuje jesu li se promijenili zadaci dodatka za korisnika.  Ako je tako, osf.DLL će se učitati pa možemo pozvati ExchangeGetEntitlements radi dobivanja određenih zadataka (pozvat će se i ExchangeGetManifests radi dohvaćanja novih potrebnih manifesta).  ExchangeGetEntitlements (i ExchangeGetManifests) mogu se također pozvati na zahtjev kada je glavna aplikacija pokrenuta.  Svrha je toga da se ne učita veliki DLL ako nije potreban.  Bez tog događaja u atributu Obavezno ne bismo mogli znati jesu li pokušaji korisnika da dobiju dodijeljene dodatke neuspješni ako prvi servisni poziv ne uspije.  To je i glavni signal za probleme s provjerom autentičnosti s kojima smo suočeni pri razgovaranju sa servisom.

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

Prikuplja informacije o pozivanju poslužitelja za automatizaciju ili klijenta u rješenjima VBA. Koristi se za razumijevanje interakcije između objekata VBA i Com.

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

  - **Standardna HVA aktivnost bez prilagođenog opterećenja**

#### <a name="officeprogrammabilityadd-insinternalsetconnectenterprise"></a>Office.Programmability.Add-ins.InternalSetConnectEnterprise

Događaj koji se stvara kada je COM dodatak učitan na uređaju sa sustavom Enterprise. Analitika za stolna računala: \# učitavanja koristi se kao nazivnik za izračun stanja (\# rušenje / \# učitavanja) za izračun metrike stanja za krugove pilot-verzije i proizvodnje u korporativnim scenarijima. To zahtijeva da podaci budu točni, a ne uzorkovani budući da je broj uređaja manji (100-1K).

Prikupljaju se sljedeća polja:

  - **Add-inconnectFlag** – trenutno ponašanje učitavanja

  - **Add-inDescription** – opis dodatka

  - **Add-inFileName** – naziv datoteke dodatka, bez puta datoteke

  - **Add-inFriendlyName** – neslužbeni naziv dodatka

  - **Add-inId** – ID klase dodatka

  - **Add-inProgId** – programski ID dodatka

  - **Add-inProvider** – davatelj dodatka

  - **Add-inTimeDateStamp** – vremenska oznaka dodatka iz metapodataka DLL-a

  - **Add-inVersion** – verzija dodatka

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

  - **Pravilnik** – je pravilnik koji je postavljen, nije postavljen ili nije dostupan

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

Prati kada se sigurnosni upit prikazuje korisniku prilikom učitavanja ActiveX kontrole koja je označena kao nepouzdana za inicijalizaciju. Koristi se za praćenje rasprostranjenosti UFI ActiveX kontrola u dokumentima sustava Office za poboljšanje rješavanja (npr. kontrole značajke killbit) kao odgovor na sigurnosne incidente.

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


### <a name="application-feature-success-subtype"></a>*Podvrsta uspjeha značajke aplikacije*

Uspješno funkcioniranje aplikacije. Ograničeno na otvaranje i zatvaranje aplikacije i dokumenata, uređivanje datoteka i zajedničko korištenje dokumenata (suradnju).

#### <a name="officeappcompatappcompatagentscanandupload"></a>Office.AppCompat.AppCompat.AgentScanAndUpload

Prikuplja se samo kada je krajnji korisnik omogućio telemetrijsku nadzornu ploču sustava Office. Prikuplja informacije o tome kada se izvršava telemetrijski agent sustava Office.  Prikuplja se samo kada je omogućena telemetrijska nadzorna ploča sustava Office i služi za utvrđivanje stanja telemetrijskog agenta sustava Office.

Prikupljaju se sljedeća polja:

  - **Data.AgentExit** – vremenska oznaka uspješnog zatvaranja telemetrijskog agenta

  - **Data.AgentScan** – vremenska oznaka uspješnog dovršavanja pregleda telemetrijskog agenta

  - **Data.AgentUpload** – vremenska oznaka uspješnog učitavanja telemetrijskog agenta

#### <a name="officeappcompatappcompattelemetrydashboardresiliencycrashlog"></a>Office.AppCompat.AppCompat.TelemetryDashboardResiliencyCrashLog

Prikuplja se samo kada je krajnji korisnik (najčešće administrator) omogućio telemetrijsku nadzornu ploču sustava Office. Prikuplja pojavu rušenja dodataka i dokumenata sustava Office. Prikuplja se samo kada je korisnik omogućio telemetrijsku nadzornu ploču sustava Office i služi za utvrđivanje povećane pojave rušenja dodataka ili dokumenata.

Prikupljaju se sljedeća polja:

  - **Data.CollectionTime** – vremenska oznaka zapisivanja događaja rušenja

#### <a name="officeconnectdeviceactivitystart"></a>Office.ConnectDevice.Activity.Start

Omogućuje da utvrdimo je li uspjelo povezivanje s uređajem ili aplikacijom.  Koristi se za stanje i nadzor značajke. Taj je događaj generirao dodatak Microsoft Data Streamer za Excel.

Prikupljaju se sljedeća polja:

- **Datasource_Type** – informacije o serijskom uređaju ili servisu aplikacije

- **DataSource_Name** – naziv povezanog izvora podataka

- **Activity_Name** = naziv aktivnosti „ConnectDevice“

- **Activity_CV** = ID za povezivanje događaja u sesiji povezivanja

- **Activity_StartStopType** = početak

- **Activity_DateTimeTicks** = vrijeme podataka za aktivnost
 
#### <a name="officeconnectdeviceactivitystop"></a>Office.ConnectDevice.Activity.Stop

Omogućuje da utvrdimo je li uspjelo povezivanje s uređajem ili aplikacijom. Koristi se za stanje i nadzor značajke. Taj je događaj generirao dodatak Microsoft Data Streamer za Excel.

Prikupljaju se sljedeća polja:

- **Datasource_Type** – informacije o serijskom uređaju ili servisu aplikacije

- **DataSource_Name** – naziv povezanog izvora podataka

- **Activity_Name** – naziv aktivnosti „ConnectDevice“

- **Activity_CV** – ID za povezivanje događaja u sesiji povezivanja

- **Activity_StartStopType** – zaustavljanje

- **Activity_DateTimeTicks** – vrijeme podataka za aktivnost

#### <a name="officeextensibilitycatalogexchangeprocessentitlement"></a>Office.Extensibility.Catalog.ExchangeProcessEntitlement

Podaci vezani uz obradu pojedinačnih prava dodatka koji je dodijelio administrator klijenta sustava Office 365.

Koristi se u izradi grafikona (zahtijeva ga upravljanje timom) uspjeha klijenata i analizu korisničkih problema.

Prikupljaju se sljedeća polja:

  - **AppVersion** – verzija glavne aplikacije dodatka

  - **SolutionId** – GUID koji predstavlja jedinstveni dodatak

  - **TelemetryId** – GUID koji predstavlja jedinstvenog korisnika

#### <a name="officefileiocsiccachedfilecsiloadfilebasic"></a>Office.FileIO.CSI.CCachedFileCsiLoadFileBasic

Omogućuje da utvrdimo je li datoteka uspješno otvorena u FIO sloju. Koristi se za stanje i nadzor značajke.

Prikupljaju se sljedeća polja:

  - **Activity.Group –** oznaka koja omogućuje postavljanje grupiranja događaja nadzora za upravljanje ukupnim uspjehom

  - **Activity.IsHVA –** zastavica koja označava da je događaj ključan za uspjeh korisnika

  - **Data.AsyncOpen –** zastavica koja označava da se u otvorenom nalazi sadržaj koji je primljen nakon otvaranja glavnog tijela

  - **Data.CacheFileId –** povezuje se s telemetrijom predmemorije dokumenta sustava Office radi omogućivanja analize utjecaja problema s predmemorijom na korisničko iskustvo

  - **Data.CoauthStatus –** izvješćuje status suradnje dokumenta pri otvaranju

  - **Data.CountOfMultiRoundTripsDownload –** broj povratnih prijenosa na poslužitelj koji se koristi za otklanjanje poteškoća s performansama i mrežom

  - **Data.CountOfMultiRoundTripsUpload –** broj povratnih prijenosa na poslužitelj koji se koristi za otklanjanje poteškoća s performansama i mrežom

  - **Data.DialogId –** postavljeno ako je otvoren dijaloški okvir korisničkog sučelja tijekom otvaranja, što upućuje da je poruka upozorenja prikazana korisniku

  - **Data.DidFallbackToDAV –** postavljeno ako je dokument otvoren pomoću starijeg protokola za prijenos datoteka

  - **Data.Doc.AccessMode –** dokument je samo za čitanje/uređivanje

  - **Data.Doc.AssistedReadingReasons –** postavljeno ako dokument ima aktiviranu zaštitu elektroničkih podataka

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

  - **Data.Input.FileOpenState –** stanje koje je zatražila aplikacija (čitanje/čitanje i pisanje itd.) **-**

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

  - **Data.WopiServiceId –** zastarjelo, zamijenio protokol Data\_Doc\_WopiServiceId

#### <a name="officefileiocsiccachedfilecsisavefilebasic"></a>Office.FileIO.CSI.CCachedFileCsiSaveFileBasic

Omogućuje da utvrdimo je li datoteka uspješno spremljena u FIO sloju. Koristi se za stanje i nadzor značajke.

Prikupljaju se sljedeća polja:

  - **Activity.Group –** oznaka koja omogućuje postavljanje grupiranja događaja nadzora za upravljanje ukupnim uspjehom

  - **Activity.IsHVA –** zastavica koja označava da je događaj ključan za uspjeh korisnika

  - **Data.AsyncOpen –** zastavica koja označava da je dokument otvoren sa sadržajem koji je primljen nakon otvaranja glavnog tijela

  - **Data.BaseDownloadTriggered –** promjena dijagnostike praćenja koja označava da je zatražena osnovna verzija dokumenta

  - **Data.BlockAutoUploadReasons –** kodovi razloga za stanje blokiranog prijenosa (npr. isključeno automatsko spremanje, dokument je u prijelazu)

  - **Data.BlockUploadDueToFailedSaveAsOverExisting –** prijenos je blokiran jer ne bi uspio da je ponovljen

  - **Data.CacheFileId –** povezuje se s telemetrijom predmemorije dokumenta sustava Office radi omogućivanja analize utjecaja problema s predmemorijom na korisničko iskustvo

  - **Data.ChartType –** zastarjelo

  - **Data.CoAuthStatus –** izvješćuje status suradnje dokumenta pri spremanju

  - **Data.CoauthUpdatesContext –** izvješćuje kontekst (spajanje/inkrementalno otvaranje)

  - **Data.CountOfMultiRoundTripsDownload –** broj povratnih prijenosa na poslužitelj koji se koristi za otklanjanje poteškoća s performansama i mrežom

  - **Data.CountOfMultiRoundTripsUpload –** broj povratnih prijenosa na poslužitelj koji se koristi za otklanjanje poteškoća s performansama i mrežom

  - **Data.DialogChoice –** bilježi odabir u dijaloškim okvirima s pogreškom

  - **Data.DialogId –** bilježi DialogId dijaloških okvira s pogreškom prikazanih tijekom spremanja

  - **Data.Dmc.IsOcsSupported –** zastarjelo

  - **Data.Doc.AccessMode –** dokument je samo za čitanje

  - **Data.Doc.AssistedReadingReasons –** postavljeno ako dokument ima aktiviranu zaštitu elektroničkih podataka

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

#### <a name="officeoutlookdesktopprovidersloadproviderlibrary"></a>Office.Outlook.Desktop.Providers.LoadProviderLibrary

Taj događaj prati uspješnost ili neuspješnost MAPI-ja pri učitavanju DLL-a davatelja usluge (npr. contab32.dll, emsmdb32.dll, DLL koji dodatak koristi). Operacija MAPI odgovorna za učitavanje DLL-ova davatelja usluge bitna je za osnovni rad programa Outlook kao i za mogućnosti proširenja (putem dodataka ili prilagođenih davatelja trgovine/prijenosa/adresara). Aktivno pratimo rezultat uspješnosti ili neuspješnosti ove operacije kako bismo osigurali da osnovna funkcija MAPI-ja nastavi funkcionirati prema očekivanjima.

Prikupljaju se sljedeća polja:

  - **Standardna HVA aktivnost** bez prilagođenog opterećenja

#### <a name="officeoutlookdesktopstorescreatenewstore"></a>Office.Outlook.Desktop.Stores.CreateNewStore

Prikuplja rezultat stvaranja nove trgovine (s vrstom i verzijom), kao i kod rezultata. Aktivno pratimo taj događaj radi praćenja stanja korisnikove mogućnosti sinkroniziranja i pohrane pošte lokalno, arhiviranje poruka e-pošte (u PST) ili korištenje grupa.

Prikupljaju se sljedeća polja:

  - **Standardna HVA aktivnost** s prilagođenim opterećenjem

  - **StoreType** – vrsta trgovine koju stvara OST/PST/NST

  - **StoreVersion** – verzija trgovine koja stvara Small/Large/Tardis

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

  - **Data\_Doc\_ChunkingType:long –** kako je dokument pohranjen u sustavu SharePoint

  - **Data\_Doc\_EdpState:long –** stanje dokumenta s obzirom na zaštitu korporativnih podataka

  - **Data\_Doc\_Ext:string –** nastavak dokumenta

  - **Data\_Doc\_Extension:string –** nastavak dokumenta

  - **Data\_Doc\_FileFormat:long –** unaprijed definirani skup vrijednosti oblika datoteke (precizniji od nastavka)

  - **Data\_Doc\_Fqdn:string –** mjesto pohrane dokumenta (SharePoint.com, live.net), dostupno samo za domene sustava Office 365

  - **Data\_Doc\_FqdnHash:string –** raspršivanje mjesta pohrane dokumenta

  - **Data\_Doc\_IdentityTelemetryId:string –** jedinstveni GUID korisnika

  - **Data\_Doc\_IdentityUniqueId:string –** jedinstveni identifikator identiteta korišten za akciju zajedničkih dokumenata

  - **Data\_Doc\_IOFlags:long –** bit-maska za razne zastavice vezane uz ulaz i izlaz za određeni dokument

  - **Data\_Doc\_IrmRights:long –** unaprijed definiran skup vrijednosti za vrstu informacija koju upravljanje pravima na informacije primjenjuje na ovom dokumentu (proslijedi, odgovori, SecureReader, uređivanje itd.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool –** istinito ako je HTTP zaglavlje „IsCloudCollabEnabled“ već prihvaćeno iz zahtjeva MOGUĆNOSTI.

  - **Data\_Doc\_IsIncrementalOpen:bool –** je li dokument otvoren inkrementalno (nova značajka koja otvara dokument bez potrebe za preuzimanjem cijelog dokumenta)

  - **Data\_Doc\_IsOcsSupported:bool –** podržava li dokument suautorstvo pomoću novog servisa OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool –** provjerava otvara li se dokument iz lokalne predmemorije

  - **Data_Doc_IsRtcAlwaysOn –** istinito ako je kanal u stvarnom vremenu (RTC) uvijek uključen za ovu datoteku.

  - **Data\_Doc\_IsSyncBacked:bool –** provjerava otvara li se dokument iz mape koja koristi aplikaciju OneDrive za povratnu sinkronizaciju

  - **Data\_Doc\_Location:long –** unaprijed definiran skup vrijednosti mjesta na kojima se dokument pohranjuje (lokalno, SharePoint, WOPI, mreža itd.)

  - **Data\_Doc\_LocationDetails:long –** unaprijed definiran skup vrijednosti detaljnijih lokacija (mapa Temp, mapa preuzimanja, dokumenti servisa One Drive, slike servisa One Drive itd.)

  - **Data\_Doc\_NumberCoAuthors:long –** broj suautora prilikom otvaranja dokumenta

  - **Data\_Doc\_PasswordFlags:long –** unaprijed definirani skup vrijednosti načina na koji je dokument šifriran pomoću lozinke (nema, lozinka za čitanje, lozinka za uređivanje)

  - **Data\_Doc\_ReadOnlyReasons:long –** unaprijed definirani skup vrijednosti koji naznačuje zašto je dokument označen samo za čitanje (zaključan na poslužitelju, konačni dokument, zaštićen lozinkom za uređivanje itd.)

  - **Data\_Doc\_ResourceIdHash:string –** raspršivanje identifikatora resursa za dokumente pohranjene u oblaku

  - **Data\_Doc\_ServerDocId:string –** nepromjenjivi identifikator za dokumente pohranjene u oblaku

  - **Data\_Doc\_ServerProtocol:long –** unaprijed definirani skup vrijednosti o protokolu koji se koristi za komuniciranje s poslužiteljem (Http, Cobalt, WOPI itd.)

  - **Data\_Doc\_ServerType:long –** unaprijed definirani skup vrijednosti o vrsti poslužitelja (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long –** provjerava temelji li se poslužitelj na sustavu Office14, Office15 ili Office 16

  - **Data\_Doc\_SessionId:long –** generirani GUID koji identificira instancu dokumenta u sklopu iste sesije procesa

  - **Data\_Doc\_SharePointServiceContext:string –** neprozirni niz, obično GridManagerID.FarmID. Korisno za korelaciju klijentskih i poslužiteljskih zapisnika

  - **Data\_Doc\_SizeInBytes:long –** veličina dokumenta u bajtovima

  - **Data\_Doc\_SpecialChars:long –** bit-maska koja pokazuje posebne znakove u URL-u ili putu dokumenta

  - **Data\_Doc\_StorageProviderId:string –** niz koji određuje davatelja pohrane dokumenta, primjerice „DropBox“

  - **Data\_Doc\_StreamAvailability:long –** unaprijed definirani skup vrijednosti statusa toka dokumenta (dostupno, trajno onemogućeno, nije dostupno)

  - **Data\_Doc\_UrlHash:string –** raspršivanje punog URL-a dokumenata pohranjenih u oblaku

  - **Data\_Doc\_UsedWrsDataOnOpen:bool –** istinito ako je datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka na glavnom računalu

  - **Data\_Doc\_WopiServiceId:string –** identifikator WOPI servisa, npr. „Dropbox“

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

  - **Data\_UserContinuedZRTClose:bool –** nakon prikazivanja dijaloškog okvira prilikom zatvaranja, je li korisnik odabrao „Nastavi“ za zatvaranje?

#### <a name="officepowerpointdocoperationnewdocument"></a>Office.PowerPoint.DocOperation.NewDocument

Prikuplja se kada PowerPoint stvori novu prezentaciju. Obuhvaća metriku uspjeha, neuspjeha i performansi.

Te se informacije koriste da bismo uspješno stvorili datoteke bez smanjenih performansi.

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

  - **Data\_Doc\_ChunkingType:long –** kako je dokument pohranjen u sustavu SharePoint

  - **Data\_Doc\_EdpState:long –** stanje dokumenta s obzirom na zaštitu korporativnih podataka

  - **Data\_Doc\_Ext:string –** nastavak dokumenta

  - **Data\_Doc\_Extension:string –** nastavak dokumenta

  - **Data\_Doc\_FileFormat:long –** unaprijed definirani skup vrijednosti oblika datoteke (precizniji od nastavka)

  - **Data\_Doc\_Fqdn:string –** mjesto pohrane dokumenta (SharePoint.com, live.net), dostupno samo za domene sustava Office 365

  - **Data\_Doc\_FqdnHash:string –** raspršivanje mjesta pohrane dokumenta

  - **Data\_Doc\_IdentityTelemetryId:string –** jedinstveni GUID korisnika

  - **Data\_Doc\_IdentityUniqueId:string –** jedinstveni identifikator identiteta korišten za akciju zajedničkih dokumenata

  - **Data\_Doc\_IOFlags:long –** bit-maska za razne zastavice vezane uz ulaz i izlaz za određeni dokument

  - **Data\_Doc\_IrmRights:long –** unaprijed definiran skup vrijednosti za vrstu informacija koju upravljanje pravima na informacije primjenjuje na ovom dokumentu (proslijedi, odgovori, SecureReader, uređivanje itd.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool –** istinito ako je HTTP zaglavlje „IsCloudCollabEnabled“ već prihvaćeno iz zahtjeva MOGUĆNOSTI.

  - **Data\_Doc\_IsIncrementalOpen:bool –** je li dokument otvoren inkrementalno (nova značajka koja otvara dokument bez potrebe za preuzimanjem cijelog dokumenta)

  - **Data\_Doc\_IsOcsSupported:bool –** podržava li dokument suautorstvo pomoću novog servisa OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool –** otvara li se dokument iz lokalne predmemorije?

  - **Data_Doc_IsRtcAlwaysOn –** istinito ako je kanal u stvarnom vremenu (RTC) uvijek uključen za ovu datoteku.

  - **Data\_Doc\_IsSyncBacked:bool –** otvara li se dokument iz mape koja koristi aplikaciju OneDrive za povratnu sinkronizaciju

  - **Data\_Doc\_Location:long –** unaprijed definiran skup vrijednosti mjesta na kojima se dokument pohranjuje (lokalno, SharePoint, WOPI, mreža itd.)

  - **Data\_Doc\_LocationDetails:long –** unaprijed definiran skup vrijednosti detaljnijih lokacija (mapa Temp, mapa preuzimanja, dokumenti servisa One Drive, slike servisa One Drive itd.)

  - **Data\_Doc\_NumberCoAuthors:long –** broj suautora prilikom otvaranja dokumenta

  - **Data\_Doc\_PasswordFlags:long –** unaprijed definirani skup vrijednosti načina na koji je dokument šifriran pomoću lozinke (nema, lozinka za čitanje, lozinka za uređivanje)

  - **Data\_Doc\_ReadOnlyReasons:long –** unaprijed definirani skup vrijednosti koji naznačuje zašto je dokument označen samo za čitanje (zaključan na poslužitelju, konačni dokument, zaštićen lozinkom za uređivanje itd.)

  - **Data\_Doc\_ResourceIdHash:string –** raspršivanje identifikatora resursa za dokumente pohranjene u oblaku

  - **Data\_Doc\_ServerDocId:string –** nepromjenjivi identifikator za dokumente pohranjene u oblaku

  - **Data\_Doc\_ServerProtocol:long –** unaprijed definirani skup vrijednosti o protokolu koji se koristi za komuniciranje s poslužiteljem (Http, Cobalt, WOPI itd.)

  - **Data\_Doc\_ServerType:long –** unaprijed definirani skup vrijednosti o vrsti poslužitelja (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long –** provjerava temelji li se poslužitelj na sustavu Office14, Office15 ili Office 16

  - **Data\_Doc\_SessionId:long –** generirani GUID koji identificira instancu dokumenta u sklopu iste sesije procesa

  - **Data\_Doc\_SharePointServiceContext:string –** neprozirni niz, obično GridManagerID.FarmID. Korisno za korelaciju klijentskih i poslužiteljskih zapisnika

  - **Data\_Doc\_SizeInBytes:long –** veličina dokumenta u bajtovima

  - **Data\_Doc\_SpecialChars:long –** bit-maska koja pokazuje posebne znakove u URL-u ili putu dokumenta

  - **Data\_Doc\_StorageProviderId:string –** niz koji određuje davatelja pohrane dokumenta, primjerice „DropBox“

  - **Data\_Doc\_StreamAvailability:long –** unaprijed definirani skup vrijednosti statusa toka dokumenta (dostupno, trajno onemogućeno, nije dostupno)

  - **Data\_Doc\_UrlHash:string –** raspršivanje punog URL-a dokumenata pohranjenih u oblaku

  - **Data\_Doc\_UsedWrsDataOnOpen:bool –** istinito ako je datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka na glavnom računalu

  - **Data\_Doc\_WopiServiceId:string –** identifikator WOPI servisa, npr. „Dropbox“

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

Prikuplja se svaki put kada PowerPoint izvodi spremanje pomoću modernog puta koda. Obuhvaća vrstu rezultata uspješno ili neuspješno metrike performansi spremanja i relevantnih metapodataka dokumenta.  Problemi sa spremanjem mogu uzrokovati gubitak podataka. Microsoft koristi te podatke da bi osigurao da značajka funkcionira prema očekivanjima i da se korisnički sadržaj uspješno održava.

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

  - **Data\_Doc\_ChunkingType:long –** kako je dokument pohranjen u sustavu SharePoint

  - **Data\_Doc\_EdpState:long –** stanje dokumenta s obzirom na zaštitu korporativnih podataka

  - **Data\_Doc\_Ext:string –** nastavak dokumenta

  - **Data\_Doc\_Extension:string –** nastavak dokumenta

  - **Data\_Doc\_FileFormat:long –** unaprijed definirani skup vrijednosti oblika datoteke (precizniji od nastavka)

  - **Data\_Doc\_Fqdn:string –** mjesto pohrane dokumenta (SharePoint.com, live.net), dostupno samo za domene sustava Office 365

  - **Data\_Doc\_FqdnHash:string –** raspršivanje mjesta pohrane dokumenta

  - **Data\_Doc\_IdentityTelemetryId:string –** jedinstveni GUID korisnika

  - **Data\_Doc\_IdentityUniqueId:string –** jedinstveni identifikator identiteta korišten za akciju zajedničkih dokumenata

  - **Data\_Doc\_IOFlags:long –** bit-maska za razne zastavice vezane uz ulaz i izlaz za određeni dokument

  - **Data\_Doc\_IrmRights:long –** unaprijed definiran skup vrijednosti za vrstu informacija koju upravljanje pravima na informacije primjenjuje na ovom dokumentu (proslijedi, odgovori, SecureReader, uređivanje itd.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool –** istinito ako je HTTP zaglavlje „IsCloudCollabEnabled“ već prihvaćeno iz zahtjeva MOGUĆNOSTI.

  - **Data\_Doc\_IsIncrementalOpen:bool –** je li dokument otvoren inkrementalno (nova značajka koja otvara dokument bez potrebe za preuzimanjem cijelog dokumenta)

  - **Data\_Doc\_IsOcsSupported:bool –** podržava li dokument suautorstvo pomoću novog servisa OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool –** provjerava otvara li se dokument iz lokalne predmemorije

  - **Data_Doc_IsRtcAlwaysOn –** istinito ako je kanal u stvarnom vremenu (RTC) uvijek uključen za ovu datoteku.

  - **Data\_Doc\_IsSyncBacked:bool –** otvara li se dokument iz mape koja koristi aplikaciju OneDrive za povratnu sinkronizaciju

  - **Data\_Doc\_Location:long –** unaprijed definiran skup vrijednosti mjesta na kojima se dokument pohranjuje (lokalno, SharePoint, WOPI, mreža itd.)

  - **Data\_Doc\_LocationDetails:long –** unaprijed definiran skup vrijednosti detaljnijih lokacija (mapa Temp, mapa preuzimanja, dokumenti servisa One Drive, slike servisa One Drive itd.)

  - **Data\_Doc\_NumberCoAuthors:long –** broj suautora prilikom otvaranja dokumenta

  - **Data\_Doc\_PasswordFlags:long –** unaprijed definirani skup vrijednosti načina na koji je dokument šifriran pomoću lozinke (nema, lozinka za čitanje, lozinka za uređivanje)

  - **Data\_Doc\_ReadOnlyReasons:long –** unaprijed definirani skup vrijednosti koji naznačuje zašto je dokument označen samo za čitanje (zaključan na poslužitelju, konačni dokument, zaštićen lozinkom za uređivanje itd.)

  - **Data\_Doc\_ResourceIdHash:string –** raspršivanje identifikatora resursa za dokumente pohranjene u oblaku

  - **Data\_Doc\_ServerDocId:string –** nepromjenjivi identifikator za dokumente pohranjene u oblaku

  - **Data\_Doc\_ServerProtocol:long –** unaprijed definirani skup vrijednosti o protokolu koji se koristi za komuniciranje s poslužiteljem (Http, Cobalt, WOPI itd.)

  - **Data\_Doc\_ServerType:long –** unaprijed definirani skup vrijednosti o vrsti poslužitelja (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long –** provjerava temelji li se poslužitelj na sustavu Office14, Office15 ili Office 16

  - **Data\_Doc\_SessionId:long –** generirani GUID koji identificira instancu dokumenta u sklopu iste sesije procesa

  - **Data\_Doc\_SharePointServiceContext:string –** neprozirni niz, obično GridManagerID.FarmID. Korisno za korelaciju klijentskih i poslužiteljskih zapisnika

  - **Data\_Doc\_SizeInBytes:long –** veličina dokumenta u bajtovima

  - **Data\_Doc\_SpecialChars:long –** bit-maska koja pokazuje posebne znakove u URL-u ili putu dokumenta

  - **Data\_Doc\_StorageProviderId:string –** niz koji određuje davatelja pohrane dokumenta, primjerice „DropBox“

  - **Data\_Doc\_StreamAvailability:long –** unaprijed definirani skup vrijednosti statusa toka dokumenta (dostupno, trajno onemogućeno, nije dostupno)

  - **Data\_Doc\_UrlHash:string –** raspršivanje punog URL-a dokumenata pohranjenih u oblaku

  - **Data\_Doc\_UsedWrsDataOnOpen:bool –** istinito ako je datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka na glavnom računalu

  - **Data\_Doc\_WopiServiceId:string –** identifikator WOPI servisa, npr. „Dropbox“

  - **Data\_DurationUAEOnSaveStartedMs:long –** vrijeme potrebno za zatvaranje nepoznate aplikacije tijekom spremanja

  - **Data\_EnsureSaveTransactionTimeMS:long –** vrijeme potrebno za stvaranje transakcije spremanja ako već ne postoji

  - **Data\_FailureComponent:long–** unaprijed definirani skup vrijednosti koji označava koja je komponenta uzrokovala neuspjeh ovog protokola? (Conflict, CSI, Internal itd.)

  - **Data\_FailureReason:long –** unaprijed definirani skup vrijednosti koji označava razlog pogreške (FileIsCorrupt, BlockedByAntivirus itd.)

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

Prikuplja se svaki put kada PowerPoint izvodi Spremi u obliku. Obuhvaća vrstu rezultata uspješno ili neuspješno metrike performansi spremanja i relevantnih metapodataka dokumenta. Problemi sa spremanjem mogu uzrokovati gubitak podataka.

Microsoft koristi te podatke da bi osigurao da značajka funkcionira prema očekivanjima i da se korisnički sadržaj uspješno održava.

Prikupljaju se sljedeća polja:

  - **Data\_AddDocTelemetryResult:long –** ima li ova stavka zapisnika svu potrebnu telemetriju dokumenta (polja Data\_Doc\_\*)? Ako ne, zašto?

  - **Data\_CppUncaughtExceptionCount:long –** neuhvaćene lokalne iznimke dok je aktivnost pokrenuta

  - **Data\_DetachedDuration:long –** vrijeme tijekom kojeg je aktivnost isključena/nije pokrenuta

  - **Data\_Doc\_AccessMode:long –** kako je dokument otvoren (samo za čitanje | čitanje i pisanje)

  - **Data\_DstDoc\_AssistedReadingReasons:long –** unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

  - **Data\_DstDoc\_ChunkingType:long –** kako je dokument pohranjen u sustavu SharePoint

  - **Data\_DstDoc\_EdpState:long –** stanje dokumenta s obzirom na zaštitu korporativnih podataka

  - **Data\_DstDoc\_Ext:string –** nastavak dokumenta

  - **Data\_DstDoc\_Extension:string –** nastavak dokumenta

  - **Data\_DstDoc\_FileFormat:long –** unaprijed definirani skup vrijednosti oblika datoteke (precizniji od nastavka)

  - **Data\_DstDoc\_Fqdn:string –** mjesto pohrane dokumenta (SharePoint.com, live.net), dostupno samo za domene sustava Office 365

  - **Data\_DstDoc\_FqdnHash:string –** raspršivanje mjesta pohrane dokumenta

  - **Data\_DstDoc\_IdentityTelemetryId:string –** jedinstveni GUID korisnika

  - **Data\_DstDoc\_IdentityUniqueId:string –** jedinstveni identifikator identiteta korišten za akciju zajedničkih dokumenata

  - **Data\_DstDoc\_IOFlags:long –** bit-maska za razne zastavice vezane uz ulaz i izlaz za određeni dokument

  - **Data\_DstDoc\_IrmRights:long –** unaprijed definirani skup vrijednosti za vrstu informacija koju upravljanje pravima primjenjuje na ovom dokumentu (proslijedi, odgovori, SecureReader, uređivanje itd.)

  - **Data\_DstDoc\_IsCloudCollabEnabled:bool –** istinito ako je HTTP zaglavlje „IsCloudCollabEnabled“ već prihvaćeno iz zahtjeva MOGUĆNOSTI.

  - **Data\_DstDoc\_IsIncrementalOpen:bool –** je li dokument otvoren inkrementalno (nova značajka koja otvara dokument bez potrebe za preuzimanjem cijelog dokumenta)

  - **Data\_DstDoc\_IsOcsSupported:bool –** podržava li dokument suautorstvo pomoću novog servisa OCS

  - **Data\_DstDoc\_IsOpeningOfflineCopy:bool –** provjerava otvara li se dokument iz lokalne predmemorije

  - **Data\_DstDoc\_IsSyncBacked:bool –** otvara li se dokument iz mape koja koristi aplikaciju OneDrive za povratnu sinkronizaciju

  - **Data\_DstDoc\_Location:long –** unaprijed definiran skup vrijednosti mjesta na kojima se dokument pohranjuje (lokalno, SharePoint, WOPI, mreža itd.)

  - **Data\_DstDoc\_LocationDetails:long –** unaprijed definiran skup vrijednosti detaljnijih lokacija (mapa Temp, mapa preuzimanja, dokumenti servisa One Drive, slike servisa One Drive itd.)

  - **Data\_DstDoc\_NumberCoAuthors:long –** broj suautora prilikom otvaranja dokumenta

  - **Data\_DstDoc\_PasswordFlags:long –** unaprijed definirani skup vrijednosti načina na koji je dokument šifriran pomoću lozinke (nema, lozinka za čitanje, lozinka za uređivanje)

  - **Data\_DstDoc\_ReadOnlyReasons:long –** unaprijed definirani skup vrijednosti koji naznačuje zašto je dokument označen samo za čitanje (zaključan na poslužitelju, konačni dokument, zaštićen lozinkom za uređivanje itd.)

  - **Data\_DstDoc\_ResourceIdHash:string –** raspršivanje identifikatora resursa za dokumente pohranjene u oblaku

  - **Data\_DstDoc\_ServerDocId:string –** nepromjenjivi identifikator za dokumente pohranjene u oblaku

  - **Data\_DstDoc\_ServerProtocol:long –** unaprijed definirani skup vrijednosti o protokolu koji se koristi za komuniciranje s poslužiteljem (Http, Cobalt, WOPI itd.)

  - **Data\_DstDoc\_ServerType:long –** unaprijed definirani skup vrijednosti o vrsti poslužitelja (SharePoint, DropBox, WOPI)

  - **Data\_DstDoc\_ServerVersion:long –** provjerava temelji li se poslužitelj na sustavu Office14, Office15 ili Office 16

  - **Data\_DstDoc\_SessionId:long –** generirani GUID koji identificira instancu dokumenta u sklopu iste sesije procesa

  - **Data\_DstDoc\_SharePointServiceContext:string –** neprozirni niz, obično GridManagerID.FarmID. Korisno za korelaciju klijentskih i poslužiteljskih zapisnika

  - **Data\_DstDoc\_SizeInBytes:long –** veličina dokumenta u bajtovima

  - **Data\_DstDoc\_SpecialChars:long –** bit-maska koja pokazuje posebne znakove u URL-u ili putu dokumenta

  - **Data\_DstDoc\_StorageProviderId:string –** niz koji određuje davatelja pohrane dokumenta, primjerice „DropBox“

  - **Data\_DstDoc\_StreamAvailability:long –** unaprijed definirani skup vrijednosti statusa toka dokumenta (dostupno, trajno onemogućeno, nije dostupno)

  - **Data\_DstDoc\_UrlHash:string –** raspršivanje punog URL-a dokumenata pohranjenih u oblaku

  - **Data\_DstDoc\_UsedWrsDataOnOpen:bool –** istinito ako je datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka na glavnom računalu

  - **Data\_DstDoc\_WopiServiceId:string –** identifikator WOPI servisa, npr. „Dropbox“

  - **Data\_FileType:long –** unaprijed definirani skup vrijednosti interne vrste datoteke

  - **Data\_fLifeguarded:bool –** je li dokument ikad popravljen pomoću značajke lifeguard (značajka za popravljanje pogrešaka dokumenta bez slanja upita korisniku)?

  - **Data\_FWebCreated:bool –** ima li ovaj dokument zastavicu WebCreator?

  - **Data\_SaveReason:long –** unaprijed definirani skup vrijednosti koji označava zašto je izvršeno spremanje? (AutoSave, ToOCSTransitionSave, ToCSITransitionSave itd.)

  - **Data\_SaveType:long –** unaprijed definirani skup vrijednosti o vrsti spremanja (SaveAs, Publish, Manual, OMSave itd.)

  - **Data\_SrcDoc\_AccessMode:long –** kako je dokument otvoren (samo za čitanje | čitanje i pisanje)

  - **Data\_SrcDoc\_AssistedReadingReasons:long –** unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

  - **Data\_SrcDoc\_ChunkingType:long –** kako je dokument pohranjen u sustavu SharePoint

  - **Data\_SrcDoc\_EdpState:long –** stanje dokumenta s obzirom na zaštitu korporativnih podataka

  - **Data\_SrcDoc\_Ext:string –** nastavak dokumenta

  - **Data\_SrcDoc\_Extension:string –** nastavak dokumenta

  - **Data\_SrcDoc\_FileFormat:long –** unaprijed definirani skup vrijednosti oblika datoteke (precizniji od nastavka)

  - **Data\_SrcDoc\_Fqdn:string –** mjesto pohrane dokumenta (SharePoint.com, live.net), dostupno samo za domene sustava Office 365

  - **Data\_SrcDoc\_FqdnHash:string –** raspršivanje mjesta pohrane dokumenta

  - **Data\_SrcDoc\_IdentityTelemetryId:string –** jedinstveni GUID korisnika

  - **Data\_SrcDoc\_IdentityUniqueId:string –** jedinstveni identifikator identiteta korišten za akciju zajedničkih dokumenata

  - **Data\_SrcDoc\_IOFlags:long –** bit-maska za razne zastavice vezane uz ulaz i izlaz za određeni dokument

  - **Data\_SrcDoc\_IrmRights:long –** unaprijed definirani skup vrijednosti za vrstu informacija koju upravljanje pravima primjenjuje na ovom dokumentu (proslijedi, odgovori, SecureReader, uređivanje itd.)

  - **Data\_SrcDoc\_IsCloudCollabEnabled:bool –** istinito ako je HTTP zaglavlje „IsCloudCollabEnabled“ već prihvaćeno iz zahtjeva MOGUĆNOSTI.

  - **Data\_SrcDoc\_IsIncrementalOpen:bool –** je li dokument otvoren inkrementalno (nova značajka koja otvara dokument bez potrebe za preuzimanjem cijelog dokumenta)

  - **Data\_SrcDoc\_IsOcsSupported:bool –** podržava li dokument suautorstvo pomoću novog servisa OCS

  - **Data\_SrcDoc\_IsOpeningOfflineCopy:bool –** provjerava otvara li se dokument iz lokalne predmemorije

  - **Data\_SrcDoc\_IsSyncBacked:bool –** otvara li se dokument iz mape koja koristi aplikaciju OneDrive za povratnu sinkronizaciju

  - **Data\_SrcDoc\_Location:long –** unaprijed definiran skup vrijednosti mjesta na kojima se dokument pohranjuje (lokalno, SharePoint, WOPI, mreža itd.)

  - **Data\_SrcDoc\_LocationDetails:long –** unaprijed definiran skup vrijednosti detaljnijih lokacija (mapa Temp, mapa preuzimanja, dokumenti servisa One Drive, slike servisa One Drive itd.)

  - **Data\_SrcDoc\_NumberCoAuthors:long –** broj suautora prilikom otvaranja dokumenta

  - **Data\_SrcDoc\_PasswordFlags:long –** unaprijed definirani skup vrijednosti načina na koji je dokument šifriran pomoću lozinke (nema, lozinka za čitanje, lozinka za uređivanje)

  - **Data\_SrcDoc\_ReadOnlyReasons:long –** unaprijed definirani skup vrijednosti koji naznačuje zašto je dokument označen samo za čitanje (zaključan na poslužitelju, konačni dokument, zaštićen lozinkom za uređivanje itd.)

  - **Data\_SrcDoc\_ResourceIdHash:string –** raspršivanje identifikatora resursa za dokumente pohranjene u oblaku

  - **Data\_SrcDoc\_ServerDocId:string –** nepromjenjivi identifikator za dokumente pohranjene u oblaku

  - **Data\_SrcDoc\_ServerProtocol:long –** unaprijed definirani skup vrijednosti o protokolu koji se koristi za komuniciranje s poslužiteljem (Http, Cobalt, WOPI itd.)

  - **Data\_SrcDoc\_ServerType:long –** unaprijed definirani skup vrijednosti o vrsti poslužitelja (SharePoint, DropBox, WOPI)

  - **Data\_SrcDoc\_ServerVersion:long –** provjerava temelji li se poslužitelj na sustavu Office14, Office15 ili Office 16Data\_SrcDoc\_SessionId:long generirani GUID koji prepoznaje instancu dokumenta u istoj sesiji postupka

  - **Data\_SrcDoc\_SharePointServiceContext:string –** neprozirni niz, obično GridManagerID.FarmID. Korisno za korelaciju klijentskih i poslužiteljskih zapisnika

  - **Data\_SrcDoc\_SizeInBytes:long –** veličina dokumenta u bajtovima

  - **Data\_SrcDoc\_SpecialChars:long –** bit-maska koja pokazuje posebne znakove u URL-u ili putu dokumenta

  - **Data\_SrcDoc\_StorageProviderId:string –** niz koji određuje davatelja pohrane dokumenta, primjerice „DropBox“

  - **Data\_SrcDoc\_StreamAvailability:long –** unaprijed definirani skup vrijednosti statusa toka dokumenta (dostupno, trajno onemogućeno, nije dostupno)

  - **Data\_SrcDoc\_UrlHash:string –** raspršivanje punog URL-a dokumenata pohranjenih u oblaku

  - **Data\_SrcDoc\_UsedWrsDataOnOpen:bool –** istinito ako je datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka na glavnom računalu

  - **Data\_SrcDoc\_WopiServiceId:string –** identifikator WOPI servisa, npr. „Dropbox“

  - **Data\_StopwatchDuration:long –** ukupno vrijeme za aktivnost

  - **Data\_TypeOfSaveDialog:long –** unaprijed definirani skup vrijednosti dijaloškog okvira (RUN\_SAVEAS\_DLG, RUN\_SAVEMEDIA\_DLG, RUN\_SAVEAS\_VIDEO\_DLG etd.)

  - **DstDoc –** nova lokacija dokumenta

  - **SrcDoc –** izvorna lokacija dokumenta

#### <a name="officepowerpointdocoperationsavelegacy"></a>Office.PowerPoint.DocOperation.SaveLegacy

Prikuplja se svaki put kada PowerPoint izvodi spremanje pomoću naslijeđenog puta koda. Obuhvaća vrstu rezultata uspješno ili neuspješno metrike performansi spremanja i relevantnih metapodataka dokumenta. Problemi sa spremanjem mogu uzrokovati gubitak podataka. Microsoft koristi te podatke da bi osigurao da značajka funkcionira prema očekivanjima i da se korisnički sadržaj uspješno održava.

Prikupljaju se sljedeća polja:

  - **Data\_AddDocTelemetryResult:long –** ima li ova stavka zapisnika svu potrebnu telemetriju dokumenta (polja Data\_Doc\_\*)? Ako ne, zašto?

  - **Data\_CppUncaughtExceptionCount:long –** neuhvaćene lokalne iznimke dok je aktivnost pokrenuta

  - **Data\_DetachedDuration:long –** vrijeme tijekom kojeg je aktivnost isključena/nije pokrenuta

  - **Data\_Doc\_AccessMode:long –** kako je dokument otvoren (samo za čitanje | samo za pisanje)

  - **Data\_Doc\_AssistedReadingReasons:long –** unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

  - **Data\_Doc\_ChunkingType:long –** kako je dokument pohranjen u sustavu SharePoint

  - **Data\_Doc\_EdpState:long –** stanje dokumenta s obzirom na zaštitu korporativnih podataka

  - **Data\_Doc\_Ext:string –** nastavak dokumenta

  - **Data\_Doc\_Extension:string –** nastavak dokumenta

  - **Data\_Doc\_FileFormat:long –** unaprijed definirani skup vrijednosti oblika datoteke (precizniji od nastavka)

  - **Data\_Doc\_Fqdn:string –** mjesto pohrane dokumenta (SharePoint.com, live.net), dostupno samo za domene sustava Office 365

  - **Data\_Doc\_FqdnHash:string –** raspršivanje mjesta pohrane dokumenta

  - **Data\_Doc\_IdentityTelemetryId:string –** jedinstveni GUID korisnika

  - **Data\_Doc\_IdentityUniqueId:string –** jedinstveni identifikator identiteta korišten za akciju zajedničkih dokumenata

  - **Data\_Doc\_IOFlags:long –** bit-maska za razne zastavice vezane uz ulaz i izlaz za određeni dokument

  - **Data\_Doc\_IrmRights:long –** unaprijed definiran skup vrijednosti za vrstu informacija koju upravljanje pravima na informacije primjenjuje na ovom dokumentu (proslijedi, odgovori, SecureReader, uređivanje itd.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool –** istinito ako je HTTP zaglavlje „IsCloudCollabEnabled“ već prihvaćeno iz zahtjeva MOGUĆNOSTI.

  - **Data\_Doc\_IsIncrementalOpen:bool –** je li dokument otvoren inkrementalno (nova značajka koja otvara dokument bez potrebe za preuzimanjem cijelog dokumenta)

  - **Data\_Doc\_IsOcsSupported:bool –** podržava li dokument suautorstvo pomoću novog servisa OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool –** provjerava otvara li se dokument iz lokalne predmemorije

  - **Data_Doc_IsRtcAlwaysOn –** istinito ako je kanal u stvarnom vremenu (RTC) uvijek uključen za ovu datoteku.

  - **Data\_Doc\_IsSyncBacked:bool –** otvara li se dokument iz mape koja koristi aplikaciju OneDrive za povratnu sinkronizaciju

  - **Data\_Doc\_Location:long –** unaprijed definiran skup vrijednosti mjesta na kojima se dokument pohranjuje (lokalno, SharePoint, WOPI, mreža itd.)

  - **Data\_Doc\_LocationDetails:long –** unaprijed definiran skup vrijednosti detaljnijih lokacija (mapa Temp, mapa preuzimanja, dokumenti servisa One Drive, slike servisa One Drive itd.)

  - **Data\_Doc\_NumberCoAuthors:long –** broj suautora prilikom otvaranja dokumenta

  - **Data\_Doc\_PasswordFlags:long –** unaprijed definirani skup vrijednosti načina na koji je dokument šifriran pomoću lozinke (nema, lozinka za čitanje, lozinka za uređivanje)

  - **Data\_Doc\_ReadOnlyReasons:long –** unaprijed definirani skup vrijednosti koji naznačuje zašto je dokument označen samo za čitanje (zaključan na poslužitelju, konačni dokument, zaštićen lozinkom za uređivanje itd.)

  - **Data\_Doc\_ResourceIdHash:string –** raspršivanje identifikatora resursa za dokumente pohranjene u oblaku

  - **Data\_Doc\_ServerDocId:string –** nepromjenjivi identifikator za dokumente pohranjene u oblaku

  - **Data\_Doc\_ServerProtocol:long –** unaprijed definirani skup vrijednosti o protokolu koji se koristi za komuniciranje s poslužiteljem (Http, Cobalt, WOPI itd.)

  - **Data\_Doc\_ServerType:long –** unaprijed definirani skup vrijednosti o vrsti poslužitelja (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long –** provjerava temelji li se poslužitelj na sustavu Office14, Office15 ili Office 16

  - **Data\_Doc\_SessionId:long –** generirani GUID koji identificira instancu dokumenta u sklopu iste sesije procesa

  - **Data\_Doc\_SharePointServiceContext:string –** neprozirni niz, obično GridManagerID.FarmID. Korisno za korelaciju klijentskih i poslužiteljskih zapisnika

  - **Data\_Doc\_SizeInBytes:long –** veličina dokumenta u bajtovima

  - **Data\_Doc\_SpecialChars:long –** bit-maska koja pokazuje posebne znakove u URL-u ili putu dokumenta

  - **Data\_Doc\_StorageProviderId:string –** niz koji određuje davatelja pohrane dokumenta, primjerice „DropBox“

  - **Data\_Doc\_StreamAvailability:long –** unaprijed definirani skup vrijednosti statusa toka dokumenta (dostupno, trajno onemogućeno, nije dostupno)

  - **Data\_Doc\_UrlHash:string –** raspršivanje punog URL-a dokumenata pohranjenih u oblaku

  - **Data\_Doc\_UsedWrsDataOnOpen:bool –** istinito ako je datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka na glavnom računalu

  - **Data\_Doc\_WopiServiceId:string –** identifikator WOPI servisa, npr. „Dropbox“

  - **Data\_Doc\_AccessMode:long –** kako je dokument otvoren (samo za čitanje | čitanje i pisanje)

  - **Data\_DstDoc\_AssistedReadingReasons:long –** unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

  - **Data\_DstDoc\_ChunkingType:long –** kako je dokument pohranjen u sustavu SharePoint

  - **Data\_DstDoc\_EdpState:long –** stanje dokumenta s obzirom na zaštitu korporativnih podataka

  - **Data\_DstDoc\_Ext:string –** nastavak dokumenta

  - **Data\_DstDoc\_Extension:string –** nastavak dokumenta

  - **Data\_DstDoc\_FileFormat:long –** unaprijed definirani skup vrijednosti oblika datoteke (precizniji od nastavka)

  - **Data\_DstDoc\_Fqdn:string –** mjesto pohrane dokumenta (SharePoint.com, live.net), dostupno samo za domene sustava Office 365

  - **Data\_DstDoc\_FqdnHash:string –** raspršivanje mjesta pohrane dokumenta

  - **Data\_DstDoc\_IdentityTelemetryId:string –** jedinstveni GUID korisnika

  - **Data\_DstDoc\_IdentityUniqueId:string –** jedinstveni identifikator identiteta korišten za akciju zajedničkih dokumenata

  - **Data\_DstDoc\_IOFlags:long –** bit-maska za razne zastavice vezane uz ulaz i izlaz za određeni dokument

  - **Data\_DstDoc\_IrmRights:long –** unaprijed definirani skup vrijednosti za vrstu informacija koju upravljanje pravima primjenjuje na ovom dokumentu (proslijedi, odgovori, SecureReader, uređivanje itd.)

  - **Data\_DstDoc\_IsCloudCollabEnabled:bool –** istinito ako je HTTP zaglavlje „IsCloudCollabEnabled“ već prihvaćeno iz zahtjeva MOGUĆNOSTI.

  - **Data\_DstDoc\_IsIncrementalOpen:bool –** je li dokument otvoren inkrementalno (nova značajka koja otvara dokument bez potrebe za preuzimanjem cijelog dokumenta)

  - **Data\_DstDoc\_IsOcsSupported:bool –** podržava li dokument suautorstvo pomoću novog servisa OCS

  - **Data\_DstDoc\_IsOpeningOfflineCopy:bool –** provjerava otvara li se dokument iz lokalne predmemorije

  - **Data\_DstDoc\_IsSyncBacked:bool –** otvara li se dokument iz mape koja koristi aplikaciju OneDrive za povratnu sinkronizaciju

  - **Data\_DstDoc\_Location:long –** unaprijed definiran skup vrijednosti mjesta na kojima se dokument pohranjuje (lokalno, SharePoint, WOPI, mreža itd.)

  - **Data\_DstDoc\_LocationDetails:long –** unaprijed definiran skup vrijednosti detaljnijih lokacija (mapa Temp, mapa preuzimanja, dokumenti servisa One Drive, slike servisa One Drive itd.)

  - **Data\_DstDoc\_NumberCoAuthors:long –** broj suautora prilikom otvaranja dokumenta

  - **Data\_DstDoc\_PasswordFlags:long –** unaprijed definirani skup vrijednosti načina na koji je dokument šifriran pomoću lozinke (nema, lozinka za čitanje, lozinka za uređivanje)

  - **Data\_DstDoc\_ReadOnlyReasons:long –** unaprijed definirani skup vrijednosti koji naznačuje zašto je dokument označen samo za čitanje (zaključan na poslužitelju, konačni dokument, zaštićen lozinkom za uređivanje itd.)

  - **Data\_DstDoc\_ResourceIdHash:string –** raspršivanje identifikatora resursa za dokumente pohranjene u oblaku

  - **Data\_DstDoc\_ServerDocId:string –** nepromjenjivi identifikator za dokumente pohranjene u oblaku

  - **Data\_DstDoc\_ServerProtocol:long –** unaprijed definirani skup vrijednosti o protokolu koji se koristi za komuniciranje s poslužiteljem (Http, Cobalt, WOPI itd.)

  - **Data\_DstDoc\_ServerType:long –** unaprijed definirani skup vrijednosti o vrsti poslužitelja (SharePoint, DropBox, WOPI)

  - **Data\_DstDoc\_ServerVersion:long –** provjerava temelji li se poslužitelj na sustavu Office14, Office15 ili Office 16

  - **Data\_DstDoc\_SessionId:long –** generirani GUID koji identificira instancu dokumenta u sklopu iste sesije procesa

  - **Data\_DstDoc\_SharePointServiceContext:string –** neprozirni niz, obično GridManagerID.FarmID. Korisno za korelaciju klijentskih i poslužiteljskih zapisnika

  - **Data\_DstDoc\_SizeInBytes:long –** veličina dokumenta u bajtovima

  - **Data\_DstDoc\_SpecialChars:long –** bit-maska koja pokazuje posebne znakove u URL-u ili putu dokumenta

  - **Data\_DstDoc\_StorageProviderId:string –** niz koji određuje davatelja pohrane dokumenta, primjerice „DropBox“

  - **Data\_DstDoc\_StreamAvailability:long –** unaprijed definirani skup vrijednosti statusa toka dokumenta (dostupno, trajno onemogućeno, nije dostupno)

  - **Data\_DstDoc\_UrlHash:string –** raspršivanje punog URL-a dokumenata pohranjenih u oblaku

  - **Data\_DstDoc\_UsedWrsDataOnOpen:bool –** istinito ako je datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka na glavnom računalu

  - **Data\_DstDoc\_WopiServiceId:string –** identifikator WOPI servisa, npr. „Dropbox“

  - **Data\_FileType:long –** unaprijed definirani skup vrijednosti interne vrste datoteke

  - **Data\_fLifeguarded:bool –** je li dokument ikad popravljen pomoću značajke lifeguard (značajka za popravljanje pogrešaka dokumenta bez slanja upita korisniku)?

  - **Data\_SaveReason:long –** unaprijed definirani skup vrijednosti koji označava zašto je izvršeno spremanje? (AutoSave, ToOCSTransitionSave, ToCSITransitionSave itd.)

  - **Data\_SaveType:long –** unaprijed definirani skup vrijednosti o vrsti spremanja (SaveAs, Publish, Manual, OMSave itd.)

  - **Data\_SrcDoc\_AccessMode:long –** kako je dokument otvoren (samo za čitanje | čitanje i pisanje)

  - **Data\_SrcDoc\_AssistedReadingReasons:long –** unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

  - **Data\_SrcDoc\_ChunkingType:long –** kako je dokument pohranjen u sustavu SharePoint

  - **Data\_SrcDoc\_EdpState:long –** stanje dokumenta s obzirom na zaštitu korporativnih podataka

  - **Data\_SrcDoc\_Ext:string –** nastavak dokumenta

  - **Data\_SrcDoc\_Extension:string –** nastavak dokumenta

  - **Data\_SrcDoc\_FileFormat:long –** unaprijed definirani skup vrijednosti oblika datoteke (precizniji od nastavka)

  - **Data\_SrcDoc\_Fqdn:string –** mjesto pohrane dokumenta (SharePoint.com, live.net), dostupno samo za domene sustava Office 365

  - **Data\_SrcDoc\_FqdnHash:string –** raspršivanje mjesta pohrane dokumenta

  - **Data\_SrcDoc\_IdentityTelemetryId:string –** jedinstveni GUID korisnika

  - **Data\_SrcDoc\_IdentityUniqueId:string –** jedinstveni identifikator identiteta korišten za akciju zajedničkih dokumenata

  - **Data\_SrcDoc\_IOFlags:long –** bit-maska za razne zastavice vezane uz ulaz i izlaz za određeni dokument

  - **Data\_SrcDoc\_IrmRights:long –** unaprijed definirani skup vrijednosti za vrstu informacija koju upravljanje pravima primjenjuje na ovom dokumentu (proslijedi, odgovori, SecureReader, uređivanje itd.)

  - **Data\_SrcDoc\_IsCloudCollabEnabled:bool –** istinito ako je HTTP zaglavlje „IsCloudCollabEnabled“ već prihvaćeno iz zahtjeva MOGUĆNOSTI.

  - **Data\_SrcDoc\_IsIncrementalOpen:bool –** je li dokument otvoren inkrementalno (nova značajka koja otvara dokument bez potrebe za preuzimanjem cijelog dokumenta)

  - **Data\_SrcDoc\_IsOcsSupported:bool –** podržava li dokument suautorstvo pomoću novog servisa OCS

  - **Data\_SrcDoc\_IsOpeningOfflineCopy:bool –** provjerava otvara li se dokument iz lokalne predmemorije

  - **Data\_SrcDoc\_IsSyncBacked:bool –** otvara li se dokument iz mape koja koristi aplikaciju OneDrive za povratnu sinkronizaciju

  - **Data\_SrcDoc\_Location:long –** unaprijed definiran skup vrijednosti mjesta na kojima se dokument pohranjuje (lokalno, SharePoint, WOPI, mreža itd.)

  - **Data\_SrcDoc\_LocationDetails:long –** unaprijed definiran skup vrijednosti detaljnijih lokacija (mapa Temp, mapa preuzimanja, dokumenti servisa One Drive, slike servisa One Drive itd.)

  - **Data\_SrcDoc\_NumberCoAuthors:long –** broj suautora prilikom otvaranja dokumenta

  - **Data\_SrcDoc\_PasswordFlags:long –** unaprijed definirani skup vrijednosti načina na koji je dokument šifriran pomoću lozinke (nema, lozinka za čitanje, lozinka za uređivanje)

  - **Data\_SrcDoc\_ReadOnlyReasons:long –** unaprijed definirani skup vrijednosti koji naznačuje zašto je dokument označen samo za čitanje (zaključan na poslužitelju, konačni dokument, zaštićen lozinkom za uređivanje itd.)

  - **Data\_SrcDoc\_ResourceIdHash:string –** raspršivanje identifikatora resursa za dokumente pohranjene u oblaku

  - **Data\_SrcDoc\_ServerDocId:string –** nepromjenjivi identifikator za dokumente pohranjene u oblaku

  - **Data\_SrcDoc\_ServerProtocol:long –** unaprijed definirani skup vrijednosti o protokolu koji se koristi za komuniciranje s poslužiteljem (Http, Cobalt, WOPI itd.)

  - **Data\_SrcDoc\_ServerType:long –** unaprijed definirani skup vrijednosti o vrsti poslužitelja (SharePoint, DropBox, WOPI)

  - **Data\_SrcDoc\_ServerVersion:long –** provjerava temelji li se poslužitelj na sustavu Office14, Office15 ili Office 16

  - **Data\_SrcDoc\_SessionId:long –** generirani GUID koji identificira instancu dokumenta u sklopu iste sesije procesa

  - **Data\_SrcDoc\_SharePointServiceContext:string –** neprozirni niz, obično GridManagerID.FarmID. Korisno za korelaciju klijentskih i poslužiteljskih zapisnika

  - **Data\_SrcDoc\_SizeInBytes:long –** veličina dokumenta u bajtovima

  - **Data\_SrcDoc\_SpecialChars:long –** bit-maska koja pokazuje posebne znakove u URL-u ili putu dokumenta

  - **Data\_SrcDoc\_StorageProviderId:string –** niz koji određuje davatelja pohrane dokumenta, primjerice „DropBox“

  - **Data\_SrcDoc\_StreamAvailability:long –** unaprijed definirani skup vrijednosti statusa toka dokumenta (dostupno, trajno onemogućeno, nije dostupno)

  - **Data\_SrcDoc\_UrlHash:string –** raspršivanje punog URL-a dokumenata pohranjenih u oblaku

  - **Data\_SrcDoc\_UsedWrsDataOnOpen:bool –** istinito ako je datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka na glavnom računalu

  - **Data\_SrcDoc\_WopiServiceId:string –** identifikator WOPI servisa, npr. „Dropbox“

  - **Data\_StopwatchDuration:long –** ukupno vrijeme za aktivnost

  - **Data\_TypeOfSaveDialog:long –** unaprijed definirani skup vrijednosti dijaloškog okvira (RUN\_SAVEAS\_DLG, RUN\_SAVEMEDIA\_DLG, RUN\_SAVEAS\_VIDEO\_DLG etd.)

  - **Doc –** trenutni dokument za spremanje

  - **DstDoc –** nova lokacija dokumenta (u slučaju SaveAs)

  - **DstDoc –** izvorna lokacija dokumenta (u slučaju SaveAs)

#### <a name="officepowerpointpptsharedslideshowfailure"></a>Office.PowerPoint.PPT.Shared.SlideShow.Failure

Prikupljanje pogrešaka tijekom dijaprojekcije. Dijaprojekcija je ključna značajka u programu PowerPoint. Microsoft prikuplja kada se poruka pojavljuje tijekom dijaprojekcije za poboljšanje korisničkog iskustva na dijaprojekciji. Microsoft koristi te podatke da bi dobio dijagnostičke informacije o mjestu pogreške dok korisnik koristi dijaprojekciju

Prikupljaju se sljedeća polja:

  - **CountSlideShowErrors** – ukupan broj pogrešaka dijaprojekcije

  - **CountPPTErrors** – ukupan broj PPT pogrešaka

  - **CountOArtErrors** – ukupan broj OArt pogrešaka

  - **CountOtherErrors** – ukupan broj drugih pogrešaka

  - **FirstSlideShowError** – prva pogreška dogodila se u dijaprojekciji

  - **FirstOArtError** – prva pogreška dogodila se u OArt-u

  - **FirstPPTError** – prva pogreška dogodila se u PPT-u

  - **FirstOtherError** – prva pogreška dogodila se u drugom području

#### <a name="officeprojectprojectfilesave"></a>Office.Project.ProjectFileSave

Project sprema datoteku. Taj događaj označava spremanje u programu Project. Omogućuje Microsoftu mjerenje uspjeha spremanja datoteke programa Project što je važno za sprječavanje gubitka podataka dokumenta.

Prikupljaju se sljedeća polja:

  - **Data\_TriggerTime** – vrijeme spremanja

  - **Data\_FileType** – vrsta datoteke u koju se sprema projekt
 
#### <a name="officesessionactivitystart"></a>Office.Session.Activity.Start

Omogućuje nam da znamo kada je pokrenuta sesija dodatka Data streamer.  Koristi se za stanje i nadzor značajke. Taj je događaj generirao dodatak Microsoft Data Streamer za Excel.

Prikupljaju se sljedeća polja:

- **Activity_Name** – naziv aktivnosti „Sesija“

- **Activity_CV** – ID za povezivanje događaja u sesiji povezivanja

- **Activity_StartStopType** – početak

- **Activity_DateTimeTicks** – vrijeme podataka za aktivnost

#### <a name="officesessionactivitystop"></a>Office.Session.Activity.Stop

Omogućuje nam da znamo kada je sesija dodatka Data streamer zaustavljena. Koristi se za stanje i nadzor značajke. Taj je događaj generirao dodatak Microsoft Data Streamer za Excel.

Prikupljaju se sljedeća polja:

- **Activity_Name** – naziv aktivnosti „Sesija“

- **Activity_CV** – ID za povezivanje događaja u sesiji povezivanja

- **Activity_StartStopType** – zaustavljanje

- **Activity_DateTimeTicks** – vrijeme podataka za aktivnost

#### <a name="officestreamdeviceactivitystart"></a>Office.StreamDevice.Activity.Start

Omogućuje nam da znamo je li početak strujanja izvora podataka uspješan.   Koristi se za stanje i nadzor značajke. Taj je događaj generirao dodatak Microsoft Data Streamer za Excel.

Prikupljaju se sljedeća polja:

- **Datasource_Type** – informacije o serijskom uređaju ili servisu aplikacije

- **DataSource_Name** – naziv povezanog izvora podataka

- **Activity_Name** – naziv aktivnosti „StreamDeviceData“ ili „StreamFileData“

- **Activity_CV** – ID za povezivanje događaja u sesiji povezivanja

- **Activity_StartStopType** – početak

- **Activity_DateTimeTicks** – vrijeme podataka za aktivnost

#### <a name="officestreamdeviceactivitystop"></a>Office.StreamDevice.Activity.Stop

Omogućuje nam da znamo je li zaustavljanje strujanja izvora podataka uspješno.   Koristi se za stanje i nadzor značajke. Taj je događaj generirao dodatak Microsoft Data Streamer za Excel.

Prikupljaju se sljedeća polja:

- **Datasource_Type** – informacije o serijskom uređaju ili servisu aplikacije

- **DataSource_Name** – naziv povezanog izvora podataka

- **Activity_Name** – naziv aktivnosti „StreamDeviceData“ ili „StreamFileData“

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

  - **Data.actionSource –** kako je pokrenut prijevod odabira

  - **Data.bodyBackgroundColor –** pozadinska boja spremnika teme sustava Office

  - **Data.bodyForegroundColor –** boja prednjeg plana spremnika teme sustava Office

  - **Data.browserLang –** trenutni jezik prikaza preglednika

  - **Data.browserOnline –** zastarjelo

  - **Data.browserPlatform –** platforma preglednika

  - **Data.browserUserAgent –** korisnički agent preglednika

  - **Data.colorDepth –** dubina boje sustava

  - **Data.contentLanguage –** otkriveni jezik sadržaja za prijevod

  - **Data.controlBackgroundColor –** pozadinska boja kontrole teme sustava Office

  - **Data.controlForegroundColor –** boja prednjeg plana kontrole teme sustava Office

  - **Data.correlationId –** jedinstveni identifikator zahtjeva poslanog servisu

  - **Data.crossSessionId –** jedinstveni identifikator korisnika

  - **Data.crossSessionStartTime –** vremenska oznaka UTC-a kada se pokrene sesija prijevoda

  - **Data.currentTime –** vremenska oznaka UTC-a kada se pošalje ova telemetrijska poruka

  - **Data.displayLanguage –** jezik prikaza sustava Office

  - **Data.documentSourceLang –** jezik sadržaja dokumenta

  - **Data.documentTargetLang –** jezik na koji će dokument biti preveden

  - **Data.environment –** okruženje servisa kojem je zahtjev poslan

  - **Data.errorMessage –** poruka o pogrešci koju je servis prijavio

  - **Data.eventActionType –** vrsta telemetrijskog događaja

  - **Data.eventTagId –** jedinstveni identifikator retka koda koji je stvorio ovu telemetrijsku poruku

  - **Data.flights–** omogućene međuverzije

  - **Data.fileSize –** veličina datoteke programa Word za prijevod

  - **Data.fileSource –** gdje je hostirana datoteka programa Word (izvanmrežno, na mreži)

  - **Data.fileType –** nastavak datoteke programa Word

  - **Data.innerHeight"–** visina spremnika bočnog okna

  - **Data.innerWidth"–** širina spremnika bočnog okna

  - **Data.lookupSourceLang–** ne koristi se za prijevod dokumenta

  - **Data.lookupTargetLang–** ne koristi se za prijevod dokumenta

  - **Data.officeHost–** aplikacija sustava Office koja hostira bočno okno

  - **Data.officeLocale–** jezik korisnika sustava Office

  - **Data.officeMachineId–** jedinstveni identifikator uređaja

  - **Data.officePlatform –** platforma uređaja

  - **Data.officeSessionId –** identifikator sesije sustava Office

  - **Data.officeUserId –** jedinstveni identifikator korisnika sustava Office

  - **Data.officeVersion –** verzija sustava Office

  - **Data.pageXOffset –** položaj vodoravnog klizača u bočnom oknu s lijeve strane okna

  - **Data.pageYOffset –** položaj okomitog klizača u bočnom oknu s gornje strane okna

  - **Data.pixelDepth –** razlučivost boje zaslona

  - **Data.responseCode –** kod odgovora na zahtjev iz servisa

  - **Data.responseTime –** proteklo vrijeme zahtjeva

  - **Data.resultType –** rezultat zahtjeva

  - **Data.screenHeight –** visina zaslona u pikselima

  - **Data.screenLeft –** vodoravna koordinata prozora u odnosu prema zaslonu

  - **Data.screenTop –** okomita koordinata prozora u odnosu prema zaslonu

  - **Data.screenWidth –** širina zaslona u pikselima

  - **Data.selectedTab –** koja je kartica odabrana, Odabir ili Dokument

  - **Data.serverUrl –** URL servisa za prevođenje

  - **Data.sessionId –** identifikator sesije u bočnom oknu

  - **Data.sessionStartTime –** vremenska oznaka UTC-a kada se pokrene sesija prijevoda

  - **Data.sourceTextHash –** raspršivanje teksta za prijevod

  - **Data.sourceTextLength –** duljina teksta za prijevod

  - **Data.sourceTextWords –** broj riječi u tekstu za prijevod

  - **Data.warningMessage –** poruka s upozorenjem koju je prijavio servis

#### <a name="officetranslatortexttranslated"></a>Office.Translator.TextTranslated

Prikuplja uspjeh ili neuspjeh prijevoda odabira koji korisnik pokreće u servisu Translator SDX. To je vrlo važno zbog procjene stanja značajke prijevoda i reagiranja na kvarove koji se mogu dogoditi. Koristi se za praćenje stanja scenarija „Prijevod odabira“ u programima Excel, PowerPoint i Word.

Prikupljaju se sljedeća polja:

  - **Data.actionSource –** kako je pokrenut prijevod odabira

  - **Data.bodyBackgroundColor –** pozadinska boja spremnika teme sustava Office

  - **Data.bodyForegroundColor –** boja prednjeg plana spremnika teme sustava Office

  - **Data.browserLang –** trenutni jezik prikaza preglednika

  - **Data.browserOnline –** zastarjelo

  - **Data.browserPlatform –** platforma preglednika

  - **Data.browserUserAgent –** korisnički agent preglednika

  - **Data.colorDepth –** dubina boje sustava

  - **Data.contentLanguage –** otkriveni jezik sadržaja za prijevod

  - **Data.controlBackgroundColor –** pozadinska boja kontrole teme sustava Office

  - **Data.controlForegroundColor –** boja prednjeg plana kontrole teme sustava Office

  - **Data.correlationId –** jedinstveni identifikator zahtjeva poslanog servisu

  - **Data.crossSessionId –** jedinstveni identifikator korisnika

  - **Data.crossSessionStartTime –** vremenska oznaka UTC-a kada se pokrene sesija prijevoda

  - **Data.currentTime –** vremenska oznaka UTC-a kada se pošalje ova telemetrijska poruka

  - **Data.displayLanguage –** jezik prikaza sustava Office

  - **Data.documentSourceLang –** ne koristi se za odabir

  - **Data.documentTargetLang –** ne koristi se za odabir prijevoda

  - **Data.environment –** okruženje servisa kojem je zahtjev poslan

  - **Data.errorMessage –** poruka o pogrešci koju je servis prijavio

  - **Data.eventActionType –** vrsta telemetrijskog događaja

  - **Data.eventTagId –** jedinstveni identifikator retka koda koji je stvorio ovu telemetrijsku poruku

  - **Data.flights–** omogućene međuverzije

  - **Data.innerHeight"–** visina spremnika bočnog okna

  - **Data.innerWidth"–** širina spremnika bočnog okna

  - **Data.lookupSourceLang–** jezik trenutno odabranog teksta

  - **Data.lookupTargetLang–** jezik na koji će trenutno odabrani tekst biti preveden

  - **Data.officeHost–** aplikacija sustava Office koja hostira bočno okno

  - **Data.officeLocale–** jezik korisnika sustava Office

  - **Data.officeMachineId–** jedinstveni identifikator uređaja

  - **Data.officePlatform –** platforma uređaja

  - **Data.officeSessionId –** identifikator sesije sustava Office

  - **Data.officeUserId –** jedinstveni identifikator korisnika sustava Office

  - **Data.officeVersion –** verzija sustava Office

  - **Data.pageXOffset –** položaj vodoravnog klizača u bočnom oknu s lijeve strane okna

  - **Data.pageYOffset –** položaj okomitog klizača u bočnom oknu s gornje strane okna

  - **Data.pixelDepth –** razlučivost boje zaslona

  - **Data.responseCode –** kod odgovora na zahtjev iz servisa

  - **Data.responseTime –** proteklo vrijeme zahtjeva

  - **Data.resultType –** rezultat zahtjeva

  - **Data.screenHeight –** visina zaslona u pikselima

  - **Data.screenLeft –** vodoravna koordinata prozora u odnosu prema zaslonu

  - **Data.screenTop –** okomita koordinata prozora u odnosu prema zaslonu

  - **Data.screenWidth –** širina zaslona u pikselima

  - **Data.selectedTab –** koja je kartica odabrana, Odabir ili Dokument

  - **Data.serverUrl –** URL servisa za prevođenje

  - **Data.sessionId –** identifikator sesije u bočnom oknu

  - **Data.sessionStartTime –** vremenska oznaka UTC-a kada se pokrene sesija prijevoda

  - **Data.sourceTextHash –** raspršivanje teksta za prijevod

  - **Data.sourceTextLength –** duljina teksta za prijevod

  - **Data.sourceTextWords –** broj riječi u tekstu za prijevod

  - **Data.warningMessage –** poruka s upozorenjem koju je prijavio servis

#### <a name="officewordexperimentationdocumentstatsoncloseandsuspend"></a>Office.Word.Experimentation.DocumentStatsOnCloseAndSuspend

Taj događaj zapisuje statistiku dokumenta za svaki dokument kada je Office Word zatvoren ili obustavljen.

Događaj se koristi za povezivanja uređivanja, veličine itd. dokumenta sa spremanjem dokumenta, zajedničkim korištenjem dokumenta i pogreškama mrežne suradnje na dokumentu.

Prikupljaju se sljedeća polja:

  - **Data\_BkmkRefCount –** broj referenci knjižnih oznaka u dokumentu

  - **Data\_CharacterCount –** broj znakova u dokumentu

  - **Data\_CharactersWithSpaceCount –** broj znakova i razmaka u dokumentu

  - **Data\_ChartCount –** broj grafikona u dokumentu

  - **Data\_CitationCount –** broj navoda u dokumentu

  - **Data\_DocumentLocation –** označava koji je servis dobavio dokument (OneDrive, File Server, SharePoint itd.)

  - **Data\_ETW\_TrackbackTag –** označava mjesto u kodu iz kojeg je taj događaj pokrenut (Zatvori ili Obustavi)

  - **Data\_EndnoteDocCount –** broj krajnjih bilješki u dokumentu

  - **Data\_FootnoteDocCount –** broj fusnota u dokumentu

  - **Data\_HasBibliography –** označava sadrži li dokument bibliografiju

  - **Data\_HasHeader –** označava sadrži li dokument zaglavlje

  - **Data\_IsImeUsed –** označava je li uređivač načina unosa korišten u dokumentu

  - **Data\_IsPageCountInProgress –** označava je li brojanje stranica trenutno u tijeku za dokument.

  - **Data\_IsTouchUsed –** označava je li unos dodirom korišten u dokumentu

  - **Data\_IsTrackChangesOn –** označava je li evidentiranje promjena uključeno u dokumentu

  - **Data\_LineCount –** broj redaka u dokumentu

  - **Data\_MainPdod –** identifikator dokumenta u sklopu procesa Office Word.

  - **Data\_PageCount –** broj stranica u dokumentu

  - **Data\_PageNumberFieldCount –** broj polja za broj stranice u dokumentu

  - **Data\_ParagraphCount –** broj odlomaka u dokumentu

  - **Data\_PicCount –** broj slika u dokumentu

  - **Data\_RsidCount –** broj identifikatora spremanja revizija u dokumentu

  - **Data\_TocCount –** broj tablica sadržaja u dokumentu

  - **Data\_UrlHash –** jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta

  - **Data\_UserActionID –** ovo polje podataka ne koristi se (vrijednost je uvijek 0)

  - **Data\_UserActionName –** uvijek „DocumentStatsOnCloseAndSuspend“

  - **Data\_UserInteractionTimeMsec –** broj milisekundi koji je korisnik aktivno radio s dokumentom

  - **Data\_WordCount –** broj riječi u dokumentu

#### <a name="officewordfilenewcreatenewfile"></a>Office.Word.FileNew.CreateNewFile

Taj događaj označava da je novi dokument stvoren u programu Office Word i prati uspjeh ili neuspjeh operacije. Događaj se koristi za praćenje radi li stvaranje novog dokumenta prema očekivanjima. Koristi se i za izračunavanje broja mjesečnih aktivnih korisnika/uređaja i metriku pouzdanosti oblaka.

Prikupljaju se sljedeća polja:

  - **Data\_DirtyState** – je li dokument stvoren u prljavom stanju (s promjenama koje treba spremiti)

  - **Data\_ErrorID** – identifikator pogreške u slučaju pogreške operacije

  - **Data\_MainPdod –** identifikator dokumenta tijekom ove sesije postupka

  - **Data\_UsesCustomTemplate** – označava je li dokument stvoren iz prilagođenog predloška

#### <a name="officewordfilesaveactcmdgosubsaveas"></a>Office.Word.FileSave.ActCmdGosubSaveAs

Taj događaj označava da korisnik sprema promjene u novom dokumentu. Događaj nadzire funkcionira li spremanje u novom dokumentu prema očekivanjima. Koristi se i za izračunavanje broja mjesečnih aktivnih korisnika/uređaja i metriku pouzdanosti oblaka.

Prikupljaju se sljedeća polja:

  - **Data\_AddDocTelemRes –** izvješćuje jesmo li mogli pravilno popuniti ostale vrijednosti vezane uz telemetriju dokumenta u sklopu događaja. Koristi se za dijagnostiku kvalitete podataka.

  - **Data\_DetachedDuration –** koliko je dugo aktivnost bila odvojena od niti

  - **Data\_Doc\_AccessMode –** dokument je samo za čitanje ili za uređivanje

  - **Data\_Doc\_AssistedReadingReasons –** unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

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

  - **Data_Doc_IsRtcAlwaysOn –** istinito ako je kanal u stvarnom vremenu (RTC) uvijek uključen za ovu datoteku.

  - **Data\_Doc\_IsSyncBacked –** zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

  - **Data\_Doc\_Location –** označava koji je servis dobavio dokument (OneDrive, File Server, SharePoint itd.)

  - **Data\_Doc\_LocationDetails –** označava koja je poznata mapa dobavila lokalno pohranjeni dokument

  - **Data\_Doc\_NumberCoAuthors –** broj drugih korisnika u sesiji zajedničkog uređivanja

  - **Data\_Doc\_PasswordFlags –** označava postavljene zastavice za čitanje ili čitanje i pisanje lozinke

  - **Data\_Doc\_ReadOnlyReasons –** razlozi zbog kojih je dokument otvoren samo za čitanje

  - **Data\_Doc\_ResourceIdHash –** anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

  - **Data\_Doc\_ServerDocId –** nepromjenjivi anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

  - **Data\_Doc\_ServerProtocol –** verzija protokola korištena za komuniciranje sa servisom

  - **Data\_Doc\_ServerType –** vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.)

  - **Data\_Doc\_ServerVersion –** verzija poslužitelja koji pruža servis

  - **Data\_Doc\_SessionId –** identificira specifičnu sesiju uređivanja dokumenta u sklopu cijele sesije

  - **Data\_Doc\_SharePointServiceContext –** dijagnostičke informacije iz zahtjeva sustava SharePoint Online

  - **Data\_Doc\_SizeInBytes –** pokazatelj veličine dokumenta

  - **Data\_Doc\_SpecialChars –** pokazatelj posebnih znakova u URL–u ili putu dokumenta

  - **Data\_Doc\_StreamAvailability –** pokazatelj je li tok dokumenta dostupan/onemogućen

  - **Data\_Doc\_SyncBackedType –** pokazatelj vrste dokumenta (lokalni ili na servisu)

  - **Data\_Doc\_UrlHash –** jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta

  - **Data\_EditorDisablingRename –** identifikator prvog uređivača koji je uzrokovao onemogućivanje preimenovanja

  - **Data\_EditorsCount –** broj uređivača dokumenta

  - **Data\_LastLoggedTag –** jedinstvena oznaka mjesta pozivanja koda, koja se koristi za identifikaciju dvokratnog neuspjelog pokušaja spremanja (koristi se za dijagnostiku kvalitete podataka)

  - **Data\_MoveDisabledReason –** pogreška koja onemogućuje premještanje dokumenta

  - **Data\_MoveFlightEnabled –** je li omogućena testna verzija za značajku premještanja

  - **Data\_RenameDisabledReason –** pogreška koja uzrokuje onemogućivanje preimenovanja za dokument

  - **Data\_RenameFlightEnabled –** je li omogućena testna verzija za značajku preimenovanja

#### <a name="officewordfilesaveactfconfirmsavedoccoreautorecoverysave"></a>Office.Word.FileSave.ActFConfirmSaveDocCoreAutoRecoverySave

Taj događaj označava da Office Word sprema automatski oporavljeni dokument koji još nije bio spremljen. On Microsoftu omogućuje otkrivanje pogrešaka s automatskim oporavkom, što je važno za zaštitu podataka dokumenta.

Događaj nadzire funkcionira li spremanje automatskog oporavka prema očekivanjima. Koristi se i za izračunavanje broja mjesečnih aktivnih korisnika/uređaja i metriku pouzdanosti oblaka.

Prikupljaju se sljedeća polja:

  - **Data\_DetachedDuration –** koliko je dugo aktivnost bila odvojena od niti

  - **Data\_Doc\_AccessMode –** dokument je samo za čitanje ili za uređivanje

  - **Data\_Doc\_AssistedReadingReasons –** unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

  - **Data\_Doc\_ChunkingType –** jedinice korištene za inkrementalno otvaranje dokumenta

  - **Data\_Doc\_EdpState –** postavka zaštite elektroničkih podataka za dokument

  - **Data\_Doc\_Ext –** nastavak dokumenta (docx/xlsb/pptx itd.)

  - **Data\_Doc\_FileFormat –** verzija protokola za oblik datoteke

  - **Data\_Doc\_Fqdn –** naziv domene servisa OneDrive ili sustava SharePoint Online

  - **Data\_Doc\_FqdnHash –** jednosmjerno raspršivanje naziva domene koji identificira korisnika

  - **Data\_Doc\_IdentityTelemetryId –** jednosmjerno raspršivanje korisničkog identiteta koji se koristio za otvaranje

  - **Data\_Doc\_InitializationScenario –** bilježi način otvaranja dokumenta

  - **Data\_Doc\_IOFlags –** izvješćuje o predmemoriranim zastavicama korištenima za postavljanje mogućnosti otvorenog zahtjeva

  - **Data\_Doc\_IrmRights –** radnje dopuštene pravilima zaštite elektroničkih podataka primijenjenima na dokument/korisnika

  - **Data\_Doc\_IsIncrementalOpen –** zastavica koja označava da je dokument inkrementalno otvoren

  - **Data\_Doc\_IsOcsSupported –** zastavica koja označava da je dokument podržan u servisu za suradnju

  - **Data\_Doc\_IsOpeningOfflineCopy –** zastavica koja označava da je otvorena izvanmrežna kopija dokumenta

  - **Data_Doc_IsRtcAlwaysOn –** istinito ako je kanal u stvarnom vremenu (RTC) uvijek uključen za ovu datoteku.

  - **Data\_Doc\_IsSyncBacked –** zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

  - **Data\_Doc\_Location –** označava koji je servis dobavio dokument (OneDrive, File Server, SharePoint itd.)

  - **Data\_Doc\_LocationDetails –** označava koja je poznata mapa dobavila lokalno pohranjeni dokument

  - **Data\_Doc\_NumberCoAuthors –** broj drugih korisnika u sesiji zajedničkog uređivanja

  - **Data\_Doc\_PasswordFlags –** označava postavljene zastavice za čitanje ili čitanje i pisanje lozinke

  - **Data\_Doc\_ReadOnlyReasons –** razlozi zbog kojih je dokument otvoren samo za čitanje

  - **Data\_Doc\_ResourceIdHash –** anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

  - **Data\_Doc\_ServerDocId –** nepromjenjivi anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

  - **Data\_Doc\_ServerProtocol –** verzija protokola korištena za komuniciranje sa servisom

  - **Data\_Doc\_ServerType –** vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.)

  - **Data\_Doc\_ServerVersion –** verzija poslužitelja koji pruža servis

  - **Data\_Doc\_SessionId –** identificira specifičnu sesiju uređivanja dokumenta u sklopu cijele sesije

  - **Data\_Doc\_SharePointServiceContext –** dijagnostičke informacije iz zahtjeva sustava SharePoint Online

  - **Data\_Doc\_SizeInBytes –** pokazatelj veličine dokumenta

  - **Data\_Doc\_SpecialChars –** pokazatelj posebnih znakova u URL–u ili putu dokumenta

  - **Data\_Doc\_StreamAvailability –** pokazatelj je li tok dokumenta dostupan/onemogućen

  - **Data\_Doc\_SyncBackedType –** pokazatelj vrste dokumenta (lokalni ili na servisu)

  - **Data\_Doc\_UrlHash –** jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta

  - **Data\_Doc\_WopiServiceId –** sadrži jedinstveni identifikator davatelja usluge WOPI

  - **Data\_FailureClass –** cijeli broj koji predstavlja klasu neuspjeha za neuspjehe tranzicije servisa Office Collaboration Services (OCS)

  - **Data\_MainPdod –** identifikator dokumenta u sklopu procesa Office Word.

  - **Data\_MoveFlightEnabled –** je li omogućena testna verzija za značajku premještanja

  - **Data\_OCSSyncbackSaveStarted –** zastavica koja označava da je to spremanje povezano sa spremanjem radi povratne sinkronizacije

  - **Data\_RenameDisabledReason –** pogreška koja uzrokuje onemogućivanje preimenovanja za taj dokument

  - **Data\_RenameFlightEnabled –** je li omogućena testna verzija za značajku preimenovanja

  - **Data\_SaveInitiateKind –** cijeli broj koji označava kako je pokrenuto spremanje

  - **Data\_SrcDocIsUnnamedOrNew –** označava je li dokument koji spremamo nov

#### <a name="officewordfilesaveactfconfirmsavedoccorequerysave"></a>Office.Word.FileSave.ActFConfirmSaveDocCoreQuerySave

Taj događaj označava da Office Word traži od korisnika da spremi promjene kada pokuša zatvoriti dokument. To omogućuje Microsoftu praćenje radi li spremanje pri zatvaranju prema očekivanjima kako bi se spriječio gubitak podataka. Događaj nadzire funkcionira li spremanje pri zatvaranju prema očekivanjima. Koristi se i za izračunavanje broja mjesečnih aktivnih korisnika/uređaja i metriku pouzdanosti oblaka.

Prikupljaju se sljedeća polja:

  - **Data\_AddDocTelemRes –** izvješćuje jesmo li mogli pravilno popuniti ostale vrijednosti vezane uz telemetriju dokumenta u sklopu događaja. Koristi se za dijagnostiku kvalitete podataka.

  - **Data\_DetachedDuration –** koliko je dugo aktivnost bila odvojena od niti

  - **Data\_Doc\_AccessMode –** dokument je samo za čitanje ili za uređivanje

  - **Data\_Doc\_AssistedReadingReasons –** unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

  - **Data\_Doc\_ChunkingType –** jedinice korištene za inkrementalno otvaranje dokumenta

  - **Data\_Doc\_EdpState –** postavka zaštite elektroničkih podataka za dokument

  - **Data\_Doc\_Ext –** nastavak dokumenta (docx/xlsb/pptx itd.)

  - **Data\_Doc\_FileFormat –** verzija protokola za oblik datoteke

  - **Data\_Doc\_Fqdn –** naziv domene servisa OneDrive ili sustava SharePoint Online

  - **Data\_Doc\_FqdnHash –** jednosmjerno raspršivanje naziva domene koji identificira korisnika

  - **Data\_Doc\_IdentityTelemetryId –** jednosmjerno raspršivanje korisničkog identiteta koji se koristio za otvaranje

  - **Data\_Doc\_InitializationScenario –** bilježi način otvaranja dokumenta

  - **Data\_Doc\_IOFlags –** izvješćuje o predmemoriranim zastavicama korištenima za postavljanje mogućnosti otvorenog zahtjeva

  - **Data\_Doc\_IrmRights –** radnje dopuštene pravilima zaštite elektroničkih podataka primijenjenima na dokument/korisnika

  - **Data\_Doc\_IsIncrementalOpen –** zastavica koja označava da je dokument inkrementalno otvoren

  - **Data\_Doc\_IsOcsSupported –** zastavica koja označava da je dokument podržan u servisu za suradnju

  - **Data\_Doc\_IsOpeningOfflineCopy –** zastavica koja označava da je otvorena izvanmrežna kopija dokumenta

  - **Data_Doc_IsRtcAlwaysOn –** istinito ako je kanal u stvarnom vremenu (RTC) uvijek uključen za ovu datoteku.

  - **Data\_Doc\_IsSyncBacked –** zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

  - **Data\_Doc\_Location –** označava koji je servis dobavio dokument (OneDrive, File Server, SharePoint itd.)

  - **Data\_Doc\_LocationDetails –** označava koja je poznata mapa dobavila lokalno pohranjeni dokument

  - **Data\_Doc\_NumberCoAuthors –** broj drugih korisnika u sesiji zajedničkog uređivanja

  - **Data\_Doc\_PasswordFlags –** označava postavljene zastavice za čitanje ili čitanje i pisanje lozinke

  - **Data\_Doc\_ReadOnlyReasons –** razlozi zbog kojih je dokument otvoren samo za čitanje

  - **Data\_Doc\_ResourceIdHash –** anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

  - **Data\_Doc\_ServerDocId –** nepromjenjivi anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

  - **Data\_Doc\_ServerProtocol –** verzija protokola korištena za komuniciranje sa servisom

  - **Data\_Doc\_ServerType –** vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.)

  - **Data\_Doc\_ServerVersion –** verzija poslužitelja koji pruža servis

  - **Data\_Doc\_SessionId –** identificira specifičnu sesiju uređivanja dokumenta u sklopu cijele sesije

  - **Data\_Doc\_SharePointServiceContext –** dijagnostičke informacije iz zahtjeva sustava SharePoint Online

  - **Data\_Doc\_SizeInBytes –** pokazatelj veličine dokumenta

  - **Data\_Doc\_SpecialChars –** pokazatelj posebnih znakova u URL–u ili putu dokumenta

  - **Data\_Doc\_StreamAvailability –** pokazatelj je li tok dokumenta dostupan/onemogućen

  - **Data\_Doc\_SyncBackedType –** pokazatelj vrste dokumenta (lokalni ili na servisu)

  - **Data\_Doc\_UrlHash –** jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta

  - **Data\_Doc\_WopiServiceId –** sadrži jedinstveni identifikator davatelja usluge WOPI

  - **Data\_DstDoc\_AccessMode –** odredišni je dokument samo za čitanje ili za uređivanje

  - **Data\_DstDoc\_EdpState – postavka zaštite elektroničkih podataka za odredišni dokument–**

  - **Data\_DstDoc\_Ext –** nastavak dokumenta (docx/xlsb/pptx itd.) za odredišni dokument

  - **Data\_DstDoc\_FileFormat –** verzija protokola za oblik datoteke za odredišni dokument

  - **Data\_DstDoc\_Location –** označava koji će servis pružiti pohranu odredišnog dokumenta (OneDrive, File Server, SharePoint itd.)

  - **Data\_DstDoc\_LocationDetails –** označava koja je lokalna poznata mapa pohranila odredišni dokument

  - **Data\_DstDoc\_SessionId –** identificira specifičnu sesiju uređivanja dokumenta u sklopu cijele sesije

  - **Data\_DstDoc\_UrlHash –** jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta za odredišni dokument

  - **Data\_FailureClass –** cijeli broj koji predstavlja klasu neuspjeha za neuspjehe OCS tranzicije

  - **Data\_LocationPickerSaveStatus –** cjelobrojna vrijednost koja označava akciju koja je aktivirala spremanje iz dijaloškog okvira za spremanje prilikom izlaska

  - **Data\_MainPdod –** identifikator dokumenta u sklopu procesa Office Word.

  - **Data\_MoveFlightEnabled –** je li omogućena testna verzija za značajku premještanja

  - **Data\_OCSSyncbackSaveStarted –** zastavica koja označava da je to spremanje povezano sa spremanjem radi povratne sinkronizacije

  - **Data\_RenameDisabledReason –** pogreška koja uzrokuje onemogućivanje preimenovanja za taj dokument

  - **Data\_RenameFlightEnabled –** je li omogućena testna verzija za značajku preimenovanja

  - **Data\_SaveInitiateKind –** cijeli broj koji označava kako je pokrenuto spremanje

  - **Data\_SrcDocIsUnnamedOrNew –** označava je li dokument koji spremamo nov

#### <a name="officewordfilesavesaveassavefile"></a>Office.Word.FileSave.SaveAsSaveFile

Taj događaj označava da Office Word sprema dokument u novi dokument. On Microsoftu omogućuje otkrivanje pogrešaka pri izvođenju naredbe Spremi kao, što je važno za izbjegavanje gubitka podataka iz dokumenta. Događaj nadzire funkcionira li naredba Spremi kao prema očekivanjima. Koristi se i izračunavanje broja mjesečnih aktivnih korisnika/uređaja i metriku pouzdanosti oblaka.

Prikupljaju se sljedeća polja:

  - **Data\_AddDocTelemRes –** izvješćuje jesmo li mogli pravilno popuniti ostale vrijednosti vezane uz telemetriju dokumenta u sklopu događaja. Koristi se za dijagnostiku kvalitete podataka.

  - **Data\_AddDocTelemResDst –** izvješćuje jesmo li mogli pravilno popuniti ostale vrijednosti vezane uz telemetriju dokumenta u sklopu događaja za odredišni dokument. Koristi se za dijagnostiku kvalitete podataka.

  - **Data\_AddDocTelemResSrc –** izvješćuje jesmo li mogli pravilno popuniti ostale vrijednosti vezane uz telemetriju dokumenta u sklopu događaja za izvorni dokument. Koristi se za dijagnostiku kvalitete podataka.

  - **Data\_DetachedDuration –** koliko je dugo aktivnost bila odvojena od niti

  - **Data\_Doc\_AccessMode –** dokument je samo za čitanje ili za uređivanje

  - **Data\_Doc\_AssistedReadingReasons –** unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

  - **Data\_Doc\_ChunkingType –** jedinice korištene za inkrementalno otvaranje dokumenta

  - **Data\_Doc\_EdpState –** postavka zaštite elektroničkih podataka za dokument

  - **Data\_Doc\_Ext –** nastavak dokumenta (docx/xlsb/pptx itd.)

  - **Data\_Doc\_FileFormat –** verzija protokola za oblik datoteke

  - **Data\_Doc\_Fqdn –** naziv domene servisa OneDrive ili sustava SharePoint Online

  - **Data\_Doc\_FqdnHash –** jednosmjerno raspršivanje naziva domene koji identificira korisnika

  - **Data\_Doc\_IdentityTelemetryId –** jednosmjerno raspršivanje korisničkog identiteta koji se koristio za otvaranje

  - **Data\_Doc\_IOFlags –** izvješćuje o predmemoriranim zastavicama korištenima za postavljanje mogućnosti otvorenog zahtjeva

  - **Data\_Doc\_IrmRights –** radnje dopuštene pravilima zaštite elektroničkih podataka primijenjenima na dokument/korisnika

  - **Data\_Doc\_IsIncrementalOpen –** zastavica koja označava da je dokument inkrementalno otvoren

  - **Data\_Doc\_IsOcsSupported –** zastavica koja označava da je dokument podržan u servisu za suradnju

  - **Data\_Doc\_IsOpeningOfflineCopy –** zastavica koja označava da je otvorena izvanmrežna kopija dokumenta

  - **Data_Doc_IsRtcAlwaysOn –** istinito ako je kanal u stvarnom vremenu (RTC) uvijek uključen za ovu datoteku.

  - **Data\_Doc\_IsSyncBacked –** zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

  - **Data\_Doc\_Location –** označava koji je servis dobavio dokument (OneDrive, File Server, SharePoint itd.)

  - **Data\_Doc\_LocationDetails –** označava koja je poznata mapa dobavila lokalno pohranjeni dokument

  - **Data\_Doc\_NumberCoAuthors –** broj drugih korisnika u sesiji zajedničkog uređivanja

  - **Data\_Doc\_ReadOnlyReasons –** razlozi zbog kojih je dokument otvoren samo za čitanje

  - **Data\_Doc\_ResourceIdHash –** anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

  - **Data\_Doc\_ServerDocId –** nepromjenjivi anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

  - **Data\_Doc\_ServerProtocol –** verzija protokola korištena za komuniciranje sa servisom

  - **Data\_Doc\_ServerType –** vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.)

  - **Data\_Doc\_ServerVersion –** verzija poslužitelja koji pruža servis

  - **Data\_Doc\_SessionId –** identificira specifičnu sesiju uređivanja dokumenta u sklopu cijele sesije

  - **Data\_Doc\_SharePointServiceContext –** dijagnostičke informacije iz zahtjeva sustava SharePoint Online

  - **Data\_Doc\_SizeInBytes –** pokazatelj veličine dokumenta

  - **Data\_Doc\_SpecialChars –** pokazatelj posebnih znakova u URL–u ili putu dokumenta

  - **Data\_Doc\_StreamAvailability –** pokazatelj je li tok dokumenta dostupan/onemogućen

  - **Data\_Doc\_UrlHash –** jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta

  - **Data\_DstDoc\_AccessMode –** odredišni je dokument samo za čitanje ili za uređivanje

  - **Data\_DstDoc\_AssistedReadingReasons –** unaprijed definiran skup vrijednosti razloga zbog kojih se odredišni dokument otvorio u načinu za pomoć pri čitanju

  - **Data\_DstDoc\_ChunkingType –** jedinice korištene za inkrementalno otvaranje dokumenta

  - **Data\_DstDoc\_EdpState –** postavka zaštite elektroničkih podataka za odredišni dokument

  - **Data\_DstDoc\_Ext –** nastavak dokumenta (docx/xlsb/pptx itd.)

  - **Data\_DstDoc\_FileFormat –** verzija protokola za oblik datoteke

  - **Data\_DstDoc\_Fqdn –** naziv domene servisa OneDrive ili sustava SharePoint Online za odredišni dokument

  - **Data\_DstDoc\_FqdnHash –** jednosmjerno raspršivanje naziva domene koji identificira korisnika za odredišni dokument

  - **Data\_DstDoc\_IdentityTelemetryId –** jednosmjerno raspršivanje korisničkog identiteta korištenog za otvaranje

  - **Data\_DstDoc\_InitializationScenario –** bilježi način otvaranja dokumenta

  - **Data\_DstDoc\_IOFlags –** izvješćuje o predmemoriranim zastavicama korištenima za postavljanje mogućnosti otvorenog zahtjeva za odredišni dokument

  - **Data\_DstDoc\_IrmRights –** radnje dopuštene pravilima zaštite elektroničkih podataka primijenjenima na odredišni dokument ili odredišnog korisnika

  - **Data\_DstDoc\_IsIncrementalOpen –** zastavica koja označava da je dokument inkrementalno otvoren

  - **Data\_DstDoc\_IsOcsSupported –** zastavica koja označava da je dokument podržan u servisu za suradnju

  - **Data\_DstDoc\_IsOpeningOfflineCopy –** zastavica koja označava da je otvorena izvanmrežna kopija dokumenta

  - **Data\_DstDoc\_IsSyncBacked – **zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

  - **Data\_DstDoc\_Location –** označava koji je servis pružio pohranu odredišnog dokumenta (OneDrive, File Server, SharePoint itd.)

  - **Data\_DstDoc\_LocationDetails –** označava koja je poznata mapa dobavila lokalno pohranjeni dokument

  - **Data\_DstDoc\_NumberCoAuthors –** broj drugih korisnika u sesiji zajedničkog uređivanja

  - **Data\_DstDoc\_PasswordFlags –** označava zastavice za čitanje ili čitanje i pisanje lozinke postavljene za odredišni dokument

  - **Data\_DstDoc\_ReadOnlyReasons –** razlozi zbog kojih je odredišni dokument otvoren samo za čitanje

  - **Data\_DstDoc\_ResourceIdHash –** anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

  - **Data\_DstDoc\_ServerDocId –** nepromjenjivi anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

  - **Data\_DstDoc\_ServerProtocol –** verzija protokola korištena za komuniciranje sa servisom

  - **Data\_DstDoc\_ServerType –** vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.)

  - **Data\_DstDoc\_ServerVersion –** verzija poslužitelja koji pruža servis

  - **Data\_DstDoc\_SessionId –** identificira specifičnu sesiju uređivanja dokumenta u sklopu cijele sesije

  - **Data\_DstDoc\_SharePointServiceContext –** dijagnostičke informacije iz zahtjeva sustava SharePoint Online

  - **Data\_DstDoc\_SizeInBytes –** pokazatelj veličine dokumenta

  - **Data\_DstDoc\_SpecialChars –** pokazatelj posebnih znakova u URL-u ili putu dokumenta

  - **Data\_DstDoc\_StreamAvailability –** pokazatelj je li tok dokumenta dostupan/onemogućen

  - **Data\_DstDoc\_SyncBackedType –** pokazatelj vrste dokumenta (lokalni ili na servisu)

  - **Data\_DstDoc\_UrlHash –** jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta za odredišni dokument

  - **Data\_DstDoc\_WopiServiceId –** sadrži jedinstveni identifikator davatelja usluge WOPI

  - **Data\_FailureClass –** cijeli broj koji predstavlja klasu neuspjeha za neuspjehe OCS tranzicije

  - **Data\_LocationPickerPropagateToSaveTime,spLapsedMsec –** u milisekundama mjeri vrijeme potrebno da se pokrene spremanje nakon dobivanja rezultata od birača lokacije

  - **Data\_LocationPickerSaveStatus –** status koji je birač lokacije vratio

  - **Data\_MainPdod –** identifikator dokumenta u sklopu procesa Office Word

  - **Data\_MoveDisabledReason –** pogreška koja onemogućuje premještanje dokumenta

  - **Data\_MoveFlightEnabled –** je li omogućena testna verzija za značajku premještanja

  - **Data\_RenameDisabledReason –** pogreška koja uzrokuje onemogućivanje preimenovanja za taj dokument

  - **Data\_RenameFlightEnabled –** je li omogućena testna verzija za značajku preimenovanja

  - **Data\_SaveInitiateKind –** cijeli broj koji označava kako je pokrenuto spremanje

  - **Data\_SrcDoc\_AccessMode –** izvorni je dokument samo za čitanje ili za uređivanje

  - **Data\_SrcDoc\_AssistedReadingReasons –** unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

  - **Data\_SrcDoc\_ChunkingType –** jedinice korištene za inkrementalno otvaranje dokumenta

  - **Data\_SrcDoc\_EdpState –** postavka zaštite elektroničkih podataka za izvorni dokument

  - **Data\_SrcDoc\_Ext –** nastavak dokumenta za izvorni dokument (docx/xlsb/pptx itd.)

  - **Data\_SrcDoc\_FileFormat –** verzija protokola za oblik datoteke za izvorni dokument

  - **Data\_SrcDoc\_Fqdn –** naziv domene servisa OneDrive ili sustava SharePoint Online za izvorni dokument

  - **Data\_SrcDoc\_FqdnHash –** jednosmjerno raspršivanje naziva domene koji identificira korisnika za izvorni dokument

  - **Data\_SrcDoc\_IdentityTelemetryId –** jednosmjerno raspršivanje korisničkog identiteta korištenog za otvaranje

  - **Data\_SrcDoc\_InitializationScenario –** bilježi način otvaranja dokumenta

  - **Data\_SrcDoc\_IOFlags –** izvješćuje o predmemoriranim zastavicama korištenima za postavljanje mogućnosti otvorenog zahtjeva

  - **Data\_SrcDoc\_IrmRights –** radnje dopuštene pravilima zaštite elektroničkih podataka primijenjenima na dokument/korisnika

  - **Data\_SrcDoc\_IsIncrementalOpen –** zastavica koja označava da je dokument inkrementalno otvoren

  - **Data\_SrcDoc\_IsOcsSupported –** zastavica koja označava da je dokument podržan u servisu za suradnju

  - **Data\_SrcDoc\_IsOpeningOfflineCopy –** zastavica koja označava da je otvorena izvanmrežna kopija dokumenta

  - **Data\_SrcDoc\_IsSyncBacked – **zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

  - **Data\_SrcDoc\_Location –** označava koji je servis dobavio izvorni dokument (OneDrive, File Server, SharePoint itd.)

  - **Data\_SrcDoc\_LocationDetails –** označava koja je poznata mapa dobavila lokalno pohranjeni dokument

  - **Data\_SrcDoc\_NumberCoAuthors –** broj drugih korisnika u sesiji zajedničkog uređivanja

  - **Data\_SrcDoc\_PasswordFlags –** označava postavljene zastavice za čitanje ili čitanje i pisanje lozinke

  - **Data\_SrcDoc\_ReadOnlyReasons –** razlozi zbog kojih je dokument otvoren samo za čitanje

  - **Data\_SrcDoc\_ResourceIdHash –** anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

  - **Data\_SrcDoc\_ServerDocId –** nepromjenjivi anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

  - **Data\_SrcDoc\_ServerProtocol –** verzija protokola korištena za komuniciranje sa servisom

  - **Data\_SrcDoc\_ServerType –** vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.)

  - **Data\_SrcDoc\_ServerVersion –** verzija poslužitelja koji pruža servis

  - **Data\_SrcDoc\_SessionId –** identificira specifičnu sesiju uređivanja dokumenta u sklopu cijele sesije

  - **Data\_SrcDoc\_SharePointServiceContext –** dijagnostičke informacije iz zahtjeva sustava SharePoint Online

  - **Data\_SrcDoc\_SizeInBytes –** pokazatelj veličine dokumenta

  - **Data\_SrcDoc\_SpecialChars –** pokazatelj posebnih znakova u URL-u ili putu dokumenta

  - **Data\_SrcDoc\_StreamAvailability –** pokazatelj je li tok dokumenta dostupan/onemogućen

  - **Data\_SrcDoc\_SyncBackedType –** pokazatelj vrste dokumenta (lokalni ili na servisu)

  - **Data\_SrcDoc\_UrlHash –** jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta

  - **Data\_SrcDoc\_WopiServiceId –** sadrži jedinstveni identifikator davatelja usluge WOPI

  - **Data\_SrcDocIsUnnamedOrNew –** označava je li dokument koji spremamo nov

#### <a name="officewordworddocumentdirtyflagchanged"></a>Office.Word.Word.DocumentDirtyFlagChanged

Ovaj događaj označava da Office Word uređuje dokument koji mijenja interno stanje dokumenta u „prljavo”. On Microsoftu omogućuje procjenu stanja značajke uređivanja dokumenta. Taj je događaj impuls korisničkog uređivanja. Koristi se i izračunavanje broja mjesečnih aktivnih korisnika/uređaja.

Prikupljaju se sljedeća polja:

  - **Data\_CollectionTime–** vremenska oznaka događaja

  - **Data\_DocumentLocation–** vrsta mjesta dokumenta

  - **Data\_DocumentLocationDetails–** podvrsta mjesta dokumenta

  - **Data\_FAlwaysSaveEnabled–** označava je li omogućeno spremanje u bilo kojem trenutku

  - **Data\_FirstEditTime–** vremenska oznaka prvog uređivanja

  - **Data\_NumberCoAuthors–** broj suautora koji su uređivali dokument tijekom sesije

  - **Data\_NumberOfTimesDocumentDirtied–** broj izmjena u dokumentu

  - **Data\_Pdod–** identifikator dokumenta u sklopu procesa Office Word

  - **Data\_UrlHash–** raspršivanje puta dokumenta

  - **Data\_ViewKind–** vrsta prikaza u programu Word

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

### <a name="application-status-and-boot-subtype"></a>*Podvrsta stanja i pokretanja aplikacije*

Utvrđivanje je li došlo do određenih događaja povezanih sa značajkama, poput pokretanja ili zaustavljanja, te je li značajka pokrenuta.

#### <a name="officeextensibilityofficejsappactivated"></a>Office.Extensibility.OfficeJS.Appactivated

Bilježi informacije o neočekivanim isključivanjima sustava Office. To nam omogućuje prepoznavanje rušenja ili blokiranja proizvoda kako bismo na njih mogli reagirati.

Prikupljaju se sljedeća polja:

  - **Data\_AirspaceInitTime:integer–** trajanje inicijalizacije komponente Airspace za Office

  - **Data\_AllShapes:integer –** broj oblika u dokumentu

  - **Data\_APIInitTime:integer –** trajanje inicijalizacije API modula za Visio

  - **Data\_AppSizeHeight –** visina prozora dodatka

  - **Data\_AppSizeWidth –** širina prozora dodatka

  - **Data\_AppURL –** URL dodatka; bilježi puni URL za dodatke iz trgovine i domenu URL-a za dodatke koji nisu iz trgovine

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

  - **Data_Doc_IsRtcAlwaysOn –** istinito ako je kanal u stvarnom vremenu (RTC) uvijek uključen za ovu datoteku.

  - **Data\_Doc\_IsSyncBacked:bool–** istinito kad je riječ o poslužiteljskom dokumentu koji postoji lokalno te se sinkronizira s poslužiteljem (npr. putem servisa OneDrive ili ODB klijentskih aplikacija)

  - **Data\_Doc\_Location:long–** : unaprijed definiran skup vrijednosti mjesta na kojima se dokument pohranjuje (lokalno, SharePoint, WOPI, mreža itd.)

  - **Data\_Doc\_LocationDetails:long –** unaprijed definiran skup vrijednosti detaljnijih lokacija (mapa Temp, mapa preuzimanja, dokumenti servisa One Drive, slike servisa One Drive)

  - **Data\_Doc\_ResourceIdHash:string –** raspršivanje identifikatora resursa za dokumente pohranjene u oblaku

  - **Data\_Doc\_ServerDocId:string –** nepromjenjivi identifikator za dokumente pohranjene u oblaku

  - **Data\_Doc\_SessionId:long –** generirani GUID koji identificira instancu dokumenta u sklopu iste sesije procesa

  - **Data\_Doc\_SizeInBytes:long –** veličina dokumenta u bajtovima

  - **Data\_Doc\_SpecialChars:long –** dugačka bit-maska koja pokazuje posebne znakove u URL-u ili putu dokumenta

  - **Data\_Doc\_SyncBackedType –** pokazatelj vrste dokumenta (lokalni ili na servisu) 

  - **Data\_Doc\_UrlHash:string –** raspršivanje punog URL-a dokumenata pohranjenih u oblaku

  - **Data\_DpiAwarenessTime:integer –** trajanje omogućivanja svjesnosti o razlučivosti po monitoru

  - **Data\_DurationToCompleteInMilliseconds:double–** trajanje spremanja u milisekundama

  - **Data\_ErrorCode:int –** : 0 za uspjelo, a cijeli broj za neuspjelo spremanje

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

  - **Data\_InternalFile:bool –** istinito ako je datoteka interna datoteka. npr. šablona

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

  - **Data\_MsoInitCoreTime:integer –** trajanje inicijalizacije MSO komponente sustava office

  - **Data\_MsoInitUITime:integer –** trajanje inicijalizacije korisničkog sučelja MSO komponente sustava office

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

  - **Data\_SDX\_HostJsVersion –** ovo je verzija sustava Office.js specifična za određenu platformu (npr. outlook web16.01.js) i sadrži podlogu API-ja za dodatke

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

  - **Office.Visio.FileCharacteristicsVisio –** bilježi svojstva datoteke u trenutku pokretanja datoteka za Visio C2R i Dev16. Taj nam događaj pomaže kategorizirati i ispraviti pogreške vezane uz svojstva dokumenta, što pak omogućuje brže otkrivanje korijenskih uzroka problema i njihovo otklanjanje na zadovoljstvo korisnika.

  - **Office.Visio.Shared.BootStats –** taj događaj prikuplja vrijeme pokretanja aplikacije Visio Win32. On prikuplja razna polja za pokretanje različitih komponenti, kao što su vrijeme učitavanja vrpce i vrijeme inicijalizacije aplikacije. Taj se događaj koristi za mjerenje performansi pokretanja programa Visio.

  - **Office.Visio.Shared.FileOpen –** taj događaj prikuplja statistiku otvaranja datoteka za Visio. Taj se događaj koristi za praćenje stopa uspjeha/neuspjeha otvaranja datoteka i njihovo mapiranje s nekolicinom svojstava poput veličine datoteke. Svojstva datoteke omogućuju nam brže ispravljanje pogrešaka i otkrivanje korijenskih uzroka problema.

  - **Office.Visio.Shared.Filesave –** taj događaj prikuplja statistiku spremanja datoteka za Visio. Taj se događaj koristi za praćenje stopa uspjeha/neuspjeha spremanja datoteka i njihovo mapiranje s nekolicinom svojstava kao što su veličina datoteke i mjesto na koje se ona sprema, npr. oblak/lokalno. Svojstva datoteke omogućuju nam brže ispravljanje pogrešaka i otkrivanje korijenskih uzroka problema.

  - **Office.Visio.Shared.FilesaveAs –** taj događaj prikuplja statistiku spremanja datoteka u drugom obliku za Visio. Taj se događaj koristi za praćenje stopa uspjeha/neuspjeha spremanja datoteka i njihovo mapiranje s nekolicinom svojstava kao što su veličina datoteke i mjesto na koje se ona sprema, npr. oblak/lokalno. Svojstva datoteke omogućuju nam brže ispravljanje pogrešaka i otkrivanje korijenskih uzroka problema.

  - **Office.Visio.Shared.PostSave –** taj događaj bilježi razlog neuspjeha prilikom neuspjelog spremanja datoteke.

  - **Office.Visio.VisioFileSaveAs –** taj događaj prikuplja statistiku spremanja datoteka u drugom obliku za Visio Dev 16. Taj se događaj koristi za praćenje stopa uspjeha/neuspjeha spremanja datoteka u drugom obliku i njihovo mapiranje s nekolicinom svojstava kao što su veličina datoteke i mjesto na koje se ona sprema, npr. oblak/lokalno. Svojstva datoteke omogućuju nam brže ispravljanje pogrešaka i otkrivanje korijenskih uzroka problema.

  - **Office.Visio.VisioFileSaveAsync –** taj događaj prikuplja statistiku asinkronog spremanja datoteka za Visio Dev 16. Taj se događaj koristi za praćenje stopa uspjeha/neuspjeha asinkronog spremanja datoteka u drugom obliku i njihovo mapiranje s nekolicinom svojstava kao što su veličina datoteke i mjesto na koje se ona sprema, npr. oblak/lokalno. Svojstva datoteke omogućuju nam brže ispravljanje pogrešaka i otkrivanje korijenskih uzroka problema.

  - **Office.Visio.VisioFileSaveSync –** taj događaj prikuplja statistiku sinkronog spremanja datoteka za Visio Dev 16. Taj se događaj koristi za praćenje stopa uspjeha/neuspjeha sinkronog spremanja datoteka u drugom obliku i njihovo mapiranje s nekolicinom svojstava kao što su veličina datoteke i mjesto na koje se ona sprema, npr. oblak/lokalno. Svojstva datoteke omogućuju nam brže ispravljanje pogrešaka i otkrivanje korijenskih uzroka problema. Taj nam događaj pomaže nadzirati razloge neuspjeha pri spremanju datoteke.

#### <a name="officeoutlookdesktopexchangepuidandtenantcorrelation"></a>Office.Outlook.Desktop.ExchangePuidAndTenantCorrelation

Jedanput po sesiji prikuplja PUID korisnika i identifikator klijenta. Korelacija PUID-a i klijenta nužna je za razumijevanje i dijagnosticiranje problema s programom Outlook na razini pojedinih klijenata.

Prikupljaju se sljedeća polja:

  - **CollectionTime** – vremenska oznaka događaja

  - **ConnId** – identifikator veze: identifikator veze kojom se raščlanjuju PUID i identifikator OMS klijenta

  - **OMSTenantId** – jedinstveni identifikator klijenta, koji generira Microsoft

  - **PUID** – PUID sustava Exchange za jedinstvenu identifikaciju korisnika

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

  - **Data\_ContentTransaction –** unaprijed definiran skup vrijednosti kojima se određuje kada je moguće stvoriti transakciju (AllowedOnLoadDocument, AllowedOnOpenComplete itd.)

  - **Data\_CppUncaughtExceptionCount:long –** neuhvaćene lokalne iznimke dok se aktivnost izvršavala

  - **Data\_CreateDocumentTimeMS –** trajanje izvršavanja metode CreateDocumentTimeMS u milisekundama

  - **Data\_CreateDocumentToken –** trajanje izvršavanja metode CreateDocumentToken u milisekundama

  - **Data\_CreateDocumentToW –** trajanje izvršavanja metode CreateDocumentToW u milisekundama

  - **Data\_CreateDocWindow –** trajanje izvršavanja metode CreateDocWindow u milisekundama

  - **Data\_CreateLocalTempFile –** trajanje izvršavanja metode CreateLocalTempFile u milisekundama

  - **Data\_DetachedDuration:long –** vrijeme tijekom kojeg je aktivnost bila odvojena ili se nije izvršavala

  - **Data\_DetermineFileType –** trajanje izvršavanja metode DetermineFileType u milisekundama

  - **Data\_Doc\_AccessMode:long –** kako je dokument otvoren (samo za čitanje / za čitanje i pisanje)

  - **Data\_Doc\_AssistedReadingReasons:long –** unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

  - **Data\_Doc\_ChunkingType:long –** kako je dokument pohranjen u sustavu SharePoint

  - **Data\_Doc\_EdpState:long –** stanje dokumenta s obzirom na zaštitu korporativnih podataka

  - **Data\_Doc\_Ext:string –** nastavak dokumenta

  - **Data\_Doc\_Extension:string –** nastavak dokumenta

  - **Data\_Doc\_FileFormat:long –** unaprijed definiran skup vrijednosti oblika datoteke (precizniji od nastavka)

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

  - **Data_Doc_IsRtcAlwaysOn –** istinito ako je kanal u stvarnom vremenu (RTC) uvijek uključen za ovu datoteku.

  - **Data\_Doc\_IsSyncBacked:bool –** otvara li se dokument iz mape koja koristi aplikaciju za povratnu sinkronizaciju sa servisom OneDrive

  - **Data\_Doc\_Location:long –** unaprijed definiran skup vrijednosti mjesta na kojima se dokument pohranjuje (lokalno, SharePoint, WOPI, mreža itd.)

  - **Data\_Doc\_LocationDetails:long –** unaprijed definiran skup vrijednosti detaljnijih lokacija (mapa Temp, mapa preuzimanja, dokumenti servisa One Drive, slike servisa One Drive itd.)

  - **Data\_Doc\_NumberCoAuthors:long –** broj suautora u trenutku otvaranja dokumenta

  - **Data\_Doc\_PasswordFlags:long –** unaprijed definiran skup vrijednosti načina na koji je dokument šifriran pomoću lozinke (nema, lozinka za čitanje, lozinka za uređivanje)

  - **Data\_Doc\_ReadOnlyReasons:long –** unaprijed definiran skup vrijednosti koji naznačuje zašto je dokument označen samo za čitanje (zaključan na poslužitelju, konačni dokument, zaštićen lozinkom za uređivanje itd.)

  - **Data\_Doc\_ResourceIdHash:string –** raspršivanje identifikatora resursa za dokumente pohranjene u oblaku

  - **Data\_Doc\_ServerDocId:string –** nepromjenjivi identifikator za dokumente pohranjene u oblaku

  - **Data\_Doc\_ServerProtocol:long –** unaprijed definiran skup vrijednosti za protokol koji se koristi za komuniciranje s poslužiteljem (Http, Cobalt, WOPI itd.)

  - **Data\_Doc\_ServerType:long –** unaprijed definiran skup vrijednosti za vrstu poslužitelja (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long –** temelji li se poslužitelj na sustavu Office14, Office15 ili Office 16?

  - **Data\_Doc\_SessionId:long –** generirani GUID koji identificira instancu dokumenta u sklopu iste sesije procesa

  - **Data\_Doc\_SharePointServiceContext:string –** neprozirni niz, obično GridManagerID.FarmID. Korisno za korelaciju klijentskih i poslužiteljskih zapisnika

  - **Data\_Doc\_SizeInBytes:long –** veličina dokumenta u bajtovima

  - **Data\_Doc\_SpecialChars:long –** bit-maska koja pokazuje posebne znakove u URL-u ili putu dokumenta

  - **Data\_Doc\_StorageProviderId:string –** niz koji identificira davatelja pohrane dokumenta, primjerice „DropBox“

  - **Data\_Doc\_StreamAvailability:long –** unaprijed definiran skup vrijednosti statusa toka dokumenta (dostupno, trajno onemogućeno, nije dostupno)

  - **Data\_Doc\_UrlHash:string –** raspršivanje punog URL-a dokumenata pohranjenih u oblaku

  - **Data\_Doc\_UsedWrsDataOnOpen:bool –** istinito ako je datoteka otvorena inkrementalno pomoću predmemoriranih WRS podataka na glavnom računalu

  - **Data\_Doc\_WopiServiceId:string –** identifikator WOPI servisa, npr. „Dropbox“

  - **Data\_DownloadExcludedData –** trajanje izvršavanja metode DownloadExcludedData u milisekundama

  - **Data\_DownloadExcludedDataTelemetry –** unaprijed definiran skup vrijednosti stanja sinkronog čekanja na preuzimanje (SynchronousLogicHit, UserCancelled RunModalTaskUnexpectedHResult itd.)

  - **Data\_DownloadFileInBGThread –** trajanje izvršavanja metode DownloadFileInBGThread u millisekundama

  - **Data\_DownloadFragmentSize –** veličina fragmenta (bloka datoteke koji je moguće preuzeti), obično 3,5 MB

  - **Data\_ExcludedEmbeddedItems –** broj zip dijelova izuzetih iz prvog prikaza

  - **Data\_ExcludedEmbeddedItemsSize –** ukupna veličina zip dijelova izuzetih iz prvog prikaza

  - **Data\_ExcludedRequiredItems –** broj zip dijelova koji su izuzeti, ali su obavezni za prvi prikaz

  - **Data\_ExcludedRequiredItemsSize –** ukupna veličina zip dijelova koji su izuzeti, ali su obavezni za prvi prikaz

  - **Data\_ExecutionCount –** koliko je puta izvršen protokol IncOpen

  - **Data\_FailureComponent:long –** unaprijed definiran skup vrijednosti koje označavaju koja je komponenta uzrokovala neuspjeh ovog protokola? (Conflict, CSI, Internal itd.)

  - **Data\_FailureReason:long –** unaprijed definiran skup vrijednosti razloga neuspjeha (FileIsCorrupt, BlockedByAntivirus itd.)

  - **Data\_FCreateNew –** je li to nov prazan dokument

  - **Data\_FCreateNewFromTemplate –** je li to nov dokument iz predložaka

  - **Data_FErrorAfterDocWinCreation:boolean –** je li se dogodila pogreška ili iznimka nakon stvaranja prozora dokumenta.

  - **Data\_FileUrlLocation –** unaprijed definiran skup vrijednosti mjesta pohrane dokumenta (NetworkShare, LocalDrive, ServerOther itd.)

  - **Data\_FirstSlideCompressedSize –** komprimirana veličina zip dijela prvog slajda (obično Slide1.xml)

  - **Data\_FIsDownloadFileInBgThreadEnabled –** je li omogućeno preuzimanje u pozadinskoj niti?

  - **Data\_fLifeguarded:bool –** je li dokument ikad popravljen pomoću značajke lifeguard (značajka za popravljanje pogrešaka dokumenta bez slanja upita korisniku)?

  - **Data\_ForceReopenOnIncOpenMergeFailure –** zastavica koja označava jesmo li bili primorani na ponovno otvaranje zbog neuspjelog spajanja pri inkrementalnom otvaranju

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

  - **Data\_OpenCompleteFailureHR –** rezultat koji govori zašto protokol OpenComplete nije uspio

  - **Data\_OpenCompleteFailureTag –** oznaka (pokazivač na mjesto u kodu) mjesta na kojem je protokol OpenComplete doživio neuspjeh

  - **Data\_OpenLifeguardOption –** unaprijed definiran skup vrijednosti izbora za lifeguard operaciju (None, TryAgain, OpenInWebApp itd.)

  - **Data\_OpenReason –** unaprijed definiran skup vrijednosti načina na koji je taj dokument otvoren (FilePicker, OpenFromMru, FileDrop itd.)

  - **Data\_OSRPolicy –** pravilnik za sigurni čitač

  - **Data\_OSRReason –** razlozi zašto je dokument otvoren u sigurnom čitaču

  - **Data\_OtherContentTypesWithRequiredParts –** nestandardne vrste sadržaja koje su izuzete, ali su obavezne za prvi prikaz

  - **Data\_PrepCacheAsync –** zastavica za OcsiOpenPerfPrepCacheAsync

  - **Data\_PreviousDiscardFailed –** označava da prethodni pokušaj otvaranja/zatvaranja dokumenta nije pravilno oslobodio svu memoriju

  - **Data\_PreviousFailureHr –** u slučaju ponovnog otvaranja istog dokumenta, što je bio rezultat zadnjeg neuspjeha

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

- **AppSessionGuid** – identifikator određene sesije aplikacije, koja započinje u trenutku stvaranja procesa i traje do njegovog okončanja. Oblikovan je kao standardni 128-bitni GUID, ali se sastoji od 4 dijela. Ta su četiri dijela redom: (1) 32-bitni ID procesa (2) 16-bitni ID sesije (3) 16-bitni ID pokretanja (4) 64-bitno UTC vrijeme stvaranja procesa, izraženo u koracima od 100 ns

- **processSessionId** – nasumično generirani guid za identifikaciju sesije aplikacije

- **UTCReplace_AppSessionGuid** – konstantna Booleova vrijednost. Uvijek istinito.

#### <a name="officetelemetryengineisprelaunch"></a>Office.TelemetryEngine.IsPreLaunch

Primjenjuje se na aplikacije sustava Office za UWP.  Taj se događaj pokreće kada se aplikacija sustava office prvi put pokrene nakon nadogradnje/instalacije iz trgovine. Dio je osnovnih dijagnostičkih podataka, a koristi se za praćenje je li riječ o sesiji prvog pokretanja.

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

#### <a name="officewordfileopenopencmdfilemrupriv"></a>Office.Word.FileOpen.OpenCmdFileMruPriv

Taj događaj označava da Office Word otvara dokument s popisa nedavno korištenih dokumenata (MRU). Sadrži i ključne podatke o performansama otvaranja datoteka, a iz perspektive korisnika predstavlja događaj pokretanja aplikacije. Događaj nadzire funkcionira li otvaranje datoteka s MRU-a prema očekivanjima. Koristi se i za izračunavanje broja mjesečnih aktivnih korisnika/uređaja i metriku pouzdanosti oblaka.

Prikupljaju se sljedeća polja:

  - **Data\_AddDocTelemRes –** izvješćuje jesmo li mogli pravilno popuniti ostale vrijednosti vezane uz telemetriju dokumenta u sklopu događaja. Koristi se za dijagnostiku kvalitete podataka.

  - **Data\_BytesAsynchronous –** broj (sažetih) bajtova za koje vjerujemo da možemo otvoriti datoteku bez njih ako ih dobijemo prije nego što korisnik poželi početi uređivati ili možda spremati

  - **Data\_BytesAsynchronousWithWork –** broj (sažetih) bajtova bez kojih bismo možda mogli otvoriti datoteku, ali bi to zahtijevalo značajna ulaganja u kod

  - **Data\_BytesSynchronous –** broj (sažetih) bajtova koje moramo imati prije nego što možemo početi otvarati datoteku

  - **Data\_BytesUnknown –** broj bajtova u dijelovima dokumenta koje ne očekujemo pronaći

  - **Data\_DetachedDuration –** koliko je dugo aktivnost bila odvojena od niti

  - **Data\_Doc\_AccessMode –** dokument je samo za čitanje ili za uređivanje

  - **Data\_Doc\_AssistedReadingReasons –** unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

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

  - **Data_Doc_IsRtcAlwaysOn –** istinito ako je kanal u stvarnom vremenu (RTC) uvijek uključen za ovu datoteku.

  - **Data\_Doc\_IsSyncBacked – **zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

  - **Data\_Doc\_Location –** označava koji je servis dobavio dokument (OneDrive, File Server, SharePoint itd.)

  - **Data\_Doc\_LocationDetails –** označava koja je poznata mapa dobavila lokalno pohranjeni dokument

  - **Data\_Doc\_NumberCoAuthors –** broj drugih korisnika u sesiji zajedničkog uređivanja

  - **Data\_Doc\_PasswordFlags –** označava postavljene zastavice za čitanje ili čitanje i pisanje lozinke

  - **Data\_Doc\_ReadOnlyReasons –** razlozi zbog kojih je dokument otvoren samo za čitanje

  - **Data\_Doc\_ResourceIdHash –** anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

  - **Data\_Doc\_ServerDocId –** nepromjenjivi anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

  - **Data\_Doc\_ServerProtocol –** verzija protokola korištena za komuniciranje sa servisom

  - **Data\_Doc\_ServerType –** vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.)

  - **Data\_Doc\_ServerVersion –** verzija poslužitelja koji pruža servis

  - **Data\_Doc\_SessionId –** identificira specifičnu sesiju uređivanja dokumenta u sklopu cijele sesije

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

  - **Data\_Measurements –** šifrirani niz koji sadrži analizu trajanja različitih dijelova otvaranja. Koristi se za mjerenje performansi.

  - **Data\_MoveDisabledReason –** pogreška koja onemogućuje premještanje dokumenta

  - **Data\_MoveFlightEnabled –** je li omogućena testna verzija za značajku premještanja

  - **Data\_PartsUnknown –** broj dijelova dokumenta za koje nismo mogli pribaviti podatke

  - **Data\_RecoverableFailureInitiationLocationTag –** jedinstvena oznaka mjesta pozivanja koda, koja se koristi za identifikaciju mjesta na kojem pokušavamo popraviti datoteku prije otvaranja

  - **Data\_RenameDisabledReason –** pogreška koja uzrokuje onemogućivanje preimenovanja za taj dokument

  - **Data\_RenameFlightEnabled –** je li omogućena testna verzija za značajku preimenovanja

  - **Data\_SecondaryTag –** jedinstvena oznaka mjesta pozivanja koda, koja se koristi za dodavanje dodatnih podataka o neuspjelom otvaranju

  - **Data\_TemplateFormat –** oblik datoteke predloška na kojem se dokument temelji.

  - **Data\_UsesNormal –** označava temelji li se otvoreni dokument na predlošku Normal

#### <a name="officewordfileopenopenffileopenxstzcore"></a>Office.Word.FileOpen.OpenFFileOpenXstzCore

Taj događaj označava da Office Word otvara dokument koji je korisnik dvaput kliknuo. Sadrži i ključne podatke o performansama otvaranja datoteka, a iz perspektive korisnika predstavlja događaj pokretanja aplikacije. Događaj nadzire funkcionira li otvaranje datoteke dvostrukim klikom prema očekivanjima. Koristi se i za izračunavanje broja mjesečnih aktivnih korisnika/uređaja i metriku pouzdanosti oblaka.

Prikupljaju se sljedeća polja:

  - **Data\_AddDocTelemRes –** izvješćuje jesmo li mogli pravilno popuniti ostale vrijednosti vezane uz telemetriju dokumenta u sklopu događaja. Koristi se za dijagnostiku kvalitete podataka

  - **Data\_BytesAsynchronous –** broj (sažetih) bajtova za koje vjerujemo da možemo otvoriti datoteku bez njih ako ih dobijemo prije nego što korisnik poželi početi uređivati ili možda spremati

  - **Data\_BytesAsynchronousWithWork –** broj (sažetih) bajtova bez kojih bismo možda mogli otvoriti datoteku, ali bi to zahtijevalo značajna ulaganja u kod

  - **Data\_BytesSynchronous –** broj (sažetih) bajtova koje moramo imati prije nego što možemo početi otvarati datoteku

  - **Data\_BytesUnknown –** broj bajtova u dijelovima dokumenta koje ne očekujemo pronaći

  - **Data\_DetachedDuration –** koliko je dugo aktivnost bila odvojena od niti

  - **Data\_Doc\_AccessMode –** dokument je samo za čitanje ili za uređivanje

  - **Data\_Doc\_AssistedReadingReasons –** unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

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

  - **Data_Doc_IsRtcAlwaysOn –** istinito ako je kanal u stvarnom vremenu (RTC) uvijek uključen za ovu datoteku.

  - **Data\_Doc\_IsSyncBacked –** zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

  - **Data\_Doc\_Location –** označava koji je servis dobavio dokument (OneDrive, File Server, SharePoint itd.)

  - **Data\_Doc\_LocationDetails –** označava koja je poznata mapa dobavila lokalno pohranjeni dokument

  - **Data\_Doc\_NumberCoAuthors –** broj drugih korisnika u sesiji zajedničkog uređivanja

  - **Data\_Doc\_PasswordFlags –** označava postavljene zastavice za čitanje ili čitanje i pisanje lozinke

  - **Data\_Doc\_ReadOnlyReasons –** razlozi zbog kojih je dokument otvoren samo za čitanje

  - **Data\_Doc\_ResourceIdHash –** anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

  - **Data\_Doc\_ServerDocId –** nepromjenjivi anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

  - **Data\_Doc\_ServerProtocol –** verzija protokola korištena za komuniciranje sa servisom

  - **Data\_Doc\_ServerType –** vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.)

  - **Data\_Doc\_ServerVersion –** verzija poslužitelja koji pruža servis

  - **Data\_Doc\_SessionId –** verzija poslužitelja koji pruža servis

  - **Data\_Doc\_SharePointServiceContext–**

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

  - **Data\_Measurements –** šifrirani niz koji sadrži analizu trajanja različitih dijelova otvaranja. Koristi se za mjerenje performansi.

  - **Data\_MoveDisabledReason –** pogreška koja onemogućuje premještanje dokumenta

  - **Data\_MoveFlightEnabled –** je li omogućena testna verzija za značajku premještanja

  - **Data\_PartsUnknown –** broj dijelova dokumenta za koje nismo mogli pribaviti podatke

  - **Data\_RecoverableFailureInitiationLocationTag –** jedinstvena oznaka mjesta pozivanja koda, koja se koristi za identifikaciju mjesta na kojem pokušavamo popraviti datoteku prije otvaranja.

  - **Data\_RenameDisabledReason –** pogreška koja uzrokuje onemogućivanje preimenovanja za taj dokument

  - **Data\_RenameFlightEnabled –** je li omogućena testna verzija za značajku preimenovanja

  - **Data\_SecondaryTag –** jedinstvena oznaka mjesta pozivanja koda, koja se koristi za dodavanje dodatnih podataka o neuspjelom otvaranju.

  - **Data\_TemplateFormat –** oblik datoteke predloška na kojem se dokument temelji.

  - **Data\_UsesNormal –** označava temelji li se otvoreni dokument na predlošku Normal


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

  - **Data_Doc_IsRtcAlwaysOn –** istinito ako je kanal u stvarnom vremenu (RTC) uvijek uključen za ovu datoteku.

  - **Data\_Doc\_IsSyncBacked –** zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

  - **Data\_Doc\_Location –** označava koji je servis dobavio dokument (OneDrive, File Server, SharePoint)

  - **Data\_Doc\_LocationDetails –** označava koja je poznata mapa dobavila lokalno pohranjeni dokument

  - **Data\_Doc\_NumberCoAuthors –** broj drugih korisnika u sesiji zajedničkog uređivanja

  - **Data\_Doc\_PasswordFlags –** označava postavljene zastavice za čitanje ili čitanje i pisanje lozinke

  - **Data\_Doc\_ReadOnlyReasons –** razlozi zbog kojih je dokument otvoren samo za čitanje

  - **Data\_Doc\_ResourceIdHash –** anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

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

  - **Data\_AddDocTelemRes –** izvješćuje jesmo li mogli pravilno popuniti ostale vrijednosti vezane uz telemetriju dokumenta u sklopu događaja. Koristi se za dijagnostiku kvalitete podataka.

  - **Data\_BytesAsynchronous –** broj (sažetih) bajtova za koje vjerujemo da možemo otvoriti datoteku bez njih ako ih dobijemo prije nego što korisnik poželi početi uređivati ili možda spremati

  - **Data\_BytesAsynchronousWithWork –** broj (sažetih) bajtova bez kojih bismo možda mogli otvoriti datoteku, ali bi to zahtijevalo značajna ulaganja u kod

  - **Data\_BytesSynchronous –** broj (sažetih) bajtova koje moramo imati prije nego što možemo početi otvarati datoteku

  - **Data\_BytesUnknown –** broj bajtova u dijelovima dokumenta koje ne očekujemo pronaći

  - **Data\_DetachedDuration –** koliko je dugo aktivnost bila odvojena od niti

  - **Data\_Doc\_AccessMode –** dokument je samo za čitanje ili za uređivanje

  - **Data\_Doc\_AssistedReadingReasons –** unaprijed definiran skup vrijednosti razloga zbog kojih se dokument otvorio u načinu za pomoć pri čitanju

  - **Data\_Doc\_ChunkingType –** jedinice korištene za inkrementalno otvaranje dokumenta

  - **Data\_Doc\_EdpState –** postavka zaštite elektroničkih podataka za dokument

  - **Data\_Doc\_Ext –** nastavak dokumenta (docx/xlsb/pptx itd.)

  - **Data\_Doc\_FileFormat –** verzija protokola za oblik datoteke

  - **Data\_Doc\_Fqdn –** naziv domene servisa OneDrive ili sustava SharePoint Online

  - **Data\_Doc\_FqdnHash –** jednosmjerno raspršivanje naziva domene koji identificira korisnika

  - **Data\_Doc\_IdentityTelemetryId –** jednosmjerno raspršivanje korisničkog identiteta koji se koristio za otvaranje

  - **Data\_Doc\_InitializationScenario –** bilježi način otvaranja dokumenta

  - **Data\_Doc\_IOFlags –** izvješćuje o predmemoriranim zastavicama korištenima za postavljanje mogućnosti otvorenog zahtjeva

  - **Data\_Doc\_IrmRights –** radnje dopuštene pravilima zaštite elektroničkih podataka primijenjenima na dokument/korisnika

  - **Data\_Doc\_IsIncrementalOpen –** zastavica koja označava da je dokument inkrementalno otvoren

  - **Data\_Doc\_IsOcsSupported –** zastavica koja označava da je dokument podržan u servisu za suradnju

  - **Data\_Doc\_IsOpeningOfflineCopy –** zastavica koja označava da je otvorena izvanmrežna kopija dokumenta

  - **Data_Doc_IsRtcAlwaysOn –** istinito ako je kanal u stvarnom vremenu (RTC) uvijek uključen za ovu datoteku.

  - **Data\_Doc\_IsSyncBacked –** zastavica koja označava da na računalu postoji automatski sinkronizirana kopija dokumenta

  - **Data\_Doc\_Location –** označava koji je servis dobavio dokument (OneDrive, File Server, SharePoint itd.)

  - **Data\_Doc\_LocationDetails –** označava koja je poznata mapa dobavila lokalno pohranjeni dokument

  - **Data\_Doc\_NumberCoAuthors –** broj drugih korisnika u sesiji zajedničkog uređivanja

  - **Data\_Doc\_PasswordFlags –** označava postavljene zastavice za čitanje ili čitanje i pisanje lozinke

  - **Data\_Doc\_ReadOnlyReasons –** razlozi zbog kojih je dokument otvoren samo za čitanje

  - **Data\_Doc\_ResourceIdHash –** anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

  - **Data\_Doc\_ServerDocId –** nepromjenjivi anonimizirani identifikator dokumenta korišten za dijagnosticiranje problema

  - **Data\_Doc\_ServerProtocol –** verzija protokola korištena za komuniciranje sa servisom

  - **Data\_Doc\_ServerType –** vrsta poslužitelja koji pruža servis (SharePoint, OneDrive, WOPI itd.)

  - **Data\_Doc\_ServerVersion –** verzija poslužitelja koji pruža servis

  - **Data\_Doc\_SessionId –** identificira specifičnu sesiju uređivanja dokumenta u sklopu cijele sesije

  - **Data\_Doc\_SharePointServiceContext –** dijagnostičke informacije iz zahtjeva sustava SharePoint Online

  - **Data\_Doc\_SizeInBytes –** pokazatelj veličine dokumenta

  - **Data\_Doc\_SpecialChars –** pokazatelj posebnih znakova u URL–u ili putu dokumenta

  - **Data\_Doc\_StreamAvailability –** pokazatelj je li tok dokumenta dostupan/onemogućen

  - **Data\_Doc\_SyncBackedType –** pokazatelj vrste dokumenta (lokalni ili na servisu)

  - **Data\_Doc\_UrlHash –** jednosmjerno raspršivanje za stvaranje jednostavnog identifikatora dokumenta

  - **Data\_EditorDisablingRename –** identifikator prvog uređivača koji je uzrokovao onemogućivanje preimenovanja

  - **Data\_EditorsCount –** broj uređivača dokumenta

  - **Data\_ForceReadWriteReason –** cijeli broj koji predstavlja razlog zbog kojeg je datoteka prisilno prebačena u način rada za čitanje/pisanje

  - **Data\_FSucceededAfterRecoverableFailure –** označava da je otvaranje uspjelo nakon popravljanja neuspjelog otvaranja dokumenta

  - **Data\_LastLoggedTag –** jedinstvena oznaka mjesta pozivanja koda, koja se koristi za identifikaciju dvokratnog neuspjelog pokušaja spremanja (koristi se za dijagnostiku kvalitete podataka)

  - **Data\_LinkStyles –** označava povezujemo li se sa stilovima predloška

  - **Data\_MainPdod –** identifikator dokumenta u sklopu procesa Office Word

  - **Data\_Measurements –** šifrirani niz koji sadrži analizu trajanja različitih dijelova otvaranja. Koristi se za mjerenje performansi.

  - **Data\_MoveDisabledReason –** pogreška koja onemogućuje premještanje dokumenta

  - **Data\_MoveFlightEnabled –** je li omogućena testna verzija za značajku premještanja

  - **Data\_PartsUnknown –** broj dijelova dokumenta za koje nismo mogli pribaviti podatke

  - **Data\_RecoverableFailureInitiationLocationTag –** jedinstvena oznaka mjesta pozivanja koda, koja se koristi za identifikaciju mjesta na kojem pokušavamo popraviti datoteku prije otvaranja

  - **Data\_RenameDisabledReason –** pogreška koja uzrokuje onemogućivanje preimenovanja za taj dokument

  - **Data\_RenameFlightEnabled –** je li omogućena testna verzija za značajku preimenovanja

  - **Data\_SecondaryTag –** jedinstvena oznaka mjesta pozivanja koda, koja se koristi za dodavanje dodatnih podataka o neuspjelom otvaranju

  - **Data\_TemplateFormat –** oblik datoteke predloška na kojem se dokument temelji

  - **Data\_UsesNormal** – označava temelji li se otvoreni dokument na predlošku Normal


### <a name="office-accessibility-configuration-subtype"></a>*Podvrsta konfiguracije pristupačnosti za Office*

Značajke pristupačnosti u sustavu Office

#### <a name="officeaccessibilityaccessibilitytoolsessionpresencewin32"></a>Office.Accessibility.AccessibilityToolSessionPresenceWin32

Omogućuje otkrivanje ima li korisnik alat za pomoćne tehnologije i kako se taj alat zove. To nam omogućuje razumjeti ima li korisnik sustava Office problema s određenim alatom za pomoćne tehnologije.

Prikupljaju se sljedeća polja:

  - **Data\_Data\_Jaws –** označava je li Jaws bio pokrenut tijekom sesije**Data\_Data\_Magic –** označava je li Magic bio pokrenut tijekom sesije

  - **Data\_Data\_Magnify –** označava je li Povećavanje bilo pokrenuto tijekom sesije

  - **Data\_Data\_Narrator –** označava je li Pripovjedač bio pokrenut tijekom sesije

  - **Data\_Data\_NVDA –** označava je li NVDA bila pokrenuta tijekom sesije

  - **Data\_Data\_SA –** označava je li SA bila pokrenuta tijekom sesije

  - **Data\_Data\_Supernova –** označava je li Supernova bila pokrenuta tijekom sesije

  - **Data\_Data\_SuperNovaessSuite –** označava je li SuperNovaAccessSuite bio pokrenut tijekom sesije

  - **Data\_Data\_WinEyes –** označava je li WinEyes bio pokrenut tijekom sesije

  - **Data\_Data\_ZoomText –** označava je li ZoomText bio pokrenut tijekom sesije

#### <a name="officewordaccessibilitylearningtoolsreadaloudplayreadaloud"></a>Office.Word.Accessibility.LearningTools.ReadAloud.PlayReadAloud

Taj događaj označava da Office Word naglas čita tekst u dokumentu. Taj je događaj impuls za značajku pristupačnosti koji Microsoftu omogućuje procjenu stanja značajke čitanja teksta naglas.

Prikupljaju se sljedeća polja:

  - **Data\_CharacterCount –** broj znakova u dokumentu

  - **Data\_CharactersWithSpaceCount –** broj znakova i razmaka u dokumentu

  - **Data\_IsPageCountInProgress –** je li brojanje stranica u tijeku

  - **Data\_LineCount –** broj redaka u dokumentu

  - **Data\_PageCount –** broj stranica u dokumentu

  - **Data\_ParagraphCount –** broj odlomaka u dokumentu

  - **Data\_Play –** je li to prvi put da Word čita naglas

  - **Data\_ViewKind –** prikaz vrste dokumenta

  - **Data\_WordCount –** broj riječi u dokumentu

#### <a name="officewordaccessibilitylearningtoolsreadaloudstopreadaloud"></a>Office.Word.Accessibility.LearningTools.ReadAloud.StopReadAloud

Taj događaj označava da Office Word prestaje naglas čitati tekst u dokumentu. Taj događaj Microsoftu omogućuje procjenu stanja značajke čitanja teksta naglas mjerenjem trajanja funkcioniranja.

Prikupljaju se sljedeća polja:

  - Nijedno

## <a name="product-and-service-performance-data-events"></a>Događaji koji se odnose na podatke o performansama proizvoda i usluga

Ovo su podvrste podataka u toj kategoriji:
- [Neočekivano zatvaranje (rušenje) aplikacije](#unexpected-application-exit-crash-subtype)
- [Performanse značajki aplikacije ](#application-feature-performance-subtype)
- [Pogreška aktivnosti aplikacije](#application-activity-error-subtype)

### <a name="unexpected-application-exit-crash-subtype"></a>*Podvrsta neočekivanog zatvaranja (rušenja) aplikacije*

Neočekivana zatvaranja aplikacija i stanje aplikacije kada se to dogodi.

#### <a name="officeappdomainunhandledexceptionhandlerfailed"></a>Office.AppDomain.UnhandledExceptionHandlerFailed

Prikuplja informacije za sve neobrađene iznimke pomoću aplikacije Data Streamer. Ti se podaci koriste za praćenje stanja aplikacije. Taj događaj generira dodatak Microsoft Data Streamer za Excel.

Prikupljaju se sljedeća polja:

- **Iznimka** – poziv stogu zbog iznimke

- **Naziv događaja** – naziv događaja je kategorija i oznaka događaja.

#### <a name="officeextensibilitycomaddinunhandledexception"></a>Office.Extensibility.COMAddinUnhandledException

Događaj koji se stvara prilikom rušenja COM dodatka

Analitika za stolna računala: koristi se kao brojnik za izračun stanja dodatka koje je specifično za velike tvrtke i koje se tijekom pilot-programa koristi da bi se zaključilo je li dodatak „spreman za nadogradnju” u produkcijskom okruženju.  
Globalni uvidi: koriste se za izračun globalne „spremnosti” dodatka, koja nije specifična za velike tvrtke i koja se potom objavljuje na readyforwindows.com i u drugim alatima, kao što je Readiness Toolkit

Prikupljaju se sljedeća polja:

**ScopeId** – doseg trenutne niti

**Method** – metoda sustava Office u kojoj je došlo do iznimke

**Interface** – sučelje sustava Office u kojem je došlo do iznimke

**AddinId** – ID klase dodatka

**AddinProgId** – programski ID dodatka

**AddinFriendlyName** – neslužbeni naziv dodatka

**AddinTimeDateStamp** – vremenska oznaka dodatka iz metapodataka DLL-a

**AddinVersion** – verzija dodatka

**AddinFileName** – naziv datoteke dodatka, bez puta datoteke

**VSTOAddIn** – je li dodatak VSTO

**AddinConnectFlag** – trenutno ponašanje učitavanja

**LoadAttempts** – broj pokušaja učitavanja dodatka

#### <a name="officeextensibilityvbatelemetrybreak"></a>Office.Extensibility.VbaTelemetryBreak

Događaj koji se stvara kada datoteka s omogućenim makronaredbama naiđe na pogrešku pri kompiliranju ili izvođenju

Analitika za stolna računala: koristi se kao brojnik za izračun stanja vrsta makronaredbi (npr. makronaredbe za Word, Excel itd.) koje je specifično za velike tvrtke i koje se tijekom pilot-programa koristi da bi se zaključilo je li dodatak „spreman za nadogradnju” u produkcijskom okruženju.

Prikupljaju se sljedeća polja:

**TagId** – ID telemetrijske oznake

**BreakReason** – razlog zastoja (izvođenje, kompiliranje, druga pogreška)

**SolutionType** – vrsta rješenja (dokument, predložak, dodatak za aplikaciju, COM dodatak)

**Data.ErrorCode** – kod pogreške koji je prijavio VBA modul

#### <a name="officeoutlookdesktophangbucketmetrics"></a>Office.Outlook.Desktop.HangBucketMetrics

Prikuplja vrijeme blokiranja programa Outlook – jedinstveni identifikator po blokiranju, proteklom vremenu i informacijama o pozivanju stoga. Podaci se koriste za otkrivanje i identifikaciju rušenja aplikacije radi rješavanja problema u budućim ažuriranjima.

Prikupljaju se sljedeća polja:

  - **BucketId** – raspršivanje poziva stogu 

  - **ElapsedTotal** – ukupno vrijeme provedeno u pozivu

  - **ElapsedHanging** – vrijeme blokade provedeno u pozivu

#### <a name="officeoutlookdesktophangreportingscopeperfmetrics"></a>Office.Outlook.Desktop.HangReportingScopePerfMetrics

Prikuplja vrijeme potrebno za osnovne scenarije u programu Outlook – switchfolder, switchmodule, sendmailoutbox, openitemclassic, sendmailtransport. Aktivno se nadzire ima li u podacima problema s neuobičajenim performansama. Koristi se za otkrivanje i dijagnosticiranje problema s performansama, kao i za poboljšanje performansi sa svakim ažuriranjem.

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

#### <a name="officepowerpointsession"></a>**Office.PowerPoint.Session**

Prikupljanje korištenja značajki u svakoj sesiji programa PowerPoint.Ti se podaci koriste za izračun stope neočekivanih izlazaka iz programa PowerPoint prilikom korištenja značajke. Stopa neočekivanih izlazaka iz programa PowerPoint ključni je signal koji jamči da PowerPoint funkcionira prema očekivanjima.

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

Prikuplja podatke o značajci koja se koristila u trenutku neočekivanog zatvaranja sesije programa PowerPoint.  Te su informacije ključne za bilježenje slučajeva neočekivanog zatvaranja programa PowerPoint. Microsoft koristi te podatke za dijagnosticiranje problema da bi jamčio da PowerPoint funkcionira prema očekivanjima.

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

#### <a name="officethisaddinstartupfailed"></a>Office.ThisAddIn.StartupFailed

Prikuplja informacije o iznimci koja se pojavljuje prilikom pokretanja aplikacije Data Streamer. Ti se podaci koriste za praćenje stanja aplikacije. Taj događaj generira dodatak Microsoft Data Streamer za Excel.

Prikupljaju se sljedeća polja:

- **Iznimka** – poziv stogu zbog iznimke

- **Naziv događaja** – naziv događaja je kategorija i oznaka događaja.


### <a name="application-feature-performance-subtype"></a>*Podvrsta performansi značajki aplikacije*

Loše vrijeme odziva ili performanse u situacijama kao što su pokretanje aplikacije ili otvaranje datoteke.

#### <a name="officemanageabilityserviceapplypolicy"></a>Office.Manageability.Service.ApplyPolicy

Ključna telemetrija za praćenje neuspjeha\\uspjeha primjene postavki pravilnika za oblak na registar. LastError govori zašto i gdje primjena pravilnika na registar nije uspjela.

Prikupljaju se sljedeća polja:

  - **Data.ApplyLogMsg** – poruka o iznimci ako je bilo iznimaka tijekom primjene pravilnika

  - **Data.Cid** – dinamički generiran korelacijski identifikator koji se šalje servisu prilikom pozivanja servisa radi dohvaćanja pravilnika za oblak. Koristi se za utvrđivanje korelacije s pozivom koji uzrokuje problem tijekom primjene pravilnika na oblak.

  - **Data.Last Error** – jedna od pet vrijednosti niza (enumeratora) koja se koristi da bi se zabilježilo koja se faza primjene pravilnika izvršavala u trenutku kada je došlo do iznimke

#### <a name="officeoutlookdesktopbootperfmetrics"></a>Office.Outlook.Desktop.BootPerfMetrics

Prikuplja podatke o trajanju pokretanja programa Outlook. Trajanje pokretanja programa Outlook aktivno se nadzire radi otkrivanja i dijagnostike nazadovanja. Koristi se i za dijagnosticiranje eskalacija od strane korisnika, kao i za poboljšavanje performansi pokretanja s vremenom.

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

#### <a name="officeperformanceboot"></a>Office.Performance.Boot

Prikuplja se tijekom pokretanja aplikacije sustava Office. Obuhvaća utvrđivanje je li pokretanje pokrenuto otvaranjem datoteke ili pokretanjem putem izbornika Start, je li to bilo prvo pokretanje aplikacije, koliko memorije aplikacija koristi te je li korisniku prikazano blokirajuće korisničko sučelje. Koristi se za mjerenje brzine pokretanja aplikacija sustava Office i koliko memorije one koriste tijekom pokretanja kako bi se osigurao prihvatljiv korisnički doživljaj.

Prikupljaju se sljedeća polja:

  - **ActivationKind** – je li aplikacija pokrenuta pokretanjem putem izbornika Start, otvaranjem datoteke ili putem OLE automatizacije.

  - **FirstBoot** – je li ovo bilo prvo pokretanje aplikacije.

  - **InitializationDuration** – trajanje u mikrosekundama koje je bilo potrebno za prvo pokretanje procesa sustava Office.

  - **InterruptionMessageId** – je li pokretanje prekinuo dijaloški okvir koji je tražio korisnički unos, ID dijaloškog okvira.

  - **TotalWorkingSetMB** – količina memorije u megabajtima u radnom skupu procesa.

  - **VirtualSetMB** – količina memorije u megabajtima u virtualnom skupu procesa. (samo za MacOS / iOS)

  - **WorkingSetPeakMB** – najveća količina memorije u megabajtima koja se ikad dosad nalazila u radnom skupu procesa.

#### <a name="officeuxofficeinsidercanshowofficeinsiderslab"></a>Office.UX.OfficeInsider.CanShowOfficeInsiderSlab

Praćenje aktivnosti za utvrđivanje može li se ploča Office Insider prikazati korisniku u kartici Račun u korisničkom sučelju Backstage sustava Office.

Prikupljaju se sljedeća polja:

  - **Data_CanShow** – označava može li se ploča Office Insider prikazati korisniku u kartici Račun u korisničkom sučelju Backstage sustava Office.
  
  - **Data_Event** – neiskorišteno

  - **Data_EventInfo** – neiskorišteno

  - **Data_Reason** – neiskorišteno

#### <a name="officeuxofficeinsidershowofficeinsiderdlg"></a>Office.UX.OfficeInsider.ShowOfficeInsiderDlg

Aktivnost koja prati korištenje i performanse dijaloškog okvira Office Insider.

Prikupljaju se sljedeća polja:

  - **Data_AcceptedContactMeNew** – kada uključite u razinu programa Insider i kada je korisnikov odabir uspješno snimljen, označava je li korisnik prihvaćen za kontaktiranje putem tvrtke Microsoft.

  - **Data_DialogChoice** = neiskorišteno
  
  - **Data_DialogId** = neiskorišteno
  
  - **Data_Event** – neiskorišteno
  
  - **Data_EventInfo** – neiskorišteno
  
  - **Data_InsiderLevel** – razina programa Insider kada se dijaloški okvir prvi put prikaže korisniku.
  
  - **Data_InsiderLevelNew** – nova razina programa Insider koju je odabrao korisnik.
  
  - **Data_IsInternalUser** – označava pokreće li se aplikacija putem vjerodajnica računa @microsoft.com.
  
  - **Data_IsInternalUser** – označava može li kod utvrditi pokreće li se aplikacija putem vjerodajnica računa @microsoft.com.
  
  - **Data_OpenNewsletterWebpage** – kada je značajka pretplate na bilten Office Insider omogućena i kada korisnik prijeđe na razinu programa Insider iz Proizvodnje, označava je li aktivirana navigacija preglednika do veze za pretplatu na bilten Office Insider.

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

  - **Data\_IsInternalFile: bool –** istinito ako je datoteka interna datoteka. npr. šablona

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

### <a name="application-activity-error-subtype"></a>*Podvrsta pogreške aktivnosti aplikacije*

Pogreške u funkcioniranju značajke ili korisničkog okruženja.

#### <a name="officeairspacebackendwin32graphicsdriversofthang"></a>Office.AirSpace.Backend.Win32.GraphicsDriverSoftHang 

Pomaže Microsoftu razdvojiti duge blokade upravljačkog programa grafičke kartice od onih kratkih, što pak olakšava donošenje odluka o tome s kojim upravljačkim programima grafičkih kartica možda ima problema. Upravljački program grafičke kartice uzrokovao je blokadu sustava Office, ali utjecaj te blokade još nije poznat

Prikupljaju se sljedeća polja:

  - **Data\_InDeviceCall** – metoda primijenjena na grafičkoj kartici koja je uzrokovala blokadu

  - **Data\_Timeout** – trajanje blokade

#### <a name="officegraphicsarcexceptions"></a>Office.Graphics.ARCExceptions 

Ta informacija za izvješćivanje o iznimkama važna je za procjenu ukupnog stanja grafičkog stoga i identifikaciju dijelova koda u kojima često dolazi do neuspjeha kako bi se odredili prioriteti istrage. Ta informacija za izvješćivanje o iznimkama važna je za procjenu ukupnog stanja grafičkog stoga i identifikaciju dijelova koda u kojima često dolazi do neuspjeha. To inženjeru pomaže utvrditi koji neuspjesi pri vizualizaciji zahvaćaju najveći broj korisnika te nam omogućuje odrediti prioritete istrage da bismo riješili one probleme od kojih će korisnici imati najviše koristi.

Prikupljaju se sljedeća polja:

  - **Data\_HResult** – kod pogreške koji je neuspjeh vratio

  - **Data\_TagCount** – broj svih neuspjeha do kojih je došlo

  - **Data\_TagID** – identifikator neuspjeha do kojeg je došlo

#### <a name="officeoutlookdesktopcalendaracceptcalsharenavigatetosharedfoldererror"></a>Office.Outlook.Desktop.Calendar.AcceptCalShareNavigateToSharedFolder\_Error

Prikuplja informacije kada dođe do bilo kakvog neuspjeha tijekom navigacije u zajedničkom kalendaru. Ti se podaci koriste za praćenje stanja API-ja za zajedničko korištenje kalendara i interakcije programa Outlook sa zajedničkim kalendarima.

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

  - **2 –** broj drugih procesa koji su otvorili tu bazu podataka

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

Prikuplja podatke o uspjehu i neuspjehu akcija Proslijedi, Proslijedi kao privitak i Proslijedi kao iCalendar za jednokratne, ponavljajuće i iznimne odgovore na sastanke u prikazima Pošta, Kalendar i Provjera u programu Outlook. Aktivno se prati ima li neobičnosti u stopi neuspjeha akcija Proslijedi, Proslijedi kao privitak i Proslijedi kao iCalendar. Statistički podaci koji sadrže neobičnosti ukazuju na nesposobnost programa Outlook da izvrši osnovne operacije s kalendarima. Ti se podaci koriste i za dijagnosticiranje drugih eventualno otkrivenih problema s kalendarima.

Prikupljaju se sljedeća polja:

  - **CountExceptionForward – broj iznimaka vezanih uz proslijeđene sastanke**

  - **CountExceptionForwardAsiCal – broj iznimaka vezanih uz sastanke proslijeđene kao iCal**

  - **CountExceptionForwardInSplit – broj iznimaka vezanih uz sastanke proslijeđene s podijeljenog izbornika na vrpci**

  - **CountExceptionForwardWithAttach – broj iznimaka vezanih uz sastanke proslijeđene kao privitak**

  - **CountRecurringForward – broj proslijeđenih ponavljajućih sastanaka**

  - **CountRecurringForwardAsiCal – broj ponavljajućih sastanaka proslijeđenih kao iCal**

  - **CountRecurringForwardInSplit – broj ponavljajućih sastanaka proslijeđenih s podijeljenog izbornika na vrpci**

  - **CountRecurringForwardWithAttach – broj ponavljajućih sastanaka proslijeđenih kao privitak**

  - **CountSingleForward – broj proslijeđenih jednokratnih sastanaka**

  - **CountSingleForwardAsiCal – broj jednokratnih sastanaka proslijeđenih kao iCal**

  - **CountRecurringForwardInSplit – broj jednokratnih sastanaka proslijeđenih s podijeljenog izbornika na vrpci**

  - **CountSingleForwardWithAttach – broj jednokratnih sastanaka proslijeđenih kao privitak**

  - **HResult – ErrorCode**

  - **OlkViewName – označava prikaz Pošta, Kalendar ili Provjera**

#### <a name="officeoutlookdesktopoutlookcalendarusageerrmeetrcptreplyactionsruleo16"></a>Office.Outlook.Desktop.OutlookCalendarUsageErr.MeetRcpt.ReplyActions.Rule.O16

Prikuplja podatke o uspjehu i neuspjehu akcija Odgovori, Odgovori svima, Odgovori izravnom porukom i Odgovori svima izravnom porukom za jednokratne, ponavljajuće i iznimne odgovore na sastanke u prikazima Pošta, Kalendar i Provjera u programu Outlook. Aktivno se prati ima li neobičnosti u stopi neuspjeha akcija Odgovori, Odgovori svima, Odgovori izravnom porukom i Odgovori svima izravnom porukom. Statistički podaci koji sadrže neobičnosti ukazuju na nesposobnost programa Outlook da izvrši osnovne operacije s kalendarima. Ti se podaci koriste i za dijagnosticiranje drugih eventualno otkrivenih problema s kalendarima.

Prikupljaju se sljedeća polja:

  - **CountExceptionReply – broj iznimaka vezanih uz akciju Odgovori u vezi sastanaka**

  - **CountExceptionReplyAll – broj iznimaka vezanih uz akciju Odgovori svima u vezi sastanaka**

  - **CountExceptionReplyAllWithIM – broj iznimaka vezanih uz akciju Odgovori svima izravnom porukom u vezi sastanaka**

  - **CountExceptionReplyWithIM – broj iznimaka vezanih uz akciju Odgovori izravnom porukom u vezi sastanaka**

  - **CountRecurringReply – broj akcija Odgovori u vezi ponavljajućih sastanaka**

  - **CountRecurringReplyAll – broj akcija Odgovori svima u vezi ponavljajućih sastanaka**

  - **CountRecurringReplyAllWithIM – broj akcija Odgovori svima izravnom porukom u vezi ponavljajućih sastanaka**

  - **CountRecurringReplyWithIM – broj akcija Odgovori izravnom porukom u vezi ponavljajućih sastanaka**

  - **CountSingleReply – broj akcija Odgovori u vezi jednokratnih sastanaka**

  - **CountSingleReplyAll – broj akcija Odgovori svima u vezi jednokratnih sastanaka**

  - **CountSingleReplyAllWithIM – broj akcija Odgovori svima izravnom porukom u vezi jednokratnih sastanaka**

  - **CountSingleReplyWithIM – broj akcija Odgovori izravnom porukom u vezi jednokratnih sastanaka**

  - **HResult – ErrorCode**

  - **OlkViewName – označava prikaz Pošta, Kalendar ili Provjera**

#### <a name="officeoutlookdesktopoutlookprivsdlgsingleuserloadfail"></a>Office.Outlook.Desktop.OutlookPrivsDlgSingleUser.LoadFail

To pravilo prikuplja pogreške pri zajedničkom korištenju kalendara prilikom dodavanja novog korisnika (vrste EX ili SMTP) iz adresara. Ti se podaci koriste za dijagnosticiranje i rješavanje problema otkrivenih u dijaloškom okviru Zajedničko korištenje kalendara

Prikupljaju se sljedeća polja:

  - **CountAccountWizardEnd** – koliko se puta zatvorio naslijeđeni dijaloški okvir čarobnjaka

  - **CountCreatePIMAccount** – koliko je puta korisnik stvorio PIM profil

#### <a name="officesystemsystemhealthasserts"></a>Office.System.SystemHealthAsserts

Događaji koje identificira ovaj događaj pomažu nam shvatiti kada je korisnički doživljaj narušen. Mnoge od tih ShipAssert operacija dovode do rušenja, a ovi podaci omogućuju rješavanje mnogih od njih. Prikuplja ShipAssert operacije od proizvoda, što olakšava identifikaciju pogrešaka.

Prikupljaju se sljedeća polja:

Count – broj svih prijavljenih pretpostavki

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

## <a name="device-connectivity-and-configuration-data-events"></a>Događaji koji se odnose na povezivost i konfiguracijske podatke

Ovo su podvrste podataka u toj kategoriji:

- [Povezivost i konfiguracija uređaja](#device-connectivity-and-configuration-subtype)


### <a name="device-connectivity-and-configuration-subtype"></a>*Podvrsta događaja koji se odnose na povezivost i konfiguraciju uređaja*

Stanje mrežne veze i postavke uređaja, kao što je memorija.

#### <a name="officeairspaceairspacelocalblocklistdriverupdated"></a>Office.AirSpace.AirSpaceLocalBlocklistDriverUpdated

Korisnik je ažurirao upravljački program grafičke kartice koji je prije uzrokovao rušenje sustava Office te se zbog toga više ne koristi za vizualizaciju. Obavještava Microsoft da je korisnicima kojima je na raspolaganju bila suboptimalna vizualizacija sada opet dostupna preporučena vizualizacija.

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

Korisnik je ažurirao upravljački program grafičke kartice koji je prije uzrokovao rušenje sustava Office te se zbog toga više ne koristi za vizualizaciju. Obavještava Microsoft da je korisnicima kojima je na raspolaganju bila suboptimalna vizualizacija sada opet dostupna preporučena vizualizacija.

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
