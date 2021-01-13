---
title: Ključni servisi za Office
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
description: Sadrži informacije za administratore sustava Office o ključnim servisima za Office, kao što su "klikom do cilja" i licenciranje, a sadrži i popis događaja te podatkovnih polja za te ključne servise.
hideEdit: true
ms.openlocfilehash: 8934226591ed83c630a1c98e5be70e521c93295e
ms.sourcegitcommit: 862ffbcfc2d7c3722dddb5b008d7b68c9316c675
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/12/2021
ms.locfileid: "49799127"
---
# <a name="essential-services-for-office"></a>Ključni servisi za Office

> [!NOTE]
> Popis proizvoda sustava Office obuhvaćenih ovim informacijama o zaštiti privatnosti potražite u članku [Kontrole za zaštitu privatnosti dostupne za proizvode Office](products-versions-privacy-controls.md).

Office se sastoji od klijentskih softverskih aplikacija i povezanih okruženja osmišljenih radi učinkovitijeg stvaranja, komunikacije i suradnje. Premda kao administrator tvrtke ili ustanove možete upravljati brojnim povezanim sučeljima koja su dostupna vama ili vašim korisnicima, neki su servisi ključni za funkcioniranje sustava Office, pa se ne mogu onemogućiti. To je, primjerice, servis za licenciranje, koji potvrđuje da imate odgovarajuću licencu za korištenje sustava Office. Obavezni servisni podaci o tim servisima prikupljaju se i šalju Microsoftu bez obzira na druge konfigurirane postavke zaštite privatnosti.

Dodatne informacije potražite u sljedećim člancima:

- [Obavezni servisni podaci za Office](required-service-data.md)
- [Povezana okruženja u sustavu Office](connected-experiences.md)

Ako ste administrator za tvrtku ili ustanovu, možda će vas zanimati i sljedeći članci:

- [Pregled kontrola za zaštitu privatnosti za Microsoft 365 Apps za velike tvrtke](overview-privacy-controls.md)
- [Upotreba postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Microsoft 365 Apps za velike tvrtke](manage-privacy-controls.md)
- [Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office za Mac](mac-privacy-preferences.md)
- [Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office na iOS uređajima](ios-privacy-preferences.md)
- [Korištenje postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Office na Android uređajima](android-privacy-controls.md)
- [Korištenje postavkama pravilnika za upravljanje kontrolama za zaštitu privatnosti za aplikacije Office za web](office-web-privacy-controls.md)

## <a name="list-of-essential-services-for-office"></a>Popis ključnih servisa za Office 

U tablici u nastavku naveden je popis ključnih servisa za Office i opis svakog servisa.

| **Servis**  | **Opis**  |
| ------ | ---- |
| [Provjera autentičnosti](#authentication-events) | Provjera autentičnosti servis je koji obuhvaća više platformi, a služi za provjeru valjanosti identiteta korisnika sustava Office.   Nužan je da biste se mogli prijaviti u Office, aktivirati licencu za Office, pristupiti datotekama pohranjenima u oblaku, a omogućuje i dosljedno sučelje u svim sesijama sustava Office na svim uređajima.    |
| [Klikom do cilja](#click-to-run-events) | "Klikom do cilja" tehnologija je za instalaciju koja se koristi za instaliranje i ažuriranje sustava Office u sustavu Windows. Tehnologija provjerava postoji li nova verzija sustava Office i kad postoji, preuzima je i instalira.  Tehnologija "klikom do cilja" otkrit će jesu li vam potrebna ažuriranja sustava Office, uključujući sigurnosna ažuriranja, te će ih preuzeti i instalirati.     |
| [Servis za poboljšanu konfiguraciju (eng. Enhanced Configuration Service, ECS)](#enhanced-configuration-service-ecs-events) | ECS Microsoftu omogućuje da iznova konfigurira instalacije sustava Office bez potrebe za ponovnom implementacijom sustava. Služi za kontroliranje postupnog objavljivanja značajki ili ažuriranja, a učinak objavljivanja prati se na temelju prikupljenih dijagnostičkih podataka. Koristi se i za ublažavanje sigurnosnih problema i problema s performansama neke značajke ili ažuriranja. ECS podržava i promjene konfiguracije povezane s dijagnostičkim podacima da bi se prikupljali odgovarajući događaji. |
| [Licenciranje](#licensing-events)     | Licenciranje je servis u oblaku koji podržava aktivaciju novih instalacija sustava Office te održava licencu na uređajima nakon aktivacije sustava. Servis registrira svaki uređaj i aktivira Office, provjerava status pretplate na Office te upravlja ključevima proizvoda.    |
|[Microsoftovo automatsko ažuriranje (MAU)](#microsoft-autoupdate-mau-events)|Microsoftovo automatsko ažuriranje (MAU) je tehnologija koja se koristi za ažuriranje Microsoftovih aplikacija proizvedenih za macOS, kao što je Office. MAU će otkriti jesu li vam potrebna ažuriranja aplikacije, uključujući sigurnosna ažuriranja, te će ih preuzeti i instalirati.|
|[Sinkronizacija programa OneNote](#onenote-sync-events)|OneNote za Mac podržava samo bilježnice pohranjene na internetu na servisu OneDrive ili u sustavu SharePoint Online. OneNote za Mac kontinuirano sinkronizira sve bilješke korisnika sa servisom OneDrive ili sustavom SharePoint Online. To korisnicima omogućuje otvaranje, pregled i uređivanje bilježnica na svim svojim uređajima tako da su njihove bilježnice uvijek ažurne.
 [Konfiguracija servisa](#services-configuration-events)  | Konfiguracija servisa omogućuje ažuriranje postavki konfiguracije sustava Office radi omogućivanja odnosno onemogućivanja značajki klijenata. Aktivira se svaki put kad se pokrene neka aplikacija sustava Office te sadrži pojedinosti o drugim konfiguracijama i servisima sustava Office. Konfiguracija servisa ujedno kontrolira koji su servisi određeni kao ključni.  |
| [Telemetrija](#telemetry-events)  | Servis za telemetriju služi za prikupljanje dijagnostičkih podataka iz aplikacija sustava Office. Omogućuje prikupljanje obaveznih i neobaveznih dijagnostičkih podataka koje je generirao Office. Odgovoran je i za prikupljanje nekih obaveznih servisnih podataka za Office.  |

## <a name="events-and-data-fields-for-essential-services-for-office"></a>Događaji i podatkovna polja za ključne servise za Office

U sljedećim odjeljcima navode se ove informacije:

- popis događaja za svaki ključni servis
- opis svakog događaja
- popis podatkovnih polja u svakom događaju
- opis svakog podatkovnog polja


## <a name="authentication-events"></a>Događaji provjere autentičnosti

Ti se događaji dijagnostičkih podataka prikupljaju kada Office pokuša dohvatiti token za provjeru autentičnosti, bilo u pozadini ili putem upita korisniku.

### <a name="officeandroidmsaguesttoaad"></a>Office.Android.MSAGuestToAAD

Ovaj događaj pomaže razumjeti od koliko je korisnika zatraženo davanje lozinke za osobni račun tijekom pristupanja poslovnim resursima, jer bi njihov osobni račun mogao biti valjan gost klijentu poslovnog računa.

Ovi podaci nam pomažu razumjeti koliko korisnika prolazi kroz muke prijave u ponovnim upitima radi davanja prioriteta tihom pribavljanju AAD tokena na temelju SAML (Jezik za označavanje sigurnosnih izraza) izraza Microsoftovog računa.

Prikupljaju se sljedeća polja:

- **Tag** - Označava da je korisnik dobio upit za prijavu za osobni račun tijekom pristupanja resursima poslovnog računa.


### <a name="officeidentityfbapromptwin32"></a>Office.Identity.FbaPromptWin32

Prikuplja se kada Office korisniku prikaže upit za prijavu pomoću provjere autentičnosti na temelju obrazaca.

Upiti za provjeru autentičnosti zajedno s pozadinskim pribavljanjem tokena koriste se za utvrđivanje je li korisnik u neispravnom stanju provjere autentičnosti, koje se za korisnika očituje praktički izvanmrežnim stanjem klijenta. Neispravna provjera autentičnosti može i onemogućiti dohvaćanje licence, što uzrokuje potpunu nemogućnost korištenja klijenta.

Upiti za prijavu pomoću provjere autentičnosti na temelju obrazaca (FBA) upotrebljavaju se u nekim scenarijima lokalne provjere autentičnosti i najčešće ne želimo da se to događa jer bi svi trebali koristiti modernu provjeru autentičnosti zbog sigurnosnih slabih točaka povezanih s provjerom autentičnosti na temelju obrazaca.

Prikupljaju se sljedeća polja:

  - **AuthScheme** – korištena shema provjere autentičnosti

  - **DocumentUrlHash** – šifrirano slanje zahtjeva za URL

  - **EndTag** – oznaka ispunjenosti FPA obrasca

  - **Flags** – zastarjelo

  - **FlowTag** – oznaka pokretanja FBA obrasca

  - **LastError** – vraćena šifra pogreške

  - **PromptEndTime** – vrijeme završetka upita

  - **PromptStartTime** – vrijeme početka upita

  - **Result** – označava je li provjera autentičnosti uspjela

  - **SessionEndTime** – vrijeme završetka sesije događaja

  - **Timeout** – vrijeme isteka vremena upita

### <a name="officeidentitysignoutevent"></a>Office.Identity.SignOutEvent

Prikuplja se kad se korisnik odjavi iz sustava Office.

Kad se zna da se korisnik odjavio, moguće je na očekivan način klasificirati druge događaje, kao što su upiti, kako bi se točno izračunali u metrici pouzdanosti / spremnosti za isporuku te se izbjegavaju upozorenja ili vraćanje međuverzija na temelju pogrešne premise da se korisniku prikazuju neočekivani upiti za prijavu.

Prikupljaju se sljedeća polja:

  - **FlowEndTime** – vrijeme završetka radnje odjave

  - **FlowStartTime** – vrijeme početka radnje odjave

  - **IdentityErrorState** – bilo koje stanje pogreške identiteta tijekom odjave

  - **IdentityHashedUniqueId** – šifrirani ID identiteta koji se odjavljuje

  - **IdentityProviderType** – davatelj identiteta koji se odjavljuje

  - **IdentityUniqueID** – ID identiteta koji se odjavljuje

  - **SessionEndTime** – vrijeme završetka sesije događaja

  - **SignOutUserAction** – označava da je korisnik pokrenuo radnju odjave

### <a name="officeidentitysspipromptwin32"></a>Office.Identity.SspiPromptWin32

Prikuplja se kada Office korisniku prikaže upit za prijavu putem Windows SSPI-ja. Upiti za provjeru autentičnosti zajedno s pozadinskim pribavljanjem tokena određuju je li korisnik u neispravnom stanju provjere autentičnosti, koje se očituje izvanmrežnim stanjem klijenta. Neispravna provjera autentičnosti može i onemogućiti dohvaćanje licence, što uzrokuje potpunu nemogućnost korištenja klijenta.

Upiti Windows SSPI-ja koriste se za provjeru autentičnosti u sustavu Exchange (za sinkronizaciju pošte) kad korisnikov resurs sustava Exchange nije postavljen za višestruku provjeru autentičnosti.

Ti događaji, zajedno s događajima prostora za naziv Office.MATS, koriste se u sljedeće svrhe:

1\) utvrđivanje mogu li klijenti uspješno dohvatiti token za provjeru autentičnosti ili su prešli u stanje neispravne provjere autentičnosti

2\) procjenu jesu li promjene u klijentu ili servisu uzrokovale kritično nazadovanje sučelja i pouzdanosti provjere autentičnosti korisnika

3\) u slučaju pogrešaka ti signali šalju važne šifre pogrešaka iz odgovorne komponente (koda klijentskog programa sustava Office, biblioteka za provjeru autentičnosti ili servisa izdavatelja certifikata) koje se mogu koristiti za klasifikaciju hitnosti, dijagnozu i otklanjanje problema

4\) signali služe kao podaci za razne nadzornike spremnosti za isporuku i stanja koji aktiviraju upozorenja da bi se naši inženjeri mogli brzo angažirati i skratiti vrijeme do otklanjanja kritičnih pogrešaka koje blokiraju rad korisnika

Prikupljaju se sljedeća polja:

  - **AllowSavedCreds** – jesu li nove vjerodajnice trajno pohranjene

  - **AuthScheme** – korištena shema provjere autentičnosti

  - **CredsSaved** – jesu li nove vjerodajnice spremljene

  - **DocumentUrlHash** – šifrirano slanje zahtjeva za URL

  - **EndTag** – oznaka završetka upita

  - **NewIdentity**\_ErrorState – označava je li novi identitet valjan

  - **NewIdentity\_HashedUniqueId** – šifrirani ID novog identiteta nakon dovršetka upita

  - **NewIdentity\_ProviderType** – davatelj novog identiteta nakon dovršetka upita

  - **NewIdentity\_UniqueID** – ID novog identiteta nakon dovršetka upita

  - **OutStatus** – označava je li rezultat upita valjan

  - **PromptEndTime** – vrijeme završetka upita

  - **PromptFailedTag** – oznaka da SSPI upit nije uspio

  - **PromptFlow** – oznaka koja je aktivirala SSPI upit

  - **PromptStartTime** – vrijeme početka upita

  - **Proxy** – označava koristi li se proxy

  - **ServerHash** – šifrirana adresa poslužitelja

  - **SessionEndTime** – vrijeme završetka sesije događaja

  - **Timeout** – vrijeme isteka vremena upita

  - **UiMessage** – poruka korisničkog sučelja u upitu

  - **UserNameHash** – šifrirano korisničko ime

### <a name="officeidentitywin32prompt"></a>Office.Identity.Win32Prompt

Prikuplja se kada Office korisniku prikaže upit za prijavu putem višestruke provjere autentičnosti. Upiti za provjeru autentičnosti zajedno s pozadinskim pribavljanjem tokena određuju je li korisnik u neispravnom stanju provjere autentičnosti, koje se očituje izvanmrežnim stanjem klijenta. Neispravna provjera autentičnosti može i onemogućiti dohvaćanje licence, što uzrokuje potpunu nemogućnost korištenja klijenta.

Ti događaji, zajedno s događajima prostora za naziv Office.MATS, koriste se u sljedeće svrhe:

1\) utvrđivanje mogu li klijenti uspješno dohvatiti token za provjeru autentičnosti ili su prešli u stanje neispravne provjere autentičnosti

2\) procjenu jesu li promjene u klijentu ili servisu uzrokovale kritično nazadovanje sučelja i pouzdanosti provjere autentičnosti korisnika

3\) u slučaju pogrešaka ti signali šalju važne šifre pogrešaka iz odgovorne komponente (koda klijentskog programa sustava Office, biblioteka za provjeru autentičnosti ili servisa izdavatelja certifikata) koje se mogu koristiti za klasifikaciju hitnosti, dijagnozu i otklanjanje problema

4\) signali služe kao podaci za razne nadzornike spremnosti za isporuku i stanja koji aktiviraju upozorenja da bi se naši inženjeri mogli brzo angažirati i skratiti vrijeme do otklanjanja kritičnih pogrešaka koje blokiraju rad korisnika.

Prikupljaju se sljedeća polja:

  - **AdalWAMUsed** – oznaka rezultata ako je korišten ADAL-atop-WAM

  - **CallTag** – oznaka pozivatelja korisničkog sučelja za prijavu

  - **Context** – kontekst prijave za upit

  - **EndTagIdentityProviderRequested** – oznaka da je zatražen davatelj identiteta

  - **HrdShownTag** – oznaka da je prikazan HRD dijaloški okvir za prijavu

  - **IdentityProviderResulted** – zatražena vrsta davatelja identiteta

  - **IdPFlowTag** – označava rezultat zahtjeva za identitet

  - **LastLoginDelta** – delta vremena od zadnje uspješne prijave

  - **NewIdentity\_ErrorState** – označava je li identitet valjan nakon upita

  - **NewIdentity\_ProviderType** – vrsta davatelja novog identiteta nakon upita

  - **NewIdentity\_UniqueID** – vraćeni ID novog identiteta nakon upita

  - **PromptCorrelation** – ID korelacije upita za dijagnostičke svrhe

  - **PromptEndTime** – vrijeme završetka upita

  - **PromptStartTime** – vrijeme početka upita

  - **SessionEndTime** – vrijeme završetka sesije događaja

  - **ShowUIResult** – šifra rezultata koju je vratilo korisničko sučelje upita

  - **StartTag** – oznaka da je pokrenut Win32 upit

  - **Timeout** – vrijeme isteka vremena upita

  - **WasIdentitySignedOut** – označava je li korisnik odjavljen

### <a name="officematsactionofficewin32-officematsactionofficewinrt"></a>Office.MATS.actionofficewin32, Office.MATS.actionofficewinrt

Sljedeći se opis odnosi i na Win32 događaje i na WinRT događaje (naziv ovisi o platformi)

Microsoft Auth Telemetry System (MATS) prikuplja se kada Office pokuša dohvatiti token za provjeru autentičnosti, bilo u pozadini ili putem upita korisniku. Kada pokušaj dohvaćanja ne uspije, uvrštavaju se informacije o pogrešci. Korisnici pomoću tih događaja mogu izbjeći prelazak u stanje neispravne provjere autentičnosti tako što:

1\) utvrde mogu li klijenti uspješno dohvatiti token za provjeru autentičnosti ili su prešli u stanje neispravne provjere autentičnosti

2\) procijene uzrokuju li promjene u klijentu ili servisu kritično nazadovanje sučelja i pouzdanosti provjere autentičnosti korisnika

3\) u slučaju pogrešaka ti signali šalju važne šifre pogrešaka iz odgovorne komponente (koda klijentskog programa sustava Office, biblioteka za provjeru autentičnosti ili servisa izdavatelja certifikata) koje se mogu koristiti za klasifikaciju hitnosti, dijagnozu i otklanjanje problema

4\) signali služe kao podaci za razne nadzornike spremnosti za isporuku i stanja koji aktiviraju upozorenja da bi se naši inženjeri mogli brzo angažirati i skratiti vrijeme do otklanjanja kritičnih pogrešaka.

Prikupljaju se sljedeća polja:

  - **Actiontype** – označava koja se biblioteka provjere autentičnosti koristi

  - **Appaudience** – označava je li međuverzija aplikacije za internu ili vanjsku upotrebu

  - **Appforcedprompt** – označava je li aplikacija nadjačala predmemoriju i prisilno prikazala upit

  - **Appname** – naziv aplikacije koja provodi provjeru autentičnosti

  - **Appver** – verzija aplikacije koja provodi provjeru autentičnosti

  - **Askedforcreds** – označava je li aplikacija od korisnika tražila unos vjerodajnica za tu radnju

  - **Authoutcome** – označava uspjeh, neuspjeh ili otkazivanje provjere autentičnosti

  - **Blockingprompt** – označava je li aplikacija izbacila upit na koji korisnik mora reagirati

  - **Correlationid** – GUID korišten za spajanje sa servisnim podacima

  - **Count** – broj događaja u slučajevima agregacije

  - **Data\_accounttype** – označava je li u pitanju osobni račun ili račun tvrtke ili ustanove

  - **Devicenetworkstate** – označava je li korisnik bio na mreži

  - **Deviceprofiletelemetryid** – anonimni ID uređaja koji se koristi za mjerenje iskustva na uređaju

  - **Duration** – trajanje provjere autentičnosti

  - **Duration_Max** – ako je signal skupni, označava maksimalno trajanje za bilo koji skupni događaj.

  - **Duration_Min** – ako je signal skupni, označava minimalno trajanje za bilo koji skupni događaj.

  - **Duration_Sum** – ako je signal skupni, označava zbroj trajanja svih skupnih događaja.

  - **Endtime** – vrijeme završetka događaja provjere autentičnosti

  - **Error** – šifra pogreške u slučaju da provjera autentičnosti nije uspjela

  - **Errordescription** – kratak opis pogreške

  - **Errorsource** – je li pogreška potekla iz servisa, biblioteke za provjeru autentičnosti ili aplikacije

  - **Identityservice** – označava je li pozvan račun za Microsoftove servise (MSA) ili servis Azure Active Directory (AAD)

  - **Interactiveauthcontainer** – označava koja je vrsta upita prikazana

  - **Issilent** – označava je li prikazan upit

  - **Microsoft**\_**ADAL**\_**adal**\_**version** – verzija biblioteke Azure Active Directory Authentication Library (ADAL)

  - **Microsoft\_ADAL\_api\_error\_code** – šifra pogreške koju je biblioteka za provjeru autentičnosti poslala za ovaj pokušaj provjere autentičnosti

  - **Microsoft\_ADAL\_api\_id** – API koji je pozvan za taj pokušaj provjere autentičnosti

  - **Microsoft\_ADAL\_authority** – URL izdavatelja certifikata za Azure Active Directory koji je odgovoran za provjeru autentičnosti korisnika

  - **Microsoft\_ADAL\_authority\_type** – potrošački / Microsoftov ugovor o usluzi (MSA) ili organizacijski / Azure Active Directory (AAD); trenutno uvijek AAD

  - **Microsoft\_ADAL\_authority\_validation\_status** – označava je li provjera autentičnosti provedena na strani servisa

  - **Microsoft\_ADAL\_broker\_app** – označava je li ADAL korišten kao posrednik za provjeru autentičnosti

  - **Microsoft\_ADAL\_broker\_app\_used** – označava naziv posrednika (npr. Windows Account Management)

  - **Microsoft\_ADAL\_broker\_version** – označava verziju posrednika ako se koristi

  - **Microsoft\_ADAL\_cache\_event\_count** – broj događaja predmemoriranja koje je ADAL proveo tijekom dohvaćanja tokena

  - **Microsoft\_ADAL\_cache\_event\_count\_max** – ako je signal skupni, označava maksimalni broj događaja predmemoriranja za bilo koji skupni događaj.

  - **Microsoft\_ADAL\_cache\_event\_count\_min** – ako je signal skupni, označava minimalni broj događaja predmemoriranja za bilo koji skupni događaj.

  - **Microsoft\_ADAL\_cache\_event\_count\_sum** – ako signal skupni, označava zbroj događaja predmemoriranja za sve skupne događaje.

  - **Microsoft\_ADAL\_cache\_read\_count** – označava koliko je puta API čitao iz predmemorije diska. Postoji ako je došlo barem do jednog čitanja.

  - **Microsoft\_ADAL\_cache\_read\_error\_count** – predstavlja broje neuspješnih čitanja iz predmemorije diska. Ako postoji, znači da čitanje barem jednom nije uspjelo.

  - **Microsoft\_ADAL\_cache\_read\_last\_error** – šifra pogreške ADAL-a. Postoji ako čitanje barem jednom nije uspjelo.

  - **Microsoft\_ADAL\_cache\_read\_last\_system\_error** – šifra sistemske pogreške. Postoji ako čitanje barem jednom nije uspjelo.

  - **Microsoft\_ADAL\_cache\_write\_count** – označava koliko je puta API pisao u predmemoriju diska. Postoji ako je došlo barem do jednog pisanja.

  - **Microsoft\_ADAL\_cache\_write\_error\_count** – predstavlja broje neuspješnih pisanja u predmemoriju diska. Postoji ako pisanje barem jednom nije uspjelo.

  - **Microsoft\_ADAL\_cache\_write\_last\_error** – šifra pogreške ADAL-a. Postoji ako čitanje barem jednom nije uspjelo.

  - **Microsoft\_ADAL\_cache\_write\_last\_system\_error** – šifra sistemske pogreške. Postoji ako čitanje barem jednom nije uspjelo.

  - **Microsoft\_ADAL\_client\_id** – raspršeni ID aplikacije AAD

  - **Microsoft\_ADAL\_extended\_expires\_on\_setting** – vrijednost true/false koja označava ima li token produljen životni vijek.

  - **Microsoft\_ADAL\_http\_event\_coun** t – broj HTTP poziva koje je uputio ADAL.

  - **Microsoft\_ADAL\_http\_event\_count\_max** – ako je signal skupni, označava maksimalni broj HTTP poziva koje je ADAL uputio za bilo koji skupni događaj.

  - **Microsoft\_ADAL\_http\_event\_count\_min** – ako je signal skupni, označava minimalni broj HTTP poziva koje je ADAL uputio za bilo koji skupni događaj.

  - **Microsoft\_ADAL\_http\_event\_count\_sum** – ako je signal skupni, označava zbroj HTTP poziva koje je ADAL uputio za sve skupne događaje.

  - **Microsoft\_ADAL\_is\_silent\_ui** – vrijednost true/false koja označava je li ADAL prikazao korisničko sučelje (upit).

  - **Microsoft\_ADAL\_is\_successful** – vrijednost true/false koja označava je li API ADAL-a uspio.

  - **Microsoft\_ADAL\_logging\_pii\_enabled** – vrijednost true/false koja označava je li omogućen način rada za potpuno zapisivanje za ADAL. Ti se podaci bilježe samo lokalno i ne šalju se u telemetriju.

  - **Microsoft\_ADAL\_oauth\_error\_code** – šifra pogreške protokola OAuth koju je vratio servis.

  - **Microsoft\_ADAL\_prompt\_behavior** – prijava ili parametar koji nije HTTP proslijeđen servisu kojim se određuje može li se prikazati korisničko sučelje.

  - **Microsoft\_ADAL\_request\_id** – transakcijski GUID za zahtjev koji je ADAL poslao servisu.

  - **Microsoft\_ADAL\_response\_code** – šifra HTTP odgovora servisa.

  - **Microsoft\_ADAL\_response\_time** – vrijeme koje je bilo potrebno servisu da odgovori ADAL-u.

  - **Microsoft\_ADAL\_response\_time\_max** – ako je signal skupni, maksimalno vrijeme koje je ADAL-u bilo potrebno da se vrati iz API-ja u bilo kojem od skupnih događaja.

  - **Microsoft\_ADAL\_response\_time\_min** – ako je signal skupni, minimalno vrijeme koje je servisu bilo potrebno da odgovori ADAL-u u bilo kojem od skupnih događaja.

  - **Microsoft\_ADAL\_response\_time\_sum** – ako je signal skupni, zbroj vremena koje je ADAL-u bilo potrebno da se vrati iz API-ja za sve skupne događaje.

  - **Microsoft\_ADAL\_rt\_age** – starost tokena za osvježivanje

  - **Microsoft\_ADAL\_server\_error\_code** – šifra pogreške koju je vratio poslužitelj

  - **Microsoft\_ADAL\_server\_sub\_error\_code** – podšifra pogreške koju je poslužitelj vratio, a služi za utvrđivanje zašto zahtjev nije uspio.

  - **Microsoft\_ADAL\_spe\_ring** – vrijednost true/false koja određuje je li korisnik koristio sigurni unutarnji krug produkcijskog korporacijskog okruženja (samo za Microsoftove zaposlenike).

  - **Microsoft\_ADAL\_start\_time** – vrijeme upućivanja poziva ADAL API-ja

  - **Microsoft\_ADAL\_stop\_time** – vrijeme uzvraćanja poziva ADAL API-ja

  - **Microsoft\_ADAL\_telemetry\_pii\_enabled** – vrijednost true/false koja označava je li omogućen način rada za potpunu telemetriju za ADAL. Naziv je pogrešan jer se ne šalje PII/EUII.

  - **Microsoft\_ADAL\_tenant\_id** – GUID koji označava klijent kojem korisnik provjerene autentičnosti pripada.

  - **Microsoft\_ADAL\_token\_acquisition\_from\_context** – opisuje ponašanje ADAL-a ovisno o tokenima u kontekstu provjere autentičnosti.

  - **Microsoft\_ADAL\_token\_type** – token za osvježivanje (RT) ili token za osvježivanje više resursa (MRRT).

  - **Microsoft\_ADAL\_ui\_event\_count** – broj upita prikazanih korisniku. Mogu biti i u pozadini.

  - **Microsoft\_ADAL\_user\_cancel** – vrijednost true/false koja označava je li prozor korisničkog sučelja otkazan.

  - **Microsoft_ADAL_was_request_throttled** – vrijednost true/false koja označava je li događaj ograničen ADAL-om zbog prevelikog broja zahtjeva.
 
  - **Microsoft\_ADAL\_x\_ms\_request\_id** – dodatni ID zahtjeva koji ADAL navodi u HTTP zaglavlju za servis.

  - **Platform** – Win32/WinRT/Android/iOS/Mac

  - **Promptreasoncorrelationid** – za upite, to je ID korelacije drugog događaja koji objašnjava zašto korisnik možda vidi upit za provjeru autentičnosti.

  - **Resource** – resurs za koji korisnik traži token, npr. Exchange ili SharePoint.

  - **Scenarioid** – GUID. Jedan scenarij može obuhvaćati više događaja, npr. scenarij se može odnositi na dodavanje novog računa, ali se u sklopu njega prikazuje više upita. Taj ID omogućuje korelaciju.

  - **Scenarioname** – naziv scenarija kojem ovaj događaj provjere autentičnosti pripada.

  - **Sessionid** – GUID koji određuje sesiju pokretanja

  - **Skdver** –verzija SDK-a MATS klijenta koja je korištena za stvaranje podataka

  - **StartTime** – vrijeme pozivanja MATS API-ja Start\*Action

  - **Tenantid** – GUID koji označava klijent kojem korisnik provjerene autentičnosti pripada (u slučajevima koji nisu ADAL).

  - **Uploadid** – jedinstveni GUID događaja, koristi se za poništavanje dupliciranja

  - **Wamapi** – određuje koji se WAM API poziva

  - **Wamtelemetrybatch** – trenutno se ne koristi. Ubuduće će komponenti WAM omogućiti slanje dodatnih informacija o događaju provjere autentičnosti.


### <a name="officematsoneauthactionmicrosoftofficewin32"></a>Office.MATS.OneAuth.ActionMicrosoftOfficeWin32

Microsoft Auth Telemetry System (MATS) prikuplja se kada Office pokuša dohvatiti token za provjeru autentičnosti, bilo u pozadini ili putem upita korisniku. Kada pokušaj dohvaćanja ne uspije, uvrštavaju se informacije o pogrešci. Korisnici pomoću tih događaja mogu izbjeći prelazak u stanje neispravne provjere autentičnosti tako što:

1) će utvrditi mogu li klijenti uspješno dohvatiti token za provjeru autentičnosti sa servisa ili su prešli u stanje neispravne provjere autentičnosti.

2) će procijeniti uzrokuju li promjene u klijentu ili servisu kritično nazadovanje sučelja i pouzdanosti provjere autentičnosti korisnika

3) u slučaju pogrešaka ti signali šalju važne šifre pogrešaka iz odgovorne komponente (koda klijentskog programa sustava Office, biblioteka za provjeru autentičnosti ili servisa izdavatelja certifikata) koje se mogu koristiti za klasifikaciju hitnosti, dijagnozu i otklanjanje problema

4) Ti signali služe kao podaci za razne nadzornike spremnosti za isporuku i stanja koji aktiviraju upozorenja da bi se naši inženjeri mogli brzo angažirati i skratiti vrijeme do otklanjanja kritičnih pogrešaka.

Prikupljaju se sljedeća polja:

- **Accounttype** – vrsta računa koji se koristi za taj događaj provjere autentičnosti, na primjer, potrošački ili organizacijski.

- **ActionName** – neslužbeni naziv za taj događaj, ako je naveden.

- **Actiontype** – određuje vrstu upotrebljavane biblioteke za provjeru autentičnosti.

- **Appaudience** – označava je li međuverzija aplikacije za internu ili vanjsku upotrebu

- **Appforcedprompt** – označava je li aplikacija nadjačala predmemoriju i prisilno prikazala upit

- **Appname** – naziv aplikacije koja provodi provjeru autentičnosti

- **Appver** – verzija aplikacije koja provodi provjeru autentičnosti

- **Askedforcreds** – označava je li aplikacija od korisnika tražila unos vjerodajnica za tu radnju

- **Authoutcome** – označava uspjeh, neuspjeh ili otkazivanje provjere autentičnosti

- **Blockingprompt** – označava je li aplikacija izbacila upit na koji korisnik mora reagirati

- **Correlationid** – identifikator koji se upotrebljava za spajanje podataka o ovom pojedinačnom događaju sa servisnim podacima

- **Count** – ukupan broj skupnih radnji prijavljenih u ovom jednom događaju podataka.

- **Devicenetworkstate** – označava je li uređaj povezan s internetom.

- **Deviceprofiletelemetryid** – anonimni ID uređaja koji se koristi za mjerenje iskustva autentičnosti i pouzdanosti uređaja.

- **Duration** – trajanje provjere autentičnosti

- **duration_max** – maksimalno trajanje bilo kojeg od skupnih događaja

- **duration_min** – min trajanje bilo kojeg od skupnih događaja

- **duration_sum** – zbroj trajanja svih skupnih događaja

- **endtime** – vrijeme završetka događaja provjere autentičnosti

- **error** – šifra pogreške u slučaju da provjera autentičnosti nije uspjela

- **errordescription** – kratak opis pogreške

- **errorsource** – je li pogreška potekla iz servisa, biblioteke za provjeru autentičnosti ili aplikacije

- **eventtype** – izvještava li ovaj događaja o podatkovnoj točki provjere autentičnosti ili događaju pogreške kvalitete podataka. Koristi se za mjerenje kvalitete podataka.

- **from_cache** – Booleov izraz koji predstavlja je li zapis iz predmemorije jezgre WAM-a ili dodatak

- **hasadaltelemetrija** – upućuje na to je li u knjižnici za provjeru autentičnosti servisa Azure Active Directory dostupna telemetrija za taj događaj.

- **Identityservice** – označava je li pozvan račun za Microsoftove servise (MSA) ili servis Azure Active Directory (AAD)

- **Interactiveauthcontainer** – označava koja je vrsta upita prikazana

- **Issilent** – označava je li prikazan upit ili je to bio tihi (pozadinski) događaj provjere autentičnosti.

- **Microsoft_ADAL_adal_version** – verzija biblioteke Azure Active Directory Authentication Library (ADAL)

- **Microsoft_ADAL_api_error_code** – šifra pogreške koju je biblioteka za provjeru autentičnosti poslala za ovaj pokušaj provjere autentičnosti

- **Microsoft_ADAL_api_id** – API koji je pozvan za taj pokušaj provjere autentičnosti

- **Microsoft_ADAL_application_name** – naziv aplikacije/procesa koji koristi ADAL.

- **Microsoft_ADAL_application_version** – verzija aplikacije koja koristi ADAL.

- **Microsoft_ADAL_authority** – URL izdavatelja certifikata za Azure Active Directory koji je odgovoran za provjeru autentičnosti korisnika

- **Microsoft_ADAL_authority_type** – potrošački / Microsoftov ugovor o usluzi (MSA) ili organizacijski / Azure Active Directory (AAD); trenutačno uvijek AAD

- **Microsoft_ADAL_authority_validation_status**– označava je li provjera autentičnosti provedena na strani servisa

- **Microsoft_ADAL_broker_app** – označava je li ADAL korišten kao posrednik za provjeru autentičnosti

- **Microsoft_ADAL_broker_app_used** – označava naziv posrednika (npr. Windows Account Management)

- **Microsoft_ADAL_broker_version** – označava verziju posrednika ako se koristi

- **Microsoft_ADAL_cache_event_count** – broj događaja predmemoriranja koje je ADAL proveo tijekom dohvaćanja tokena

- **Microsoft_ADAL_cache_event_count_max** – ako je signal skupni, označava maksimalni broj događaja predmemoriranja za bilo koji skupni događaj

- **Microsoft_ADAL_cache_event_count_min** – ako je signal skupni, označava minimalni broj događaja predmemoriranja za bilo koji skupni događaj

- **Microsoft_ADAL_cache_event_count_sum** – ako je signal skupni, označava zbroj događaja predmemoriranja svih skupnih događaja

- **Microsoft_ADAL_cache_read_count** – označava koliko je puta API čitao iz predmemorije diska. Postoji ako je došlo barem do jednog čitanja

- **Microsoft_ADAL_cache_read_error_count** – predstavlja broj neuspješnih čitanja iz predmemorije diska. Postoji ako je barem jedno bilo neuspješno

- **Microsoft_ADAL_cache_read_last_error** – ADAL šifra pogreške. Postoji ako čitanje barem jednom nije uspjelo

- **Microsoft_ADAL_cache_read_last_system_error** – šifra pogreške sustava.  Postoji ako čitanje barem jednom nije uspjelo

- **Microsoft_ADAL_cache_write_count** – označava koliko je puta API pisao u predmemoriju diska. Postoji ako je došlo barem do jednog pisanja

- **Microsoft_ADAL_cache_write_error_count** – predstavlja broj neuspješnih pisanja u predmemoriju diska. Postoji ako je barem jednom bilo neuspješno

- **Microsoft_ADAL_cache_write_last_error**– ADAL šifra pogreške. Postoji ako pisanje barem jednom nije uspjelo

- **Microsoft_ADAL_cache_write_last_system_error** – šifra pogreške sustava. Postoji ako pisanje barem jednom nije uspjelo

- **Microsoft_ADAL_client_id** – raspršeni ID aplikacije servisa Azure Active Directory

- **Microsoft_ADAL_device_id** – ID lokalnog uređaja koji generira ADAL.

- **Microsoft_ADAL_error_domain** – domena/komponenta koja je generirala šifru pogreške.

- **Microsoft_ADAL_error_protocol_code** – šifra pogreške protokola OAuth koji je vratio servis, snimio ADAL.

- **Microsoft_ADAL_extended_expires_on_setting** – vrijednost true/false koja označava ima li token produljen životni vijek

- **Microsoft_ADAL_http_event_count** – broj HTTP zahtjeva koje generira ADAL.

- **Microsoft_ADAL_idp** – Davatelj identiteta (IDP) koji koristi ADAL.

- **Microsoft_ADAL_network_event_count** – broj mrežnih poziva koje je uputio ADAL

- **Microsoft_ADAL_http_event_count_max** – ako je taj signal skupni, označava maksimalni broj http poziva koje je uputio ADAL

- **Microsoft_ADAL_http_event_count_min** – ako je taj signal skupni, označava minimalni broj http poziva koje je uputio ADAL

- **Microsoft_ADAL_http_event_count_sum** – ako je taj signal skupni, označava zbroj poziva koje je uputio ADAL

- **Microsoft_ADAL_network_event_count_max** – ako je taj signal skupni, označava maksimalni broj mrežnih poziva koje je ADAL uputio za bilo koji skupni događaj

- **Microsoft_ADAL_network_event_count_min** – ako je taj signal skupni, označava minimalni broj mrežnih poziva koje je ADAL uputio za bilo koji skupni događaj

- **Microsoft_ADAL_network_event_count_sum** – ako je taj signal skupni, označava zbroj mrežnih poziva koje je ADAL uputio za bilo koji skupni događaj

- **Microsoft_ADAL_is_silent_ui** – vrijednost true/false koja označava je li ADAL prikazao korisničko sučelje (upit)

- **Microsoft_ADAL_is_successfull** – vrijednost true/false koja označava je li API ADAL-a uspio (macOS)

- **Microsoft_ADAL_is_successful** – vrijednost true/false koja označava je li API ADAL-a uspio

- **Microsoft_ADAL_logging_pii_enabled** – vrijednost true/false koja označava je li omogućen način rada za potpuno zapisivanje za ADAL. Ti se podaci bilježe samo lokalno i ne šalju se u telemetriju

- **Microsoft_ADAL_ntlm** – vrijednost true/false koja označava je li ADAL upotrijebio osnovnu aut. (NTLM).

- **Microsoft_ADAL_oauth_error_code** – šifra pogreške protokola OAuth koju je vratio servis

- **Microsoft_ADAL_prompt_behavior** – prijava ili parametar koji nije mrežni proslijeđen servisu kojim se određuje može li se prikazati korisničko sučelje

- **Microsoft_ADAL_request_id** – transakcijski GUID za zahtjev koji je ADAL poslao servisu

- **Microsoft_ADAL_response_code** – kôd mrežnog odgovora sa servisa

- **Microsoft_ADAL_response_time** – vrijeme koje je bilo potrebno servisu da odgovori ADAL-u.

- **Microsoft_ADAL_response_time_max** – ako je signal skupni, maksimalno vrijeme koje je ADAL-u bilo potrebno da se vrati iz API-ja u bilo kojem od skupnih događaja

- **Microsoft_ADAL_response_time_min** – ako je signal skupni, označava minimalno vrijeme koje je servisu bilo potrebno da odgovori ADAL-u u bilo kojem od skupnih događaja

- **Microsoft_ADAL_response_time_sum** – ako je signal skupni, označava zbroj vremena koje je ADAL-u bilo potrebno da se vrati iz API-ja za sve skupne događaje.

- **Microsoft_ADAL_rt_age**– starost tokena za osvježavanje

- **Microsoft_ADAL_server_error_code** – šifra pogreške koju je vratio poslužitelj

- **Microsoft_ADAL_server_sub_error_code** – podšifra pogreške koju je poslužitelj vratio, a služi za utvrđivanje zašto zahtjev nije uspio

- **Microsoft_ADAL_spe_info** – vrijednost true/false koja određuje je li korisnik koristio sigurni unutarnji krug produkcijskog korporacijskog okruženja (samo za Microsoftove zaposlenike).

- **Microsoft_ADAL_spe_ring** – vrijednost true/false koja određuje je li korisnik koristio sigurni unutarnji krug produkcijskog korporacijskog okruženja (samo za Microsoftove zaposlenike).

- **Microsoft_ADAL_start_time**– vrijeme upućivanja poziva ADAL API-ja

- **Microsoft_ADAL_status** – status uspjeha/neuspjeha cjelokupnog pozivanja ADAL-a

- **Microsoft_ADAL_stop_time** – vrijeme uzvraćanja poziva ADAL API-ja

- **Microsoft_ADAL_telemetry_pii_enabled**– vrijednost true/false koja označava je li omogućen način rada za potpunu telemetriju za ADAL. Naziv je pogrešan jer se ne šalje PII/EUII

- **Microsoft_ADAL_tenant_id** – GUID koji označava klijenta kojem korisnik provjerene autentičnosti pripada

- **Microsoft_ADAL_token_acquisition_from_context** – opisuje ponašanje ADAL-a ovisno o tokenima u kontekstu provjere autentičnosti

- **Microsoft_ADAL_token_frt_status** – status tokena za osvježavanje: je li isproban, nije potreban, nije pronađen ili je izbrisan.

- **Microsoft_ADAL_token_mrrt_status** – status MultiResourceRefreshToken: je li isproban, nije potreban, nije pronađen ili je izbrisan.

- **Microsoft_ADAL_token_rt_status** – status tokena za osvježavanje: je li isproban, nije potreban, nije nađen ili je izbrisan.

- **Microsoft_ADAL_token_type** – token za osvježivanje (RT) ili token za osvježivanje više resursa (MRRT).

- **Microsoft_ADAL_ui_event_count** – broj upita prikazanih korisniku. Mogu biti i u pozadini

- **Microsoft_ADAL_user_cancel** – vrijednost true / false koja označava je li prozor korisničkog sučelja otkazan

- **Microsoft_ADAL_x_ms_request_id** – dodatni ID zahtjeva koji ADAL navodi u mrežnom zaglavlju za servis

- **Microsoft_ADAL_x_client_cpu** – informacije o CPU arhitekturi uređaja

- **Microsoft_ADAL_x_client_os** – verzija OS-a uređaja.

- **Microsoft_ADAL_x_client_sku** – naziv SKU-a OS-a uređaja.

- **Microsoft_ADAL_x_client_ver** – verzija biblioteke ADAL-a.

- **MSAL_all_error_tags** – sve oznake pogrešaka s kojima se susrela Microsoft Authentication Library (MSAL) za vrijeme tijeka provjere autentičnosti.

- **MSAL_api_error_code** – ako MSAL naiđe na pogrešku u OS-u, ovdje su pohranjene šifre pogrešaka platforme.

- **MSAL_api_error_context** – niz koji sadrži dodatne čovjeku čitljive pojedinosti o zadnjoj pogrešci na koju je MSAL naišla. 

- **MSAL_api_error_tag** – jedinstveni niz za mjesto u kodu gdje se pojavila ta pogreška.

- **MSAL_api_name** – naziv API-ja za MSAL najviše razine pozvanog radi pokretanja tog tijeka provjere autentičnosti.

- **MSAL_api_status_code** – kôd statusa MSAL vraćen je za taj rezultat tijeka provjere autentičnosti.

- **MSAL_auth_flow** – koraci koje je MSAL pokušao za vrijeme tog tijeka provjere autentičnosti (AT, PRT, LRT, FRT, ART, IRT). Odvojen simbolom okomite crte "|" za jednostavno raščlanjivanje.

- **MSAL_auth_flow_last_error** – šifra pogreške koju smo primili od poslužitelja u okviru predzadnje stavke u AuthFlowu. (Primj.: If AuthFlow = „PRT|LRT ", greška PRT-a bila bi u AuthFlowLastError).

- **MSAL_authority_type** – označava je li ovaj zahtjev za korisnika bio u: AAD, vanjski ili MSA.

- **MSAL_broker_app_used** – označava je li u ovom tijeku provjere autentičnosti korištena aplikacija posrednika.

- **MSAL_client_id** – ID klijenta aplikacije za pozivanje

- **MSAL_correlation_id** – jedinstveni GUID za taj događaj, koji se upotrebljava za pridruživanje radnjama u zapisnicima klijenta, poslužitelja i aplikacija.

- **MSAL_delete_token** – popis tokena koji su izbrisani iz predmemorije za vrijeme tog tijeka provjere autentičnosti.

- **MSAL_http_call_count** – broj HTTP poziva koje je MSAL izvršio za vrijeme tijeka provjere autentičnosti.

- **MSAL_is_successful** – označava je li tijek provjere autentičnosti bio uspješan.

- **MSAL_last_http_response_code** – ako je MSAL izvršio jedan ili više HTTP poziva, to je zadnji kôd odgovora HTTP-a koji smo primili.

- **MSAL_msal_version** – označava niz verzije MSAL, oblik X. X. X + („OneAuth“, „local" ili izvršite raspršivanje).

- **MSAL_read_token** – tokeni koji su se pročitali iz predmemorije (AT, ART, FRT, LRT, IRT, PRT, EAT [EAT = AT koji je istekao je pročitan, ali odbačen]).

- **MSAL_read_token_last_error** – ako je MSAL naišla na pogrešku prilikom čitanja predmemorije, ovdje ćemo pohraniti informacije. (Primjer: pogreška čitanja diska iz OS-a, pogreška privjeska za ključeve u macOS-u).

- **MSAL_request_duration** – označava koliko je zahtjevu trebalo od trenutka pozivanja API-ja najviše razine za MSAL do vraćanja rezultata.

- **MSAL_request_id** – ID zahtjeva za zadnji poziv koji smo unijeli u Microsoftov servis sigurnog tokena.

- **MSAL_server_error_code** – označava numeričku šifru pogreške Microsoftovog servisa sigurnog tokena ako smo ga primili.

- **MSAL_server_spe_ring** – informacije o krugu produkcijskog korporacijskog okruženja Microsoftovog servisa sigurnog tokena, ako smo ga primili.

- **MSAL_server_suberror_code** – niz podšifre pogreške Microsoftovog servisa sigurnog tokena, ako smo je primili.

- **MSAL_start_time** – označava vrijeme pokretanja zahtjeva MSAL-a na javnom API-ju najviše razine.

- **MSAL_stop_time** označava vrijeme u kojem je MSAL dovršila obradu zahtjeva i vratila rezultat pozivatelju.

- **MSAL_tenant_id** – označava Microsoftov GUID koji prepoznaje klijenta u kojem postoji korisnik.

- **MSAL_ui_event_count** – označava broj upita korisničkog sučelja MSAL-a prikazan na zaslonu.

- **MSAL_wam_telemetry** – sadrži skup WAM telemetrijskih podataka u nizu JSON koji će se raščlaniti i pretvoriti u polja u ovom dokumentu koja potiču iz WAM-a.

- **MSAL_was_request_throttled** – točno ako je MSAL ograničila ovaj zahtjev i spriječila ga da napadne mrežu. Ako je ovo ikad točno, u aplikaciji za pozivanje najvjerojatnije se nalazi petlja.

- **MSAL_write_token** – tokeni koji su pisani u predmemoriji (AT, ART, FRT, LRT, IRT, PRT, EAT [EAT = AT koji je istekao je pročitan, ali odbačen]).

- **MSAL_read_token_last_error** – ako je MSAL naišla na pogrešku prilikom pisanja u predmemoriju, ovdje ćemo pohraniti informacije. (Primjer: pogreška čitanja diska iz OS-a, pogreška privjeska za ključeve u macOS-u).

- **oneauth_api** – API za OneAuth koji je pozvan za taj pokušaj provjere autentičnosti.

- **oneauth_transactionuploadid** – GUID koji određuje pojedinačni poziv API-ja za OneAuth.

- **oneauth_version** – verzija SDK-a za OneAuth.

- **Platform** – označava platformu OS-a (0: Windows Desktop; 1: Android; 2: iOS; 3: macOS; 4: UWP)

- **Promptreasoncorrelationid** – označava identifikator korelacije koji se može upotrebljavati za traženje prethodnog događaja provjere autentičnosti, koji se upotrebljava za objašnjenje zašto je korisnik zatražio provjeru autentičnosti.

- **Resource** – označava resurs za koji se traži token.

- **Scenarioid** – veći broj događaja može pripadati jednom scenariju, npr. scenarij možda dodaje novi račun, ali u sklopu tog scenarija postoji više upita. Ovaj identifikator omogućuje korelaciju tih povezanih događaja.

- **Scenarioname** – označava naziv scenarija aplikacije u kojem je bila potrebna provjera autentičnosti, npr. prvo pokretanje, provjera licenciranja itd.

- **Scope** – označava opseg za koji se traži token.

- **Sdkver** – označava verziju biblioteke Microsoft Auth Telemetry System koja se upotrebljava za izradu tih podataka

- **SessionId** – označava identifikator sesije pokretanja

- **Starttime** – vrijeme kada je započeo događaj provjere autentičnosti.

- **Tenantid** – GUID koji označava klijent kojem korisnik provjerene autentičnosti pripada (u slučajevima koji nisu ADAL)

- **Uploadid** – jedinstveni GUID događaja, koristi se za poništavanje dupliciranja

- **wamapi** – određuje koji će se API za Windows Web Account Management (WAM) pozvati

- **wamtelemetrybatch** – trenutačno se ne koristi. Ubuduće će komponenti WAM omogućiti slanje dodatnih informacija o događaju provjere autentičnosti

- **WAM_account_join_on_end** – stanje pridruživanja računa na kraju operacije WAM.  Moguće vrijednosti: „primary", „secondary“, „not_joined"

- **WAM_account_join_on_start** – stanje pridruživanja računa na početku operacije WAM.  Moguće vrijednosti: „primary", „secondary“, „not_joined"

- **WAM_api_error_code** – ako je došlo do odgovora na pogrešku iz dodatka AAD WAM, to će polje postojati te će sadržavati tu šifru pogreške

- **WAM_authority** – niz koji sadrži URL autoriteta – to bi trebao biti login.windows.net krajnju točku koja se koristi

- **WAM_broker_version** – prisutno kada se upotrebljava WAM, ovo je niz verzije posrednika

- **WAM_cache_event_count** – označava broj događaja predmemoriranja u WAM-u unutar operacije

- **WAM_client_id** – identifikator za pridruživanje sa servisnim podacima, time se označava klijentska aplikacija.

- **WAM_correlation_id** – identifikator za pridruživanje događajima sa servisnim podacima

- **WAM_device_join** – označava stanje pridruživanja uređaja; moguće vrijednosti su „aadj", „haadj"

- **WAM_network_event_count** – prisutno ako se dogodio najmanje jedan mrežni poziv; broj mrežnih poziva na servis za tu operaciju WAM

- **WAM_network_status** – prisutno ako se dogodio najmanje jedan mrežni poziv, sadrži šifru pogreške HTTP-a ako mrežni zahtjev nije uspio.

- **WAM_idp** – određuje je li korišten WAM potrošački ili organizacijski dodatak za provjeru autentičnosti.

- **WAM_is_cached** – određuje je li odgovor koji je pružio WAM dohvaćen iz predmemorije.

- **WAM_oauth_error_code** – sadrži šifru pogreške koji je servis vratio kao dio protokola oauth.

- **WAM_prompt_behavior** – određuje je li ovaj upit zatražila aplikacija, ili, može li ovaj zahtjev preskočiti pitanja ako može neprimjetno provjeriti autentičnost.

- **WAM_provider_id** – Određuje Microsoftovu krajnju točku za ustanovu koja se koristi za scenarij provjere autentičnosti.

- **WAM_redirect_uri** – URI za preusmjeravanje registriran za aplikaciju u servisu Azure Active Directory.

- **WAM_resource** – označava resurs za koji se traži token.

- **WAM_server_error_code** – šifra pogreške koju je servis vratio u WAM.

- **WAM_server_sub_code** – dodatna šifra pogreške koja se upotrebljava za daljnje razbijanje uzroka kvara koji je vratio servis.

- **WAM_silent_code** – šifra pogreške koja je naišla na tihi interni pokušaj WAM-a, prije nego što pošalje upit korisniku.

- **WAM_silent_mats** – označava neiskorišteno.

- **WAM_silent_message** – označava poruku o pogrešci povezanu sa unutarnjim tihim pokušajima WAM-a, prije nego što pošalje upit korisniku.

- **WAM_silent_status** – označava status uspjeha/neuspjeha za tihi interni pokušaj WAM-a, prije nego što pošalje upit korisniku.

- **WAM_tenant_id** – identifikator za klijenta kojem pripada korisnik provjerene AAD autentičnosti, ako ga vraća servis

- **WAM_ui_visible** – prisutno ako je korisniku prikazan najmanje jedan prozor korisničkog sučelja, bilo ‘true’ ili ‘false’

- **WAM_x_ms_clitelem** – prisutno ako servis vrati zaglavlje “x-ms-clitelem"


### <a name="officematsoneauthtransactionmicrosoftofficewin32"></a>Office.MATS.OneAuth.TransactionMicrosoftOfficeWin32

Microsoft Auth Telemetry System (MATS) prikuplja se kada Office pokuša dohvatiti token za provjeru autentičnosti, bilo u pozadini ili putem upita korisniku. Ovaj je događaj nadređen jednom ili više ActionMicrosoftOffice događaja, što omogućuje grupiranje povezanih događaja. Korisnici pomoću tih događaja mogu izbjeći prelazak u stanje neispravne provjere autentičnosti tako što:

1) će utvrditi mogu li klijenti uspješno dohvatiti token za provjeru autentičnosti sa servisa ili su prešli u stanje neispravne provjere autentičnosti.

2) će procijeniti uzrokuju li promjene u klijentu ili servisu kritično nazadovanje sučelja i pouzdanosti provjere autentičnosti korisnika

3) u slučaju pogrešaka ti signali šalju važne šifre pogrešaka iz odgovorne komponente (koda klijentskog programa sustava Office, biblioteka za provjeru autentičnosti ili servisa izdavatelja certifikata) koje se mogu koristiti za klasifikaciju hitnosti, dijagnozu i otklanjanje problema

4) Ti signali služe kao podaci za razne nadzornike spremnosti za isporuku i stanja koji aktiviraju upozorenja da bi se naši inženjeri mogli brzo angažirati i skratiti vrijeme do otklanjanja kritičnih pogrešaka.

Prikupljaju se sljedeća polja:

- **Actiontype** – „oneauthtransaction" je jedina vrijednost.

- **Appaudience** – označava ciljnu skupinu aplikacije (automatizacija, pretprodukcija ili produkcija)

- **Appname** – označava naziv aplikacije

- **Appver**– označava verziju aplikacije

- **Authoutcome** – označava uspjeh, neuspjeh ili otkazivanje provjere autentičnosti

- **Correlationid** – identifikator koji se upotrebljava za spajanje podataka o ovom pojedinačnom događaju sa servisnim podacima

- **Count** – označava koliko je puta došlo do pogreške

- **Devicenetworkstate** – stanje mreže uređaja

- **Deviceprofilatelemetryid** – ID telemetrije profila uređaja (niz kojim se koristi MATS za određivanje određenog uređaja)

- **duration_max** – označava minimalno trajanje, u milisekundama, transakcija koje se skupljaju na tom signalu.

- **duration_min** – označava maksimalno trajanje, u milisekundama, transakcija koje se skupljaju na tom signalu.

- **duration_sum** – označava zbroj trajanja transakcija koje se skupljaju na tom signalu u milisekundama.

- **Endtime** – označava vrijeme u kojem je završila transakcija OneAuth.

- **Error** – OneAuth kôd statusa.

- **Eventtype** – označava vrstu događaja

- **Issilent** – False ako je prikazano korisničko sučelje; true ako je riječ o događaju u pozadini.

- **oneauth_api** – određuje javni API za OneAuth koji je pozvan.

- **oneauth_Domain** – ako je poziv API-ja uzrokovao pogrešku, to je sistemska domena te pogreške.

- **oneauth_ErrorCode** – šifra pogreške koja predstavlja interno stanje pogreške za OneAuth. Zamjenjuje staro polje oneauth_errortag field.

- **oneauth_errortag** – numerički identifikator za redak kôda koji je odgovoran za generiranje pogreške.

- **oneauth_ExecutionFlow** – niz oznaka koje identificiraju put koda koji je preuzeo ovaj API.

- **oneauth_internalerror** – šifra pogreške koja predstavlja interno stanje pogreške za OneAuth.

- **oneauth_ServerErrorCode** – pogreška poslužitelja vraćena u OneAuth po završetku tog poziva API-ja, ako se naiđe na nju.

- **oneauth_SystemErrorCode** – sistemska pogreška vraćena u OneAuth po završetku tog poziva API-ja, ako se naiđe na nju.

- **oneauth_Tag** – oznaka OneAuth koja označava konačno mjesto u kodu postignuto na kraju ovog poziva API-ja.

- **oneauth_transactionuploadid** – određuje nasumično generirani interni GUID koji se preslikava na određeno pozivanje OneAuth API-ja.

- **oneauth_version** – verzija SDK-a za OneAuth.

- **Platform** – označava platformu OS-a (0: Win32; 1: Android; 2: iOS; 3: macOS; 4: WinRT

- **Scenarioname** – naziv scenarija za koji je potrebna provjera autentičnosti, a određuje ga aplikacija za pozivanje.

- **Schemaver**– označava verziju sheme

- **Sdkver** – označava verziju SDK-a MATS-a

- **Sessionid** – označava ID sesije

- **severityError** – označava ozbiljnost

- **startime** – označava vrijeme u kojem je započela transakcija OneAuth.

- **Timestamp** – označava vremensku oznaku

- **Type** – označava vrstu pogreške

- **Uploaded** – Jedinstveni identifikator za ovaj određeni događaj, u svrhe uklanjanja duplikata.


### <a name="onenotesigninssoexternalappsaccountfound"></a>OneNote.SignIn.SSOExternalAppsAccountFound
 
Ovaj se događaj bilježi kada se na popisu računa koje nudi TokenSharingManager pronađe račun s valjanim tokenom osvježavanja.  Taj je scenarij specifičan za jedinstvenu prijavu (SSO).
 
Prikupljaju se sljedeća polja:
 
- **AccountType** - Bilježi vrstu računa

- **ProviderPackageID**-zapisuje ID paketa aplikacije koja je dala taj račun

### <a name="onenotesigninssoexternalappsinvalidaccount"></a>OneNote.SignIn.SSOExternalAppsInvalidAccount

Taj se događaj bilježi kada se prilikom pokušaja dohvaćanja tokena osvježavanja za račun na popisu računa koje nudi TokenSharingManager dogodi pogreška. Taj je scenarij specifičan za jedinstvenu prijavu (SSO)
 
Prikupljaju se sljedeća polja:
 
- **RawError** - zapisuje pogrešku RAW dobivenu prilikom pokušaja dohvaćati tokena osvježavanja pomoću danog računa

### <a name="onenotestickynotesfetchtokencompleted"></a>OneNote.StickyNotes.FetchTokenCompleted
 
Ovaj je događaj zapisan nakon provjere autentičnosti, po dovršetku dohvaćanja tokena osvježavanja.
 
Prikupljaju se sljedeća polja:
 
- **ErrorMessage** - ako dohvaćanje tokena nije uspjelo, to bi zabilježilo poruku o pogrešci 

- **Result** - zapisuje rezultat pokušaja dohvaćanja tokena

- **StickyNoteAccountType** - bilježi vrstu računa za koji je aplikacija pokušavala dohvatiti token osvježavanja


## <a name="click-to-run-events"></a>Događaji tehnologije "klikom do cilja"

### <a name="officeclicktorunbootstrapper"></a>Office.ClickToRun.Bootstrapper 

Podaci o instalaciji i inventaru sustava Office prikupljeni kada korisnik pokrene setup.exe sustava Office radi izmjene instaliranih proizvoda sustava Office. Koristi se za mjerenje uspjeha/pogrešaka instalacije sustava Office koju je u potpunosti pokrenuo korisnik, uključujući provjere preduvjeta.

Prikupljaju se sljedeća polja:

  - **Data\_BootStrapperStateFailure\_ErrorCode** – šifra pogreške zbog koje radnja nije uspjela

  - **Data\_BootStrapperStateFailure\_ErrorSource** – funkcija koja nije uspjela

  - **Data\_BootStrapperStateFailure\_FailingState** – dio datoteke bootstrapper koji nije uspio

  - **Data\_BootStrapperStateFailure\_OExceptionType** – vrsta iznimke zbog koje radnja nije uspjela

  - **Data\_Culture** – kultura u kojoj se pokreće ovaj exe, npr. hr-hr

  - **Data\_HashedOLSToken** – raspršivanje sha-256 tokena koji nam OLS servis pošalje

  - **Data\_Platform** – 64-bitna ili 32-bitna instalacija

  - **Data\_PrereqFailure\_Type** – neispunjeni preduvjet, tj. operacijski sustav nije podržan

  - **Data\_ProductReleaseId** – proizvod koji instaliramo, npr. Microsoft 365 Apps za velike tvrtke

### <a name="officeclicktoruncorruptioncheck"></a>Office.ClickToRun.CorruptionCheck

Podaci o instalaciji i inventaru sustava Office prikupljeni kada klijent tehnologije "klikom do cilja" pokrene provjeru oštećenja radi potvrđivanja jesu li binarne datoteke sustava Office točne. Koristi se za mjerenje oštećenja binarnih datoteka sustava Office i utvrđivanje koje su binarne datoteke oštećene.

Prikupljaju se sljedeća polja:

  - **Data\_Active –** trenutačni manifest strujanja koji provjeravamo na disku

  - **Data\_ActivePackages –** označava pakete koje manifest sadrži

  - **Data\_ActiveVersion –** verzija manifesta

  - **Data\_AddFileCount –** broj datoteka koje dodajemo

  - **Podataka\_AddFileFiles –** uzorak datoteka koje dodajemo

  - **Data\_CompressionLevel –** način kompresije datoteka

  - **Data\_CorruptionCheckLevel –** koliko duboko provjeravamo oštećenja, faze

  - **Data\_CorruptSizeCount –** broj datoteka oštećene veličine

  - **Data\_CorruptSizeFiles –** uzorak datoteka oštećene veličine

  - **Data\_CorruptVersionCount –** broj datoteka oštećene verzije

  - **Data\_CorruptVersionFiles –** uzorak datoteka oštećene verzije

  - **Data\_FileBadDigestCount –** broj datoteka koje se nisu uspjele otvoriti

  - **Data\_FileBadDigestFiles –** uzorak datoteka koje se nisu mogle otvoriti

  - **Data\_FileNotSignedCount –** broj nepotpisanih datoteka

  - **Data\_FileNotSignedFiles –** uzorak nepotpisanih datoteka

  - **Data\_FileNotTrustedCount –** broj datoteka koje se ne smatraju pouzdanima

  - **Data\_FileNotTrustedFiles –** uzorak datoteka koje ne smatramo pouzdanima

  - **Data\_IncompleteFileCount –** broj datoteka koje su naizgled nepotpune

  - **Data\_IncompleteFileFiles –** uzorak nepotpunih datoteka

  - **Data\_KeepFileCount –** broj datoteka koje ne diramo

  - **Data\_KeepFileFiles –** uzorak datoteka koje zadržavamo

  - **Data\_KeepIncompleteFileCount –** broj datoteka koje ne mijenjamo unatoč tome što su nepotpune

  - **Data\_KeepIncompleteFileFiles –** uzorak datoteka koje zadržavamo, a nepotpune su

  - **Data\_MismatchSizeCount –** broj datoteka koje se veličinom ne podudaraju s manifestom

  - **Data\_MismatchSizeFiles –** uzorak datoteke nepodudarne veličine

  - **Data\_MismatchVersionCount –** broj datoteka čija je verzija drukčija od manifesta

  - **Data\_MismatchVersionFiles –** uzorak datoteka nepodudarnih verzija

  - **Data\_MissingFileCount –** broj datoteka koje nedostaju

  - **Data\_MissingFileFiles –** uzorak datoteka koje nedostaju

  - **Data\_NotToBeStreamedFileCount –** broj datoteka koje ne prenosimo strujanjem

  - **Data\_RemoveFileCount –** broj datoteka koje uklanjamo

  - **Data\_RemoveFileFiles –** uzorak datoteka koje uklanjamo

  - **Data\_StreamUnitsMismatchCount –** broj datoteka s jedinicama koje nisu podudarne s manifestom

  - **Data\_StreamUnitsMismatchFiles –** uzorak datoteka u čijem strujanju jedinice nisu podudarne

  - **Data\_TimeElapsed –** vrijeme koje je bilo potrebno za provjeru oštećenja

  - **Data\_UpdateFileCount –** broj datoteka koje ažuriramo

  - **Data\_UpdateFileFiles –** uzorak datoteka koje dodajemo

  - **Data\_Working –** novi manifest koji provjeravamo

  - **Data\_WorkingVersion –** verzija novog manifesta

### <a name="officeclicktorunmachinemetadata"></a>Office.ClickToRun.MachineMetadata

Podaci o instalaciji i inventaru sustava Office koji sadrže potrebne metapodatke za instalaciju i inventuru te se koriste za utvrđivanje točne osnove za instalaciju.

Prikupljaju se sljedeća polja:

  - **Data\_C2RClientVer** – verzija datoteke OfficeClickToRun.exe na računalu

  - **Data\_OfficeBitness** – broj bitova instalacije sustava Office, x86 ili x64

  - **Data\_OfficeVersion** – verzija instaliranog sustava Office

  - **Data\_Sku** – inventarni broj instaliranog proizvoda, npr. Microsoft 365 Apps za velike tvrtke

  - **Data\_SqmMachineID** – jedinstveni ID računala koji koristi identifikator ažuriranja sustava Office Windows SQM Data\_SusClientID- Machine

### <a name="officeclicktorunodt"></a>Office.ClickToRun.ODT

Podaci o instalaciji i inventaru sustava Office prikupljeni kada IT administrator pokrene setup.exe s tehnologijom „klikom do cilja” alata za implementaciju sustava Office radi izmjene proizvoda sustava Office koje su instalirali korisnici. Koristi se za mjerenje uspjeha/pogrešaka instalacija sustava Office koje je u potpunosti pokrenuo administrator, uključujući provjere preduvjeta.

Prikupljaju se sljedeća polja:

  - **Data\_BootStrapperStateFailure\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela

  - **Data\_BootStrapperStateFailure\_ErrorSource –** funkcija koja nije uspjela

  - **Data\_BootStrapperStateFailure\_FailingState** – dio datoteke bootstrapper koji nije uspio

  - **Data\_BootStrapperStateFailure\_OExceptionType** – vrsta iznimke zbog koje radnja nije uspjela

  - **Data\_ConfigurationHost –** glavno računalo s kojeg potječe datoteka configuration.xml

  - **Data\_ConfigurationId –** ID koji primimo iz datoteke configuration.xml

  - **Data\_ConfigurationHost –** izvor datoteka configuration.xml

  - **Data\_Culture** – kultura u kojoj se pokreće ovaj exe, npr. hr-hr

  - **Data\_HashedOLSToken** – raspršivanje sha-256 tokena koji nam OLS servis pošalje

  - **Data\_MigrateArchRequest –** označava migriramo li korisnika s 32-bitne verzije na 64-bitnu ili obrnuto

  - **Data\_MigrateArchRequestValid –** označava smatramo li zahtjev za migraciju valjanim

  - **Data\_Platform** – 64-bitna ili 32-bitna instalacija

  - **Data\_PlatformMigratedFrom –** početna platforma, npr. 32-bitna

  - **Data\_PlatformMigratedTo –** završna platforma, npr. 64-bitna

  - **Data\_PrereqFailure\_Type –** neispunjen preduvjet na koji smo naišli

  - **Data\_ProductReleaseId –** proizvod koji instaliramo, npr. Microsoft 365 Apps za velike tvrtke

### <a name="officeclicktorunrepomanlogger"></a>Office.ClickToRun.RepomanLogger

Izvještava o statusu za novi kanal ažuriranja „klikom do cilja“ („Repoman“) i ako uspješno preuzima i primjenjuje ažuriranja za Office.

Prikupljaju se sljedeća polja:

  - **ApplySucceeded –** Vrijednost true ako je kanal uspješno primijenio ažuriranje sustava Office, vrijednost false ako nije.
  
  - **DownloadSucceeded –** Vrijednost true ako je kanal uspješno preuzeo ažuriranje sustava Office, vrijednost false ako nije.

  - **ErrorCode –** Kôd posljednje pogreške koja se dogodila u kanalu „klikom do cilja“ Repoman.

  - **ErrorDetails –**  Dodatni detalji posljednje pogreške koja se dogodila u kanalu „klikom do cilja“ Repoman.
 
  - **ErrorMessage –** Poruka posljednje pogreške koja se dogodila u kanalu „klikom do cilja“ Repoman.

  - **OpenStreamSessionSucceeded –** Vrijednost true ako kanal uspješno stvara sesiju za strujanje ažuriranja sustava Office, vrijednost false ako ne stvara.

  - **RepomanErrorMessage –** Poruka o pogrešci primljena od sustava  repoman.dll.
 

### <a name="officeclicktorunscenarioinstalltaskconfigure"></a>Office.ClickToRun.Scenario.InstallTaskConfigure

Podaci o instalaciji i inventaru sustava Office prikupljeni kada instalacijski program sustava Office postavlja novopreuzete datoteke. Koristi se za mjerenje uspjeha/pogrešaka instalacije sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške 

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala koji koristi Windows SQM 

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioinstalltaskconfigurelight"></a>Office.ClickToRun.Scenario.InstallTaskConfigurelight

Podaci o instalaciji i inventaru sustava Office prikupljeni kada instalacijski program sustava Office odlučuje koje je datoteke potrebno preuzeti. Koristi se za mjerenje uspjeha/pogrešaka instalacije sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške 

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM 

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioinstalltaskfinalintegrate"></a>Office.ClickToRun.Scenario.InstallTaskFinalintegrate

Podaci o instalaciji i inventaru sustava Office prikupljeni kada instalacijski program sustava Office instalira licence i postavke registra. Koristi se za mjerenje uspjeha/pogrešaka instalacije sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM 

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioinstalltaskfonts"></a>Office.ClickToRun.Scenario.InstallTaskFonts

Podaci o instalaciji i inventaru sustava Office prikupljeni kada instalacijski program sustava Office instalira fontove. Koristi se za mjerenje uspjeha/pogrešaka instalacije sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške 

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM 

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioinstalltaskinitupdates"></a>Office.ClickToRun.Scenario.InstallTaskInitupdates

Podaci o instalaciji i inventaru sustava Office prikupljeni kada instalacijski program sustava Office stvara postavke potrebne da bi ažuriranja pravilno funkcionirala. Koristi se za mjerenje uspjeha/pogrešaka instalacije sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške 

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM 

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioinstalltaskintegrateinstall"></a>Office.ClickToRun.Scenario.InstallTaskIntegrateinstall

Podaci o instalaciji i inventaru sustava Office prikupljeni kada instalacijski program sustava Office stvara unose u registar za aplikacije sustava Office. Koristi se za mjerenje uspjeha/neuspjeha instalacije sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške 

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioinstalltasklastrun"></a>Office.ClickToRun.Scenario.InstallTaskLastrun

Podaci o instalaciji i inventaru sustava Office prikupljeni kada instalacijski program sustava Office završava instalaciju, prikvačuje prečace i stvara završne postavke registra. Koristi se za mjerenje uspjeha/pogrešaka instalacije sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške 

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioinstalltaskmigrate"></a>Office.ClickToRun.Scenario.InstallTaskMigrate

Podaci o instalaciji i inventaru sustava Office prikupljeni kada instalacijski program sustava Office migrira postavke iz starijih verzija sustava Office. Koristi se za mjerenje uspjeha/pogrešaka instalacije sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioinstalltaskpublishrsod"></a>Office.ClickToRun.Scenario.InstallTaskPublishrsod

Podaci o instalaciji i inventaru sustava Office prikupljeni kada instalacijski program sustava Office objavljuje virtualni registar za virtualizacijski sloj AppV. Koristi se za mjerenje uspjeha/pogrešaka instalacije sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioinstalltaskremoveinstallation"></a>Office.ClickToRun.Scenario.InstallTaskRemoveinstallation

Podaci o instalaciji i inventaru sustava Office prikupljeni kada instalacijski program sustava Office uklanja dijelove sustava Office s uređaja. Koristi se za mjerenje uspjeha/pogrešaka instalacije sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške 

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioinstalltaskstream"></a>Office.ClickToRun.Scenario.InstallTaskStream

Podaci o instalaciji i inventaru sustava Office prikupljeni kada instalacijski program sustava Office preuzima nove datoteke za Office. Koristi se za mjerenje uspjeha/pogrešaka instalacije sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške 

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM 

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioinstalltaskuninstallcentennial"></a>Office.ClickToRun.Scenario.InstallTaskUninstallcentennial

Podaci o instalaciji i inventaru sustava Office prikupljeni kada instalacijski program sustava Office deinstalira stariju verziju sustava Office koje je instalirana iz trgovine Microsoft Store. Koristi se za mjerenje uspjeha/pogrešaka instalacije sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške 

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenariorepairtaskfinalintegrate"></a>Office.ClickToRun.Scenario.RepairTaskFinalintegrate

Podaci o instalaciji i inventaru sustava Office prikupljeni kada klijent za popravak sustava Office ponovno objavi .msi datoteke i proširenja sustava Office. Koristi se za mjerenje uspjeha/pogrešaka popravka sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške 

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM 

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenariorepairtaskfullrepair"></a>Office.ClickToRun.Scenario.RepairTaskFullrepair

Podaci o instalaciji i inventaru sustava Office prikupljeni kada klijent za popravak sustava Office preuzme najnoviju verziju klijenta tehnologije "klikom do cilja" radi pripreme računala za deinstalaciju i ponovnu instalaciju. Koristi se za mjerenje uspjeha/pogrešaka popravka sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške 

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM 

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenariorepairtaskintegraterepair"></a>Office.ClickToRun.Scenario.RepairTaskIntegraterepair

Podaci o instalaciji i inventaru sustava Office prikupljeni kada klijent za popravak sustava Office pokuša popraviti unose u registru za koje je poznato da su problematični. Koristi se za mjerenje uspjeha/pogrešaka popravka sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške 

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM 

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenariorepairtaskremoveinstallation"></a>Office.ClickToRun.Scenario.RepairTaskRemoveinstallation

Podaci o instalaciji i inventaru sustava Office prikupljeni kada klijent za popravak sustava Office ukloni Office s uređaja radi pripreme za ponovnu instalaciju prilikom popravljanja. Koristi se za mjerenje uspjeha/pogrešaka popravka sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške 

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM 

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioupdatetaskintegrateupdate"></a>Office.ClickToRun.Scenario.UpdateTaskIntegrateupdate 

Podaci o instalaciji i inventaru sustava Office prikupljeni kada klijent tehnologije "klikom do cilja" ažurira licence ako je potrebno. Koristi se za mjerenje uspjeha/pogrešaka ažuriranja sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške 

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM 

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioupdatetaskpublishrsod"></a>Office.ClickToRun.Scenario.UpdateTaskPublishrsod

Podaci o instalaciji i inventaru sustava Office prikupljeni kada klijent tehnologije "klikom do cilja" ažurira postavke registra za nove binarne datoteke. Koristi se za mjerenje uspjeha/pogrešaka ažuriranja sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške 

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM 

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioupdatetaskupdateapply"></a>Office.ClickToRun.Scenario.UpdateTaskUpdateapply

Podaci o instalaciji i inventaru sustava Office prikupljeni kada klijent tehnologije "klikom do cilja" isključi pokrenute aplikacije ako je potrebno te instalira nove datoteke koje su preuzete. Koristi se za mjerenje uspjeha/pogrešaka ažuriranja sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_AvailableVersion to –** verzija sustava Office koja je dostupna za ažuriranje

  - **Data\_CompletedWithoutActionInfo –** razlog zbog kojeg scenarij nije dovršen, npr. aplikacije su bile otvorene

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_CorruptionChecksOnly –-** označava radi li se samo o traženju oštećenja bez ažuriranja

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_HardlinkingException –** iznimka na koju smo naišli pokušavajući stvoriti fiksne veze

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_PackageOperationSuccessful –** vrijednost je „true” ako je zadatak na paketu sustava Office uspješno dovršen

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

  - **Data\_WorkstationLockState –** vrijednost je true ako smatramo da je računalo zaključano

### <a name="officeclicktorunscenarioupdatetaskupdateclientdownload"></a>Office.ClickToRun.Scenario.UpdateTaskUpdateclientdownload

Podaci o instalaciji i inventaru sustava Office prikupljeni kada klijent tehnologije "klikom do cilja" preuzme noviju verziju samog sebe. Koristi se za mjerenje uspjeha/pogrešaka ažuriranja sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške 

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioupdatetaskupdatedetection"></a>Office.ClickToRun.Scenario.UpdateTaskUpdatedetection

Podaci o instalaciji i inventaru sustava Office prikupljeni kada klijent tehnologije "klikom do cilja" provjeri postoji li novo ažuriranje. Koristi se za mjerenje uspjeha/pogrešaka ažuriranja sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_AvailableVersion to –** verzija sustava Office na koju je moguće ažurirati sustav

  - **Data\_ComAction –** cijeli broj koji predstavlja naredbenu radnju koju izvodimo

  - **Data\_CompletedWithoutActionInfo –** razlog zbog kojeg scenarij nije dovršen, npr. aplikacije su bile otvorene

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_PackageUpdateAvailable –** vrijednost je „true” ako nam je dostupna nova verzija sustava Office

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM 

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioupdatetaskupdatedownload"></a>Office.ClickToRun.Scenario.UpdateTaskUpdatedownload

Podaci o instalaciji i inventaru sustava Office prikupljeni kada klijent tehnologije "klikom do cilja" preuzima novo ažuriranje. Koristi se za mjerenje uspjeha/pogrešaka ažuriranja sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_AvailableVersion to –** verzija sustava Office na koju je moguće ažurirati sustav

  - **Data\_CompletedWithoutActionInfo –** razlog zbog kojeg scenarij nije dovršen, npr. aplikacije su bile otvorene

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_CorruptionChecksOnly –** označava radi li se samo o traženju oštećenja bez ažuriranja

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_FoundCorruptFiles –** vrijednost je „true” ako smo pronašli oštećene datoteke

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_PackageOperationSuccessful –** vrijednost true ako je zadatak na paketu sustava Office uspješno dovršen

  - **Data\_PipelineExitCode –** izlazna šifra koju je vratio kanal za datoteke

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM 

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioupdatetaskupdatefinalize"></a>Office.ClickToRun.Scenario.UpdateTaskUpdatefinalize

Podaci o instalaciji i inventaru sustava Office prikupljeni kada klijent tehnologije "klikom do cilja" čisti nakon ažuriranja i vraća prethodno otvorene aplikacije. Koristi se za mjerenje uspjeha ili pogrešaka ažuriranja sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvodi koje dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške 

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –** proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID –** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto na kojem se nalazi izvor, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala kojim se koristi Windows SQM 

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje zadatka, primjerice pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktoruntransport"></a>Office.ClickToRun.Transport

Prijavljuje o postupcima preuzimanja datoteka da bi se utvrdio uspjeh postupka, vrsta izvršenog preuzimanja i dijagnostičke informacije.


- **BytesFromGroupPeers –**    bajtovi kolega iz grupe, samo za preuzimanja pomoću optimizacije isporuke

- **BytesFromHttp –**     bajtovi s http rukovatelja, samo za preuzimanja pomoću optimizacije isporuke

- **ByteFromInternetPeers –**     bajtovi kolega s interneta, samo za preuzimanja pomoću optimizacije isporuke 

- **BytesFromLanPeers –**    bajtovi Lan kolega, samo za preuzimanja pomoću optimizacije isporuke 

- **CancelledJobs -**    Broj otkazanih zahtjeva u sesiji

- **Connected –**    jeste li povezani s izvorom

- **ErrorCode –**    kôd posljednje pogreške

- **ErrorDetails -**     Pojedinosti posljednje pogreške

- **ErrorMessage -**    Poruka posljednje pogreške 

- **ErrorSource –**    izvor posljednje pogreške, npr. Povezivanje, Učitavanje datoteke ili Raspon učitavanja

- **FailedJob –**    broj neuspjelih zahtjeva u sesiji

- **FileSize -**    Veličina resursa

- **SourcePathNoFilePath -**    Izvještava se samo o izvorišnom putu resursa samo http izvora, put lokalne datoteke ili UNC put je filtriran

- **SucceededJobs –**    broj uspješnih zahtjeva u sesiji

- **TotalJobs -**     ukupan broj zahtjeva u sesiji

- **TotalRequestedBytes –**     ukupno traženih bajtova u sesiji

- **TotalTransferTime –**    ukupno vrijeme prijenosa u sesiji

- **TransferredBytes –**     ukupno prenesenih bajtova u sesiji

- **TransportType –**    vrsta prijenosa, npr. (u memoriji optimizaciji isporuke, putem HTTP protokola, putem pozadinskog pametnog servisa za transfer)



### <a name="officeclicktoruntransportexperimentaltransportpipelinecreatetransport"></a>Office.ClickToRun.Transport.ExperimentalTransport.PipelineCreateTransport

Podaci o instalaciji i inventaru sustava Office prikupljeni kada klijent tehnologije "klikom do cilja" otvara kanal za prijenos putem kojeg će preuzimati datoteke sustava Office. Koristi se za utvrđivanje stanja raznih prijenosnih tehnologija prijenosa (npr. HTTP, BITS, DO) koje su ključne za pravilno preuzimanje sustava Office radi instalacije i ažuriranja.

Prikupljaju se sljedeća polja:

  - **Data\_IsForeGroundStreaming** – označava prenosimo li podatke strujanjem u prvom planu ili u pozadini

  - **Data\_IsInstallMode** – ako instaliramo i preuzimamo datoteke, vrijednost je 1, a ako ne, vrijednost je 0

  - **Data\_SourceProtocol –** označava preuzimamo li iz mreže podataka sadržaja (CDN-a), s računala na koje instaliramo, iz lokalne mreže ili iz resursa u lokalnoj područnoj mreži.

  - **Data\_Status** – označava uspjeh ili neuspjeh 

### <a name="officeclicktorunupdatestatus"></a>Office.ClickToRun.UpdateStatus

Podaci o instalaciji i inventaru sustava Office prikupljeni kada klijent tehnologije "klikom do cilja" završava status ažuriranja

Prikupljaju se sljedeća polja:

  - **Data\_build** – trenutno instalirana verzija sustava Office

  - **Data\_channel** – kanal u kojem se korisnik nalazi

  - **Data\_errorCode** – cijeli broj koji određuje vrstu pogreške do koje je došlo ako pogreška postoji

  - **Data\_errorMessage** – niz koji sadrži opis pogreške do koje je došlo ako pogreška postoji

  - **Data\_status** – kratak status događaja tijekom ažuriranja, npr. uspješno ili preuzeto

  - **Data\_targetBuild -** – verzija sustava Office na koju pokušavamo ažurirati


### <a name="officeclicktorununiversalbootstrapperapplication"></a>Office.ClickToRun.UniversalBootstrapper.Application

Prijavljuje rezultat sveobuhvatnih pokušaja instalacije

 - **ErrorCode –**    vrijednost cijelog broja povezana je s neobrađenom iznimkom

 - **ErrorDetails –**    Niz koji opisuje mjesto na kojem se desila neobrađena iznimka (funkcija, datoteka, broj retka, dodatni parametri koje je postavio bacač)

 - **ErrorMessage –**    Niz definiran na mjestu izbacivanja neobrađene iznimke, opisujući prirodu neuspjeha

 - **ErrorType –**    niz koji opisuje kategoriju neobrađene iznimke

 - **ExitCode –**    cjelobrojna vrijednost povezana s rezultatom pokretanja programa za automatsko pokretanje, ukazuje na uspjeh ili određenu vrstu neuspjeha

### <a name="officeclicktorununiversalbootstrappercalculateparameters"></a>Office.ClickToRun.UniversalBootstrapper.CalculateParameters

Izvješćuje o radnji koja je razlog unosa prikupljenog pomoću CollectParameters

- **BitField –** cjelobrojna vrijednost argumenta BitField, koji nam  govori je li zatražena eksplicitna instalacija / kanal za nadogradnju. Na primjer, beta kanal, trenutačni kanal (pretpregled), trenutačni kanal, mjesečni kanal za velike tvrtke, polugodišnji kanal za velike tvrtke (pretpregled) ili polugodišnji kanal za velike tvrtke.

- **ID kanala –** cijeli broj koji predstavlja vrijednost rednog broja odabranog kanala za ažuriranje/instaliranje. Na primjer, beta kanal, trenutačni kanal (pretpregled), trenutačni kanal, mjesečni kanal za velike tvrtke, polugodišnji kanal za velike tvrtke (pretpregled), polugodišnji kanal za velike tvrtke, ili nevažeći.

- **CMDMode –**    neslužbeni niz koji odgovara ukupnoj zamjeni načina otkriven je u cmd argumentima koji su proslijeđeni u exe.

- **C2RClientUICulture –**    kultura klijenta C2R koju treba instalirati

- **ErrorCode –**    vrijednost cijelog broja povezana je s neobrađenom iznimkom

- **ErrorDetails –**    Niz koji opisuje mjesto na kojem se desila neobrađena iznimka (funkcija, datoteka, broj retka, dodatni parametri koje je postavio bacač)

- **ErrorMessage –**    Niz definiran na mjestu izbacivanja neobrađene iznimke, opisujući prirodu neuspjeha

- **ErrorType –**    niz koji opisuje kategoriju neobrađene iznimke

- **ExcludedApps –**    Niz koji navodi pojedinačna imena aplikacija za Office koje su zatražene da se izuzmu iz instaliranih Office paketa

- **InstalledCabVersion –**    verzija „16.0.xxxxx.yyyyy” Office C2R klijenta već je instalirana

- **InstalledProductVersion –**    verzija „16.0.xxxxx.yyyyy” Office C2R proizvoda već je instalirana

- **IsC2RServiceRunning –**    Booleova zastavica koja označava je li moderna usluga lokalnog računala C2R klijenta pokrenuta i radi na uređaju

- **IsElevatedFlagSet –**    Booleova zastavica koja označava je li automatsko pokretanje već pokušalo steći povećanje ovlasti administratora

- **IsFireFlyInstalled –**    Booleova zastavica koja pokazuje je li Office 2013 RTM C2R klijent trenutačno instaliran

- **IsFireflyServiceRunning –**    Booleova zastavica koja označava je li servis lokalnog računala RTM C2R klijenta iz 2013. godine pokrenut i radi na uređaju

- **IsOfficeInstalled –**    Booleova zastavica koja označava je li moderni Office klijent već instaliran

- **OfficeCultures –**    serijalizirani popis Office kultura koje treba instalirati

- **OfficeSourceType –**    Neslužbeni niz povezan s identifikatorom vrijednosti instalacijskog izvora (CDN, HTTP, UNC, CMBITS, DVD, LOCAL)

- **Origin –**    vrijednost niza koja govori koji od podržanih izvora (Portoriko [PR], Singapur [SG], Dublin [DB]) treba upotrijebiti za početno instalacijsko strujanje

- **PlatformFromLink –**    Niz koji pokazuje traženi x86 | x64 | zadani bit sustava Office zatražen od C2R servisa postavljanja

- **PlatformOfExistingInstallation –**    niz koji pokazuje je li x86 ili X64 Office već instaliran na uređaju

- **PlatformToInstall –**    niz koji pokazuje konačnu odluku o tome treba li instalirati x86 ili X64 Office. Mogućnosti su: automatsko pokretanje, konfiguriranje, korisnik, preuzimanje, pomoć, program za pakiranje

- **PRID –**    Vrijednost niza koja predstavlja traženi ID izdanja proizvoda u scenariju za instalaciju kod korisnika (primjerice, "O365ProPlusRetail")

- **PridsToMigrateFromCentennial –**    niz proizvoda sustava Office za migraciju iz instalacija trgovine u značajku „klikom do cilja”

- **ProductsToAdd –**    serijalizirani niz koji upućuje C2R klijenta na kombinacije proizvoda/kulture koje bi trebao instalirati

- **ProductsToMigrateFromO15C2R-** Niz proizvoda i kultura sustava Office za migraciju iz instalacije sustava Office 2013 značajkom "klikom do cilja"

- **ProductsToRemove –**    Serijalizirani niz koji upućuje C2R klijenta na kombinacije proizvoda/kulture koje bi trebao deinstalirati

- **SharedComputerLicensing –**    Booleov izraz koji ukazuje na to je li IT administrator zatražio postavljanje da bi se omogućila značajka „SharedComputerLicensing”

- **ShouldActivate –**    Booleov izraz koji ukazuje na to je li IT administrator zatražio automatski pokušaj aktiviranja licenciranja u datoteci configuration.xml

- **ShouldUninstallCentennial -** Booleova zastavica koja upućuje na to je li proizvode iz trgovine potrebno deinstalirati

- **VersionToInstall –**    Vrijednost niza verzije sustava Office "16.0.xxxxx.yyyyy" koja se instalira
 

### <a name="officeclicktorununiversalbootstrappercollectembeddedsignature"></a>Office.ClickToRun.UniversalBootstrapper.CollectEmbeddedSignature

Izvještava o radnji koja čita označeni unos iz ugrađenog potpisa exe datoteke.  Ovo je nedokazani koncept koji prethodna iteracija izvršne datoteke setup.exe nije implementirala i na što se oslanjamo u prenošenju korisnikovih izbora proizvoda/jezika/broja bitova s web-stranice na proces unutar izvršne datoteke setup.exe.
 
- **ErrorCode –**    cijeli broj povezan s neobrađenom iznimkom

- **ErrorDetails –**    Niz koji opisuje mjesto na kojem se desila neobrađena iznimka (funkcija, datoteka, broj retka, dodatni parametri koje je postavio bacač)

- **ErrorMessage –**    Niz definiran na mjestu izbacivanja neobrađene iznimke, opisujući prirodu neuspjeha

- **ErrorType –**    niz koji opisuje kategoriju neobrađene iznimke

### <a name="officeclicktorununiversalbootstrappercollectparameters"></a>Office.ClickToRun.UniversalBootstrapper.CollectParameters

Izvješćuje o parametrima koji se koriste za instalaciju sustava Office

- **BitField –** cjelobrojna vrijednost argumenta BitField, koji nam  govori je li zatražena eksplicitna instalacija / kanal za nadogradnju. Na primjer, beta kanal, trenutačni kanal (pretpregled), trenutačni kanal, mjesečni kanal za velike tvrtke, polugodišnji kanal za velike tvrtke (pretpregled) ili polugodišnji kanal za velike tvrtke.

- **ID kanala –** cijeli broj koji predstavlja vrijednost rednog broja odabranog kanala za ažuriranje/instaliranje. Na primjer, beta kanal, trenutačni kanal (pretpregled), trenutačni kanal, mjesečni kanal za velike tvrtke, polugodišnji kanal za velike tvrtke (pretpregled), polugodišnji kanal za velike tvrtke, ili nevažeći.

- **CMDMode –**    neslužbeni niz koji odgovara ukupnoj zamjeni načina otkriven je u cmd argumentima koji su proslijeđeni u exe. Mogućnosti su: automatsko pokretanje, konfiguriranje, korisnik, preuzimanje, pomoć, program za pakiranje

- **C2RClientUICulture –**    kultura klijenta C2R koju treba instalirati

- **ErrorCode –**    vrijednost cijelog broja povezana je s neobrađenom iznimkom

- **ErrorDetails –**    Niz koji opisuje mjesto na kojem se desila neobrađena iznimka (funkcija, datoteka, broj retka, dodatni parametri koje je postavio bacač)

- **ErrorMessage –**    Niz definiran na mjestu izbacivanja neobrađene iznimke, opisujući prirodu neuspjeha

- **ErrorType –**    niz koji opisuje kategoriju neobrađene iznimke

- **ExcludedApps –**    Niz koji navodi pojedinačna imena aplikacija za Office koje su zatražene da se izuzmu iz instaliranih Office paketa

- **InstalledCabVersion –**    verzija „16.0.xxxxx.yyyyy” Office C2R klijenta već je instalirana

- **InstalledProductVersion –**    verzija „16.0.xxxxx.yyyyy” Office C2R proizvoda već je instalirana

- **IsC2RServiceRunning –**    Booleova zastavica koja označava je li moderna usluga lokalnog računala C2R klijenta pokrenuta i radi na uređaju

- **IsElevatedFlagSet –**    Booleova zastavica koja označava je li automatsko pokretanje već pokušalo steći povećanje ovlasti administratora

- **IsFireFlyInstalled –**    Booleova zastavica koja pokazuje je li Office 2013 RTM C2R klijent trenutačno instaliran

- **IsFireflyServiceRunning –**    Booleova zastavica koja označava je li servis lokalnog računala RTM C2R klijenta iz 2013. godine pokrenut i radi na uređaju

- **IsOfficeInstalled –**    Booleova zastavica koja označava je li moderni Office klijent već instaliran

- **OfficeCultures –**    serijalizirani popis Office kultura koje treba instalirati

- **OfficeSourceType –**    Neslužbeni niz povezan s identifikatorom vrijednosti instalacijskog izvora (CDN, HTTP, UNC, CMBITS, DVD, LOCAL)

- **Origin –**    vrijednost niza koja govori koji od podržanih izvora (Portoriko [PR], Singapur [SG], Dublin [DB]) treba upotrijebiti za početno instalacijsko strujanje

- **PlatformFromLink –**    Niz koji pokazuje traženi x86 | x64 | zadani bit sustava Office zatražen od C2R servisa postavljanja

- **PlatformOfExistingInstallation –**    niz koji pokazuje je li x86 ili X64 Office već instaliran na uređaju

- **PlatformToInstall –**    niz koji pokazuje konačnu odluku o tome treba li instalirati x86 ili X64 Office

- **PRID –**    Vrijednost niza koja predstavlja traženi ID izdanja proizvoda u scenariju za instalaciju kod korisnika (primjerice, "O365ProPlusRetail")

- **PridsToMigrateFromCentennial-** Niz proizvoda sustava Office za migraciju iz instalacija trgovine u značajku "klikom do cilja"

- **ProductsToAdd –**    serijalizirani niz koji upućuje C2R klijenta na kombinacije proizvoda/kulture koje bi trebao instalirati

- **ProductsToMigrateFromO15C2R-** Niz proizvoda i kultura sustava Office za migraciju iz instalacije sustava Office 2013 značajkom "klikom do cilja"

- **ProductsToRemove –**    Serijalizirani niz koji upućuje C2R klijenta na kombinacije proizvoda/kulture koje bi trebao deinstalirati

- **SharedComputerLicensing –**    Booleov izraz koji ukazuje na to je li IT administrator zatražio postavljanje da bi se omogućila značajka „SharedComputerLicensing”

- **ShouldActivate –**    Booleov izraz koji ukazuje na to je li IT administrator zatražio automatski pokušaj aktiviranja licenciranja u datoteci configuration.xml

- **ShouldUninstallCentennial -** Booleova zastavica koja upućuje na to je li proizvode iz trgovine potrebno deinstalirati

- **VersionToInstall –**    vrijednost niza verzije sustava Office „16.0.xxxxx.yyyyy” koja se instalira

### <a name="officeclicktorununiversalbootstrapperexecute"></a>Office.ClickToRun.UniversalBootstrapper.Execute

Izvješćuje o poduzetim radnjama koje su utjecale na stroj, što je utvrđeno obrazloženim podacima iz opcije "CalculateParameters"

- **AvailableClientVersionText –**    vrijednost niza C2R klijenta verzije „16.0.xxxxx.yyyyy” pronađena u verziji Deskriptor XML, koji se koristi kako bi se utvrdilo treba li ažurirati trenutno instalirani C2R klijent

- **CleanFireflyAction –**    „true” ako se planira pokretanje zadatka CleanFireFlyAction tijekom ove instalacije

- **CleanO15Action –**    „true” ako se planira pokretanje zadatka CleanO15Action tijekom ove instalacije

- **CMDMode –**    neslužbeni niz koji odgovara ukupnoj zamjeni načina otkriven je u cmd argumentima koji su proslijeđeni u exe. Mogućnosti su: automatsko pokretanje, konfiguriranje, korisnik, preuzimanje, pomoć, program za pakiranje

- **DeliveryMechanism –**   „FFNRoot” guid izdvojen iz XML-a deskriptora verzije (koji nosi oznaku RDX-a), koji nam govori iz koje publike/kanala potječe izvor međuverzije

- **DownloadC2RClientAction –**    „true” ako se planira pokretanje zadatka DownloadC2RClientAction tijekom ove instalacije

- **ErrorCode –**    vrijednost cijelog broja povezana je s neobrađenom iznimkom

- **ErrorDetails –**    Niz koji opisuje mjesto na kojem se desila neobrađena iznimka (funkcija, datoteka, broj retka, dodatni parametri koje je postavio bacač)

- **ErrorMessage –**    Niz definiran na mjestu izbacivanja neobrađene iznimke, opisujući prirodu neuspjeha

- **ErrorType –**    niz koji opisuje kategoriju neobrađene iznimke

- **ExitCode –**   cjelobrojna vrijednost povezana s rezultatom pokretanja izvršne faze programa za automatsko pokretanje, ukazuje na uspjeh ili određenu vrstu neuspjeha

- **LaunchAction –**    "true" ako se planira pokretanje zadatka LaunchAction tijekom ove instalacije

- **LaunchUpdateAction –**    „true” ako se planira pokretanje zadatka LaunchUpdateAction tijekom ove instalacije

- **PreReqResult –**    cjelobrojna vrijednost za identifikaciju rezultata kada se izvode provjere preduvjeta (prolaz/pad/ponovno pokretanje)

- **UnexpectedAction –**    "true" ako se planira pokretanje zadatka UnexpectedAction (slučaj pogreške) tijekom ove instalacije

- **VersionToInstall –**    Vrijednost niza za verziju sustava Office "16.0.xxxxx.yyyyy" koja se instalira

### <a name="officeserviceabilitymanagerinventoryaddonheartbeat"></a>Office.ServiceabilityManager.InventoryAddon.Heartbeat

*[Ovaj je događaj uklonjen iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

Taj se događaj koristi za pribavljanje standardnih meta-podataka pri svakom pokretanju dodatka Inventar, koji je dio Upravitelja za Office servisiranje i koristi se za informacije o Office inventaru na onim strojevima koje je IT administrator uključio. Meta-podatak od posebnog zanimanja u ovom slučaju je ID sesije, a koristi se za povezivanje s drugim podacima pohranjenima unutar usluge na oblaku po klijentu.

Ovaj događaj nema dodatnih polja jer su relevantni samo meta-podaci.

### <a name="officeserviceabilitymanagerinventoryaddonresults"></a>Office.ServiceabilityManager.InventoryAddon.Results

Taj se događaj bilježi kada se poziv na web-servis u sklopu dodatka "klikom do cilja" za inventar upravitelja za servis dovrši, neovisno o tome uspijeva li ili ne uspijeva. To je u suštini posljednja operacija unutar dodatka za praćenje ukupnog stanja rada.

Prikupljaju se sljedeća polja:

- **ActionDetail** – dodatne pojedinosti u slučaju nastupanja kvara.
   - Ako zahtjev HTTP-a uspije, ActionDetail bit će 0.
   - Ako Polje rezultata nije U redu (tj. nije 0), što znači da zahtjev nije poslan, u ovom će se polju zabilježiti kod interne pogreške koji je jednak Polju rezultata.
   - Ako je Polje rezultata U redu (tj. 0), što znači da je kôd odgovora HTTP-a >= 300, u njemu će se zabilježiti kôd odgovora HTTP-a (npr. 404).

- **Rezultat** – brojčana oznaka pogreške koju vraćaju API-jevi poziva web-servisa sustava Office. – npr. 3 znači da postoji problem s inicijalizacijom zaglavlja HTTP-a.

- **Type** – dodatne informacije o vrsti. U slučaju Zaliha, ove informacije određuju vrstu tereta koji se šalje – npr. pune ili samo delta promjene. 

-  **WebCallSource** – vrijednost za numeriranje (koja se određuje kao cijeli broj) koja označava dodatak upravitelja servisa koji je bio izvor poziva:
   - Zalihe: 0
   - Konfiguriranje zaliha: 1
   - Pravilnik o zalihama: 2
   - Stanje mreže zaliha: 3
   - Upravitelj servisa: 4
   - Mogućnost upravljanja: 5

### <a name="officeserviceabilitymanagerwebservicefailure"></a>Office.ServiceabilityManager.WebserviceFailure

Ova se naredba bilježi svaki put kad ne uspije poziv na web-servis unutar jednog od dodataka upravitelja servisa sustava Office. Pogreške mogu nastati zbog unutarnjih pogrešaka ili nemogućnosti povezivanja s web-servisom.

Prikupljaju se sljedeća polja:

- **Add-on** - Programski dodatak upravitelja servisa "klikom do cilja" iz kojeg je pokrenut poziv na web-servis. To može imati vrijednosti kao što su zalihe, upravljanje itd., kodirane kao numerička vrijednost.

- **Correlation ID** – nasumično generirani GUID specifičan za trenutnu instancu koji je poslan web-servisu kako bi povezao pozive između klijenta i poslužitelja.

- **ErrorInfo** - brojčana oznaka pogreške koju vraćaju API-jevi poziva web-servisa sustava Office.

- **ErrorMessage** – poruka koja omogućuje daljnji uvid u pogrešku. Svaka se vrsta greške mapira na niz ugrađen u kôd, a neke se vrste grešaka mapiraju na potencijalno više nizova ovisno o posebnoj vrsti greške.

- **Function** – funkcija u kodu iz koje je došlo do trenutnog poziva.

- **Status** – kôd HTTP-a kojeg vraća poziv web-servisu, npr. 404, 500, itd.


## <a name="enhanced-configuration-service-ecs-events"></a>Događaji servisa za eksperimentiranje i konfiguraciju (ECS-a)

### <a name="officeexperimentationfeaturequerybatched"></a>Office.Experimentation.FeatureQueryBatched

Prikuplja podatke o ulazima značajkama / ulazima za promjene kojima izvršeni kod šalje upit.

Prikupljaju se sljedeća polja:

  - **Count** – broj ulaza značajki kojima je u ovom skupnom događaju poslan upit

  - **Features** – informacije o ulazima kojima je poslan upit.

  - **Sequence** – redoslijed kojim su slani upiti ulazima značajki

### <a name="officeexperimentationflightnumberline"></a>Office.Experimentation.FlightNumberLine

Prikuplja popis konfiguracija koje je klijent primio iz ECS-a

Prikupljaju se sljedeća polja:

  - **ECSConfigs** – popis konfiguracija ECS-a razdvojenih zarezom

  - **LockType** – vrsta blokade FlightManager.

  - **TasFlightingVersion** – broj verzije

  - **TimeToLock** – vrijeme između inicijacije libleta i blokade FlightManager

  - **UnmergedConfigs** – popis konfiguracija koje nisu spojene

### <a name="officeexperimentationtriggeranalysis"></a>Office. Experimentation. TriggerAnalysis

Ovaj događaj pomaže analizi opsega upotrebe proizvoda i parametara performansi (poput rušenja, prekida i sl.) podskupini korisnika ili uređaja koji ispunjavaju uvjete za upotrebu ove značajke i na taj način pomažu u osiguravanju ispravnog rada proizvoda.

Prikupljaju se sljedeća polja:

  - **FeatureGate –** Identificira skup značajki za koje je primjenjiva analiza okidača.

### <a name="onenoteflightdefault"></a>OneNote.FlightDefault
 
Taj se događaj bilježi kada OneNote zatraži od poslužitelja ECS vrijednosti letenja.  To se koristi da bi se omogućile eksperimentalne značajke korisnicima koji su se uključili u primanje ovakvih letova.
 
Prikupljaju se sljedeća polja:
 
- **ConfigParam** – konfiguracija za koju se pristupa vrijednosti

## <a name="licensing-events"></a>Događaji licenciranja

### <a name="officeandroiddocsuipaywallcontrolautoredeempendingpurchaseresult"></a>Office.Android.DocsUI.PaywallControl.AutoRedeemPendingPurchaseResult

Kritična inženjerska telemetrija za bilježenje rezultata automatskog pokušaja iskorištavanja kupnji na čekanju. Telemetrija proizvoda koja se upotrebljava za usklađivanje podataka o transakcijama kupnje s Microsoftovim sustavom trgovine radi omogućivanja povezanih pogodnosti pretplate.

Prikupljaju se sljedeća polja:

- **EventDate** – vremenska oznaka pojavljivanja događaja 

- **Result** – Int koji označava rezultat nabrajanja operacije. 

- **SessionID** – GUID za povezivanje događaja po sesiji

### <a name="officeandroiddocsuipaywallcontrolpaywalluishown"></a>Office.Android.DocsUI.PaywallControl.PaywallUIShown

Kritična telemetrija upotrebe kada se korisniku prikazuje kontrola Paywall. Upotrebljava se za razumijevanje iskustva kupnje aplikacije za korisnika i optimizaciju istog za buduće verzije.

Prikupljaju se sljedeća polja:

- **EventDate** – vremenska oznaka pojavljivanja događaja 

- **IsModeFRE** – Booleov izraz za označavanje vrste iskustva, dijaloškog okvira prodaje dodatnih opcija ili SKU birača

- **SessionID** – GUID za povezivanje događaja po sesiji

### <a name="officeandroiddocsuipaywallcontrolpurchasebuttonclicked"></a>Office.Android.DocsUI.PaywallControl.PurchaseButtonClicked

Kritična telemetrija upotrebe kako bismo znali kada korisnik klikne na gumb Kupnja. Upotrebljava se za zaključivanje o načinu korištenja i mjernim podacima konverzije za korisnike koji pokušaju kupiti pretplatu u aplikaciji.

Prikupljaju se sljedeća polja:

- **EventDate** – vremenska oznaka pojavljivanja događaja

- **Isdefaultsk** – Booleov izraz koji ukazuje na to pokušava li korisnik kupiti SKU koji se prvi pojavio/zadani

- **ProductID** – niz koji prepoznaje korisnika pretplate koji pokušava kupiti kako je konfiguriran u trgovini

- **SessionID** – GUID za povezivanje događaja po sesiji

### <a name="officeandroiddocsuipaywallcontrolpurchaseresult"></a>Office.Android.DocsUI.PaywallControl.PurchaseResult

Kritična inženjerska telemetrija da biste evidentirali rezultat pokušaja kupnje koji korisnik aktivira ručno. Telemetrija proizvoda koja se upotrebljava za usklađivanje podataka o transakcijama kupnje s Microsoftovim sustavom trgovine radi omogućivanja povezanih pogodnosti pretplate.

Prikupljaju se sljedeća polja:

- **EventDate** – vremenska oznaka pojavljivanja događaja 

- **IsModeFre** – Booleov izraz koji ukazuje na to je li kupnja stvorena pomoću zaslona s početnim sučeljem prodaje dodatnih opcija ili SKU birača

- **Result** – Int koji označava rezultat nabrajanja operacije.

- **SessionID** – GUID za povezivanje događaja po sesiji

### <a name="officeandroiddocsuipaywallcontrolpurchasetokenredemptionresponse"></a>Office.Android.DocsUI.PaywallControl.PurchaseTokenRedemptionResponse

*[Taj se događaj prije zvao Office.Android.DocsUI.Views.PurchaseTokenRedemptionResponse.]*

Ovi se telemetrijski podaci o proizvodu prikupljaju radi praćenja i bilježenja internog statusa transakcija i informacija namijenjenih usklađivanju s ciljem poboljšanja pouzdanosti i performansi. Microsoft te podatke koristi za analizu i poboljšanje pouzdanosti i performansi obrade internih transakcija te mehanizme usklađivanja.

Prikupljaju se sljedeća polja:

- **MicrosoftPurchaseOrderId** – Microsoftov ID narudžbe koji servis Retail Federation Service (RFS) šalje za potrebe praćenja.

- **ResponseCode** – kôd HTTP odgovora (cijeli broj)

- **Kôd statusa StatusCode** – statusni kôd RFS odgovora (konačan skup cijelih brojeva koji definira RFS radi identifikacije)


### <a name="officeandroiddocsuipaywallcontrolseeallfeaturesanalytics"></a>Office.Android.DocsUI.PaywallControl.SeeAllFeaturesAnalytics

Prikupljamo ovu telemetriju upotrebe kako bismo vidjeli koliko vremena korisnik provodi na zaslonu "Pogledajte više pogodnosti".  Podaci se upotrebljavaju za razumijevanje upotrebe značajke „Pogledajte više pogodnosti" te daljnju optimizaciju iskustva u budućim verzijama.

Prikupljaju se sljedeća polja:

- **Duration** – Dugi cijeli broj koji označava vrijeme koje je korisnik proveo na zaslonu "Vidi sve značajke" u milisekundama

- **EventDate** – vremenska oznaka pojavljivanja događaja 

- **MostExplored** – cijeli broj koji označava indeks stavke s najviše promjena na popisu aplikacija Microsoft 365 i njihovih značajki

- **Sessioid** – globalno jedinstveni identifikator (GUID) za povezivanje događaja po sesiji

### <a name="officeandroiddocsuipaywallcontrolskuchooseranalytics"></a>Office.Android.DocsUI.PaywallControl.SkuChooserAnalytics

Telemetrija upotrebe da biste vidjeli koliko vremena korisnik troši na zaslonu SKU birača. Telemetrija upotrebe da biste vidjeli koliko vremena korisnik troši na zaslonu SKU birača.

Prikupljaju se sljedeća polja:

- **Duration** – Dugi cijeli broj koji označava vrijeme koje je korisnik proveo na zaslonu SKU birača u milisekundama

- **EventDate** – vremenska oznaka pojavljivanja događaja

- **SessionID** – GUID za povezivanje događaja po sesiji


### <a name="officeandroiddocsuiviewsdimeerror"></a>Office.Android.DocsUI.Views.DimeError

Taj se događaj prikuplja za aplikaciju Office za Android (objavljenu na platformi Huawei i u trgovinama u Kini). Taj događaj označava da pokušaj kupnje pretplate na Microsoft 365 putem platforme Dime (webURL učitan u web-prikazu u klijentu) nije uspio. Snimaju se samo scenariji pogrešaka. Ti su podaci o događajima samo podaci o pogreškama, a koriste se za osiguravanje dobrog stanja tijeka kupnje putem platforme Dime u klijentu.

Prikupljaju se sljedeća polja:

- **CorrelationID** – ID koji na jedinstven način identificira sesiju kupnje putem platforme Dime.

- **ErrorReason** – označava razlog pogreške do koje je došlo.
  - 0 – nepoznata pogreška
  - 1 – internet nije dostupan
  - 2 – nije uspjela provjera valjanosti univerzalno jedinstvenog identifikatora (UUID)
  - 3 – univerzalno jedinstven identifikator (UUID) null je ili prazan
  - 4 – pogreška umetanja u JavaScriptu pri kojoj aplikacija Office za Android ne može proslijediti authToken platformi Dime
  - 5 – temeljni WebURL učitan na klijentu nije valjan


### <a name="officedimesdkhealth"></a>Office.Dime.Sdk.Health

Taj događaj bilježi podatke koji omogućuju praćenje stanja Dime komponenti. Primjerice, da biste mogli koristiti tijek kupnje u aplikaciji kada se korisnik odluči za kupnju pretplate na Microsoft 365 iz aplikacije Office za Android ili na uređajima sa sustavom Windows.

Prikupljaju se sljedeća polja:

- **Data_ActivityErrorDescription** – opis pogreške u okviru aktivnosti

- **Data_ActivityErrorDescription** – poruka o pogrešci u okviru aktivnosti 

- **Data_CampaignId** – ID kampanje za pripisivanje atributa

- **Data_ContentId** – temelji se na ID-u doživljaja i mapira na ID tijeka i ID sadržaja

- **Data_CorrelationVector** – korelacijski vektor za povezivanje novčića sustava Dime s partnerima koji koriste korelacijski vektor

- **Data_CustomerImpacted** – koristi se za otklanjanje poteškoća ako je učitavanje tijeka imalo utjecaja na korisnika

- **Data_DimeActivityDuration** – vrijeme trajanja 

- **Data_DimeActivityMetadata** – metapodaci o aktivnostima

- **Data_DimeActivityName** – naziv aktivnosti za nadzor stanja sustava

- **Data_DimeActivityResult** – rezultat aktivnosti, uspjeh / pogreška / očekivana pogreška

- **Data_DimeVersion** – verzija međuverzije

- **Data_DurationLevel** – težina: 0/1/2

- **Data_EcsConfigIds** – ID-ovi za eksperimente

- **Data_EcsCountry** – otkrivena država

- **Data_EcsETag** – informacije o testnim verzijama

- **Data_Environment** – produkcijsko/pretprodukcijsko okruženje sustava Dime

- **Data_ExperienceId** – doživljaj koji treba učitati 

- **Data_FlowId** – temelji se na ID-u doživljaja i mapira na ID tijeka i ID sadržaja

- **Data_Language** – kultura

- **Data_Market** – otkriveno tržište

- **Data_OTelJS_Version** – verzija telemetrije za Office

- **Data_PageSessionId** – ID sesije za stranicu

- **Data_PartnerId** – pozivateljska aplikacija

- **Data_QosLevel** – težina: 0/1/2

- **Data_SDX_AssetId** – ID resursa za sadržaj koji pruža Service Delivered Experience (SDX) za Win32

- **Data_SDX_BrowserToken** – token preglednika za Win32

- **Data_SDX_HostJsVersion** – verzija JavaScript biblioteke za Win32

- **Data_SDX_Id** – ID servisa Service Delivered Experience za Win32

- **ID Data_SDX_InstanceId** – ID instance SDX-a za Win32

- **Data_SDX_MarketplaceType** – vrsta SDX Marketplacea za Win32

- **Data_SDX_OfficeJsVersion** – verzija Office JS-a za Win32

- **Data_PageSessionId** – ID sesije za SDX za Win32

- **Data_SDX_Version** – verzija SDX-a za Win32

- **Data_TimestampUTC** – vremenska oznaka događaja

- **Data_TsgId** – ID vodiča za otklanjanje poteškoća za svaku aktivnost

- **Data_UserAgent** – oznake zaglavlja

### <a name="officeiospaywallskuchooserbuybuttontap"></a>Office.iOS.Paywall.SKUChooser.BuyButtonTap

Kritična telemetrija upotrebe prikuplja se kako bi ukazala na to kada korisnik dodiruje gumb Kupi.  Podaci se upotrebljavaju za zaključivanje o načinu korištenja i mjernim podacima konverzije za korisnike koji pokušaju kupiti pretplatu u aplikaciji.

Prikupljaju se sljedeća polja:

- **entryPoint** – niz – gumb/tijek s kojeg je prikazan Paywall. Kao što je "Premium Upgrade Button" ili „First run flow“

- **isdefaultSKU** – Booleova vrijednost – ako korisnik kupuje proizvod, preporučili smo mu, prikazujući ga prema zadanim postavkama.

- **productId** – niz – ID proizvoda trgovine App-store za koji je dodirnut gumb Kupi

- **toggleCount** – Int – koliko je puta korisnik prelazio s jednog prikaza proizvoda na drugi prije nego što je dodirnuo gumb Kupi u trenutačnoj sesiji Paywall-a.


### <a name="officelicensingaccepteulaforcurrentlicense"></a>Office.Licensing.AcceptEulaForCurrentLicense 

To se prikuplja kad korisnik dobije licencu i prihvati EULA-u za trenutnu licencu

Koristi se radi otkrivanja je li korisnik u dobrom stanju, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **ACID** – GUID identifikator koji predstavlja proizvod sustava Office za koji korisnik ima licencu

  - **DwEulaId** – numerički identifikator vrste EULA-e koju je korisnik prihvatio

### <a name="officelicensingactivation"></a>Office.Licensing.Activation 

Nakon postavljanja licence na računalu pokušavamo licencu aktivirati pozivanjem servisa AVS. Ovo prijavljuje rezultat poziva radi aktivacije

Ključno je za otkrivanje koliko bi korisnika moglo imati problema s aktivacijom. Za otkrivanje eventualnih regresija imamo otkrivanje anomalija. To je izuzetno važno jer ovisimo o vanjskom servisu AVS, pa nam ovaj signal pokazuje je li stanje naših vanjskih partnera dobro. Koristi se i u dijagnostičke svrhe te za utvrđivanje stanja sustava ako korisnik priajvi problem s uređajem

Prikupljaju se sljedeća polja:

  - **Acid** – GUID identifikator koji predstavlja proizvod sustava Office za koji korisnik ima licencu

  - **ReferralData** – identifikator OEM-a koji je instalirao Office na računalo

### <a name="officelicensingactivationwizard"></a>Office.Licensing.ActivationWizard 

Ako zbog nekog razloga ne možemo automatski aktivirati licencu, korisniku prikazujemo čarobnjak za aktivaciju. Ovo prijavljuje da je korisniku prikazan čarobnjak. Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Događaj ne prikuplja nijedno polje.

### <a name="officelicensingdialogswebviewdialogclose"></a>Office.Licensing.Dialogs.WebViewDialog.Close
 
Taj se događaj koristi kao signal koji nam govori da su korisnik ili aplikacija zatvorili okruženje za kupnju iz aplikacije. Ti se podaci koriste za nadziranje i upozoravanje o stanju tijeka kupnje iz aplikacije kako bi se osiguralo da on funkcionira na očekivan način.  
 
Prikupljaju se sljedeća polja:
 
- **Data_ClosedDialog** – zastavica koja označava da je korisnik zatvorio dijaloški okvir

### <a name="officelicensingdialogswebviewdialoghandleerrornotification"></a>Office.Licensing.Dialogs.WebViewDialog.HandleErrorNotification
 
Taj se događaj koristi kao signal koji nam govori da se okruženje za korištenje u aplikaciji pokušalo učitati, ali je došlo do pogreške koja je dovela do toga da se dijaloški okvir ne prikaže. Ti se podaci koriste za nadziranje i upozoravanje o stanju tijeka kupnje iz aplikacije kako bi se osiguralo da on funkcionira na očekivan način.  
 
Prikupljaju se sljedeća polja:
  
- **Data_MoeErrorCode** – šifra pogreške koja se prikazuje u okruženju dijaloškog okvira za web

### <a name="officelicensingdialogswebviewdialogpreload"></a>Office.Licensing.Dialogs.WebViewDialog.Preload
 
Taj se događaj koristi kao signal koji nam govori da se okruženje za kupnju iz aplikacije učitava u pozadini. Ti se podaci koriste za nadziranje i upozoravanje o stanju tijeka kupnje iz aplikacije kako bi se osiguralo da on funkcionira na očekivan način.  
 
Prikupljaju se sljedeća polja:

 - Nijedno

### <a name="officelicensingdialogswebviewdialogshow"></a>Office.Licensing.Dialogs.WebViewDialog.Show
 
Taj se događaj koristi kao signal koji nam govori da se okruženje za kupnju iz aplikacije prikazuje korisniku. Ti se podaci koriste za nadziranje i upozoravanje o stanju tijeka kupnje iz aplikacije.  

Prikupljaju se sljedeća polja:

 - Nijedno

### <a name="officelicensingdialogswebviewdialogtimeout"></a>Office.Licensing.Dialogs.WebViewDialog.Timeout

Taj se događaj koristi kao signal koji nam govori da se okruženje za kupnju u aplikaciji pokušalo učitati, ali je vrijeme čekanja isteklo. Ti se podaci koriste za nadziranje i upozoravanje o stanju tijeka kupnje iz aplikacije kako bi se osiguralo da on funkcionira na očekivan način. 

Prikupljaju se sljedeća polja:

 - Nijedno


### <a name="officelicensingenforcesigninqualified"></a>Office.Licensing.EnforceSignInQualified 

Taj nam signal daje do znanja je li eksperiment koji smo pokrenuli radi prisilne prijave korisnika u sklopu licenciranja uspio. Ključan je za otkrivanje uspješnosti ili pogreške eksperimenta kojim se korisnika prisiljava na prijavu, što je obavezan korak za moderni stog za licenciranje. Ako se korisnik ne prijavi, neće moći koristiti aplikaciju.

Prikupljaju se sljedeća polja:

  - **Qualified** – određuje je li korisnik kvalificiran za prisilnu prijavu

### <a name="officelicensingexpirationdialogshown"></a>Office.Licensing.ExpirationDialogShown

Ovo se prikuplja prilikom prikazivanja dijaloškog okvira korisniku koji kaže da mu je licenca istekla. Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **LicNotificationState** – identifikator koji nas obavještava o tome kakve se obavijesti prikazuju korisniku

### <a name="officelicensingfullvalidation"></a>Office.Licensing.FullValidation 

To se prikupljaju u svakoj sesiji koja prijavljuje stanje licenciranja računala te prijavljuje pogreške koje se korisniku prikazuju i zbog kojih ne može koristiti aplikaciju. Događaj označava je li korisnikovo računalo u dobrom stanju. Za taj smo događaj postavili otkrivanje anomalija da bismo prepoznali uzrokuje li regresija ili mehanizam aktivacije negativno ponašanje korisnika. Ključno je i za dijagnosticiranje korisničkih problema te za praćenje stanja sustava.

Prikupljaju se sljedeća polja:

  - **Acid** – GUID identifikator koji predstavlja proizvod sustava Office za koji korisnik ima licencu  
  
  - **Atributi Activationatribute**-vrsta mehanizma aktivacije koji korisnik upotrebljava.

  - **IsSessionLicensing** – određuje je li trenutno pokrenut način rada za aktivaciju zajedničkog računala 

  - **LicenseCategory** – kategorija licence za Office koju korisnik koristi  

  - **Licenses** – popis naziva svih licenci za Office koje postoje na računalu  

  - **LicenseStatuses** – status svih licenci za Office koje postoje na računalu  

### <a name="officelicensinggetentitlement"></a>Office.Licensing.GetEntitlement 

To prikupljamo kad korisnik postavlja uređaj te pozivamo servis za licenciranje da otkrije ima li prijavljeni korisnik prava na Office. Prijavljuje rezultat poziva Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

- **EntitlementCount** – Broj prava koja korisnik ima


### <a name="officelicensingheartbeat"></a>Office.Licensing.Heartbeat 

Za svaku sesiju provjeravamo je li prošlo 72 sata od zadnje obnove licence te pokušavamo produljiti vrijeme do isteka trenutne licence. Događaj prijavljuje uspješnost ili pogrešku poziva koji upućujemo radi provjere možemo li produljiti vrijeme do isteka licence i zadržati funkcionalnost korisnikove instalacije sustava Office. Ključan je za dijagnosticiranje problema povezanih s pretplatom i problema sa servisom za korisnika te za otkrivanje regresija već aktiviranih korisnika pretplate.

Prikupljaju se sljedeća polja:

  - **Mode** – prikaz stoga licenciranja sustava Office koji se koristi na ovom računalu

### <a name="officelicensinginclientpinredemptioncallpinredemptionapi"></a>Office.Licensing.InClientPinRedemption.CallPinRedemptionAPI

Ta telemetrija prati rezultate otkupnog poziva servisa PIN sustava Office.

Prikupljaju se sljedeća polja:

- **ClientTransactionId**- jedinstveni identifikator za poziv servisa.

- **ErrorCategory** – svaka vrsta pogreške može se nalaziti u više općenitim kategorijama, npr. „Retryable”.

- **ErrorType** – razlog neuspjeha, kao što je „AlreadyRedeemedByOther”.

- **InAFOFlow** – Booleova oznaka koja upućuje na to da je u tijeku AFO iskupljenje.

- **StatusCode** – rezultat servisnog poziva od jedne riječi, poput „Created”.

- **StatusMessage** – pojedinosti o kôdu statusa, kao što je „Uspješno dodijeljeno”.

- **UsingNulApi**- Booleova vrijednost koja upućuje na to da li koristimo novi stog licenci za licenciranje.

### <a name="officelicensinginrfm"></a>Office.Licensing.InRFM 

Ako uređaj prijeđe u način rada smanjene funkcionalnosti, šaljemo signal koji označava da računalo nije u dobrom stanju. Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **ACID** – GUID identifikator koji predstavlja proizvod sustava Office za koji korisnik ima licencu

  - **DaysRemaining** – broj dana do isteka trenutne licence za Office

  - **Mode** – prikaz stoga licenciranja sustava Office koji se koristi na računalu kao identifikatora

  - **ProductName** – naziv proizvoda koji korisnik trenutno upotrebljava

  - **Reason** – šifra pogreške koja označava razlog trenutnog statusa licence

### <a name="officelicensinginstallkey"></a>Office.Licensing.InstallKey

To se prikuplja kad pokušamo instalirati ključ na uređaj radi licenciranja računala. Prijavljuje je li instalacija uspjela, a ako nije, prijavljuje šifru pogreške. Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **Prid** – naziv grupe proizvoda za koju se instalira ključ

  - **SkuId** – GUID identifikator koji predstavlja proizvod sustava Office za koji se ključ instalirana  

### <a name="officelicensinginvokelicensewizard"></a>Office.Licensing.InvokeLicenseWizard

U slučaju da uočimo probleme s tijekom rada aktivacije, pokrećemo čarobnjaka za licencu i šaljemo ovaj signal da ukazuje na isto. Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **Acid** – GUID identifikator koji predstavlja proizvod sustava Office za koji korisnik ima licencu

  - **LicenseStatus** – status licence za Office koju korisnik koristi

  - **MachineKey** – alfanumerički identifikator licencnog ključa koji je izdan korisniku

### <a name="officelicensinglicensingbar"></a>Office.Licensing.LicensingBar

Ako bi uređaj mogao imati problema s licenciranjem te korisniku prikažemo traku s obavijesti, šaljemo ovaj signal, koji ujedno prijavljuje vrstu trake s obavijesti koja je prikazana korisniku. Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **SuppressNotification** – označava jesmo li izostavili prikaz trake s obavijesti o licenciranju

  - **Title** – naslov trake s obavijesti o licenciranju koja je prikazana korisniku

  - **Type** – vrsta trake s obavijesti o licenciranju koja je prikazana korisniku

### <a name="officelicensinglicexitofficeprocess"></a>Office.Licensing.LicExitOfficeProcess 

Ako zatvorimo/srušimo Office zbog problema s licenciranjem, šaljemo ovaj signal da bismo to naznačili.  Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **ExitCode** – interni kod koji je uzrokovao zatvaranje aplikacije

### <a name="officelicensingloadidentityticket"></a>Office.Licensing.LoadIdentityTicket

Aplikacija tijekom pokušaja licenciranja uređaja pokušava učitati korisnikov identitet da bi provjerila ima li korisnik prava na Office. Događaj prijavljuje uspjeh ili neuspjeh istog zajedno s eventualnom šifrom pogreške. Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **FederationProvider** – niz koji određuje davatelja usluga vanjskog pristupa trenutno prijavljenog korisnika

  - **IdentityProvider** – niz koji određuje davatelja usluga identiteta trenutno prijavljenog korisnika

### <a name="officelicensinglvuxeulaexplicitcrash"></a>Office.Licensing.LVUX.EULAExplicitCrash 

To se prikupljaju ako smo korisniku prikazali EULA-u, a korisnik je nije prihvatio, zbog čega rušimo/zatvaramo aplikaciju. Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **Acid** – GUID identifikator koji predstavlja proizvod sustava Office za koji korisnik ima licencu

  - **OptInShown** – označava je li dijaloški okvir za uključivanje koji se prikazuje prilikom prvog pokretanja aplikacije već prikazan

### <a name="officelicensingnextuserlicensingeligible"></a>Office.Licensing.NextUserLicensingEligible 

Taj signal označava je li korisnik kvalificiran za premještanje na novi stog za licenciranje. To je ključno za kvantifikaciju učinka na postojeće korisnike tijekom uvođenja novog stoga za licenciranje i da korisnici ne bi izgubili funkcionalnost.

Događaj ne prikuplja nijedno polje.

### <a name="officelicensingnulfetcherfetchmodelfromols"></a>Office.Licensing.Nul.Fetcher.FetchModelFromOls

Kada je uređaj na modernom stogu za licenciranje, licencnu datoteku pokušavamo dohvatiti izravno sa servisa. Događaj prijavljuje uspjeh ili pogrešku zajedno s eventualnom šifrom pogreške poziva servisu. Ključan je za otkrivanje je li korisnik u dobrom stanju na modernom stogu za licenciranje, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom.

Prikupljaju se sljedeća polja:

  - **MetadataValidationResult** – rezultat provjere valjanosti metapodataka o licenci da bi se potvrdilo da nije neovlašteno mijenjana

  - **SignatureValidationResult** – rezultat provjere valjanosti potpisa licence da bi se potvrdilo da nije neovlašteno mijenjana

### <a name="officelicensingnulvalidationfullvalidation"></a>Office.Licensing.Nul.Validation.FullValidation 

To se prikuplja tijekom svake sesije uređaja koji koristi moderni stog za licenciranje. Prijavljuje stanje licenciranja računala te prijavljuje pogreške koje se korisniku prikazuju i zbog kojih ne može koristiti aplikaciju. Događaj označava je li korisnikovo računalo u dobrom stanju na modernom stogu za licenciranje. Za taj smo događaj postavili otkrivanje anomalija da bismo prepoznali uzrokuje li regresija negativno ponašanje korisnika. Ključno je i za dijagnosticiranje korisničkih problema te za praćenje stanja sustava.

Prikupljaju se sljedeća polja:

  - **Acid** – GUID identifikator koji predstavlja proizvod sustava Office za koji korisnik ima licencu 

  - **AllAcids** – popis svih GUID-ova proizvoda za koje je korisnik trenutno licenciran 

  - **Category** – kategorija licence za Office koju korisnik koristi  

  - **DaysRemaining** – broj dana do isteka trenutne licence za Office  

  - **LicenseId** – alfanumerički identifikator licence koja je izdana korisniku 

  - **LicenseType** – vrsta licence za Office koju korisnik koristi  

### <a name="officelicensingofficeclientlicensingdolicensevalidation"></a>Office.Licensing.OfficeClientLicensing.DoLicenseValidation 

To su metapodaci o licenciranju koji se prilikom svakog pokretanja prikupljaju s uređaja, a prijavljuju ACID licence, status licence, vrstu i druga svojstva licence koja su ključna za prepoznavanje skupa značajki koje su korisniku dostupne. Ključni su za prepoznavanje skupa značajki koje su korisniku dostupni te utvrđivanje ne nedostaje li korisniku koja funkcija. Koriste se i za izračune dnevnog broja aktivnih korisnika / mjesečnog broja aktivnih korisnika te za razna druga izvješća različitih timova u sustavu Office (marketing/DIG/licenciranje) jer sadrže informaciju o vrsti proizvoda koju korisnik upotrebljava, o tome je li u pitanju pretplatnički proizvod te nedostaju li mu ključne funkcije.

Prikupljaju se sljedeća polja:

  - **FullValidationMode** – način rada koji označava da provodimo potpunu provjeru valjanosti potvrde licence 

  - **IsRFM** – označava je li korisnik u načinu rada smanjene funkcionalnosti 

  - **IsSCA** – označava je li pokrenut način rada za aktivaciju na zajedničkom računalu 

  - **IsSubscription** – označava koristi li korisnik pretplatničku licencu 

  - **IsvNext** – označava koristimo li moderni stog za licenciranje 

  - **LicenseCategory** – kategorija licence za Office koju korisnik koristi  

  - **LicenseStatus** – status licence za Office koju korisnik koristi 

  - **LicenseType** – vrsta licence za Office koju korisnik koristi  

  - **LicensingACID** – GUID identifikator koji predstavlja proizvod sustava Office za koji korisnik ima licencu  

  - **OlsLicenseId** – alfanumerički identifikator licence koja je izdana korisniku 

  - **SkuIdIsNull** – označava jesmo li naišli na pogrešku zbog koje ne znamo koji proizvod korisnik upotrebljava 

  - **SlapiIsNull** – označava jesmo li naišli na problem prilikom popunjavanja jednog od objekata licenciranja 

### <a name="officelicensingonlinerepair"></a>Office.Licensing.OnlineRepair 

Ako zbog nekog razloga ne možemo aktivirati korisnika i moramo mu prikazati dijaloški okvir u kojem se od njega traži da se povežu s internetom i pokušaju s koracima za popravak, aktivira se ovaj događaj. Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Događaj ne prikuplja nijedno polje.

### <a name="officelicensingoobetrybuychoice"></a>Office.Licensing.OOBE.TryBuyChoice

Korisnici sa unaprijed instaliranim sustavom Office na novim strojevima koji nemaju pravo na sustav Office prikazani su u dijaloškom okviru pomoću kojeg mogu isprobati, kupiti ili unijeti ključ proizvoda da bi se licencirali. Tim se događajem bilježi akcija korisnika u dijaloškom okviru. Taj se događaj koristi da bi se pratila korisnička akcija poduzeta u dijaloškom okviru koji se prikazuje korisnicima koji nemaju pravo na sustav Office u kojem je Office unaprijed instaliran na računalu i pomaže pri određivanju je li korisnik licenciran ili nelicenciran po dizajnu.

Prikupljaju se sljedeća polja:

- **Buy** – govori je li korisnik kliknuo na gumb Buy ili nije

- **ForceAutoActivate** – kaže bi li se trebala pokrenuti aktivacija u aplikaciji ili ne

- **GoBackToSignIn** - kaže je li se korisnik htio ponovno prijaviti (možda s drugim računom)

- **IsPin** – upućuje na to je li korisnik unio PIN

- **ProductKey** - govori je li korisnik pokušao unijeti ključ proizvoda

- **Try** – govori je li korisnik kliknuo na gumb Try ili nije

- **UserDismissed** – to upućuje na to je li korisnik odbacio dijaloški okvir, a time i način rada u načinu mirovanja ili načinu smanjene funkcionalnosti jer nije odabrao kupovinu sustava Office niti probnu verziju

### <a name="officelicensingpurchase"></a>Office.Licensing.Purchase 

*[Ovaj je događaj uklonjen iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

Imamo eksperiment u kojem se korisniku nudi mogućnost da isproba i postavi automatsko plaćanje sustava Office izravno iz aplikacije, a da ni u jednom trenutku ne mora izaći iz aplikacije. Ovo prijavljuje uspjeh ili pogrešku tog eksperimenta, te šifru pogreške. Ključno je u otkrivanju je li korisnik u dobrom stanju, te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom.

Prikupljaju se sljedeća polja:

  - **StorePurchaseStatus** – predstavlja šifru pogreške / šifru uspjeha poziva za kupnju obavljenog putem Windows trgovine

### <a name="officelicensingsearchforsessiontoken"></a>Office.Licensing.SearchForSessionToken

Ako je korisnik u načinu rada za aktivaciju na zajedničkom računalu, pokušavamo potražiti token sesije na računalu koji korisniku omogućuje upotrebu aplikacije. Događaj prijavljuje uspjeh ili neuspjeh scenarija zajedno s eventualnom šifrom pogreške. Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **LoadLicenseResult** – predstavlja šifru pogreške / šifru uspjeha učitavanja licenci za trenutnog korisnika

  - **OpportunisticTokenRenewalAttempted** – označava jesmo li oportunistički pokušali obnoviti token za korisnikovu sesiju

  - **SetAcidResult** – predstavlja šifru pogreške / šifru uspjeha postavljanja ACID-a na očekivanu vrijednost

### <a name="officelicensingshownewdeviceactivationdialog"></a>Office.Licensing.ShowNewDeviceActivationDialog

Prilikom prvog pokretanja neke aplikacije sustava Office pokušat ćemo prikazati dijaloški okvir za prijavu koji je unaprijed popunjen vjerodajnicama koje je korisnik upotrijebio za preuzimanje sustava Office. Korisnik se potom može prijaviti pomoću tih vjerodajnica, unijeti druge vjerodajnice ili odbaciti dijaloški okvir. Događaj prijavljuje radnju koju je korisnik poduzeo kad mu se prikazao dijaloški okvir. Ključan je za otkrivanje je li korisnik u dobrom stanju na modernom stogu za licenciranje, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **UserAction** – identifikator radnje koju je korisnik poduzeo kad mu se prikazao dijaloški okvir.

### <a name="officelicensingskutoskuconversion"></a>Office.Licensing.SkuToSkuConversion

Ako prilikom licenciranja korisnika moramo korisnikov SKU promijeniti iz jednog u drugi, šaljemo ovaj signal zajedno sa šifrom uspjeha ili pogreške. Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **DestinationSku** – naziv SKU-a u koji je potrebno pretvoriti trenutno instaliran proizvod

  - **PendingAcid** – ID proizvoda za koji je na čekanju pretvorbe SKU-a

  - **SourceSku** – naziv izvornog SKU-a instaliranog na računalu

  - **UninstallProduct** – označava hoće li se stari proizvod deinstalirati prilikom pretvorbe

### <a name="officelicensingtelemetryflowolsresults"></a>Office.Licensing.TelemetryFlow.OLSResults

Kada korisnik nema licencirani program, obavit ćemo nekoliko poziva servisa da bismo korisnika doveli u licencirano stanje i aktivirali proizvod sustava Office.  Taj se događaj aktivira na poziv servisa za licenciranje sustava Office da bismo provjerili ima li korisnik pravo na njih.  Taj će se događaj koristiti za praćenje zdravlja licence korisnika nakon pozivanja servisa za licenciranje sustava Office i zdravlja klijenta sustava Office nakon pokušaja aktivacije sustava Office.

Prikupljaju se sljedeća polja:

- **EntitlementPickerShown**- upućuje na to je li korisnik imao više prava, te je li korisnik morao ručno odabrati da bi se licencirao

- **GetAuthResult** – navodi različita stanja u kojima klijent može biti ako ima prazan ključ proizvoda iz servisa za licenciranje sustava Office ili ako ima pravo na neki drugi proizvod, a Office mora biti pretvoren u novi proizvod

- **GetEntitlementsCount** – Broj prava koja korisnik ima

- **GetEntitlementsSucceeded** – upućuje na to je li poziv API-ja za licenciranje sustava Office za dohvaćanje prava korisnika uspio ili nije

- **GetKeySucceeded** – upućuje na to je li poziv API-ja za licenciranje sustava Office za dohvaćanje ključa uspio ili nije

- **GetNextUserLicenseResult** – kaže može li moderni stog za licenciranje funkcionirati i je li korisnik dobio licencu ili nije

- **InstallKeyResult** – objašnjava različite razloge zašto je korisnik možda u lošem stanju, primjerice da aktivacija nije uspjela ili nije uspjelo instaliranje ključa

- **NotInitializedBeforeWhileAdding** – to je samo informativno i govori da je događaj dodan u mapu telemetrijskog upravitelja bez eksplicitnog registriranja za nju.

- **NotInitializedBeforeWhileSending** – to je samo informativno i govori da se događaj pokušao dodati u mapu telemetrijskog upravitelja bez eksplicitnog registriranja unaprijed za nju

- **SentOnDestruction** – to je samo informativno i govori da je događaj dodan u mapu telemetrijskog upravitelja bez eksplicitnog slanja

- **Tag** – koristi se za određivanje mjesta u kodu s kojeg je poslan događaj

- **VerifyEntitlementsResult** – navodi različita stanja u kojima bi korisnik mogao biti nakon provjere prava dohvaćenih iz servisa za licenciranje sustava Office

### <a name="officelicensingtelemetryflowsearchforbindingresult"></a>Office.Licensing.TelemetryFlow.SearchForBindingResult

OEM-ovi prodaju strojeve koji isporučuju sa sustavom Office (jednogodišnja ili neprekidna pretplata).  Ti se proizvodi sustava Office plaćaju kada kupac kupi uređaj. Strojevi koje se podešava pomoću određenog reg.ključa (OOBEMode: OEMTA) možda su povezani Office povezivanjem.  Prilikom dizanja sustava Office na takvim strojevima obavljamo servisne provjere da bismo saznali je li pronađena obveza sustava Office koja odgovara stroju.

Ta telemetrijska aktivnost prati točke uspjeha i neuspjeha u traženju povezivanja da bismo mogli osigurati da ih strojevi koji imaju obveze mogu uspješno dohvatiti i da su naši servisi zdravi.  Ta aktivnost ne prati strojeve bez obveza koji nisu povezani s njima kada provjerimo naše servise.

Prikupljaju se sljedeća polja:

- **DexShouldRetry** – signal da smo naišli na problem koji se može ponovo pokušati (nema internetskih ni poslužiteljskih kvarova)

- **GenuineTicketFailure** – govori HRESULT neuspjeha kad pokušavamo dobiti originalnu Windows karticu/ključ proizvoda (WPK).

- **PinValidationFailure** – govori zašto proces provjere valjanosti PIN-a nije uspio. Moguće pogreške:
    - GeoBlocked
    - InvalidFormat
    - InvalidPin
    - InvalidState
    - InvalidVersion
    - Nepoznato
    - Iskorišteno

- **PinValidationResult** – govori nam rezultat provjere valjanosti PIN-a kojeg nismo uspjeli provaliti.

- **Pkpn** - pkpn raspon kojem PIN pripada.

- **Success** - ukazuje na to da smo uspješno dohvatili valjanu Office obvezu (PIN) za stroj.

- **Tag** – govori nam da smo prestali tražiti obveze. Moguće oznake:
  - 0x03113809    Nema Interneta/usluge greška prilikom provjere valjanosti PIN-a
  - 0x0311380a    Neuspjela provjera valjanosti PIN-a, poslano s poljem PinValidationFailure
  - 0x0310410f    Uspjeh, poslano s poljem Uspjeh
  - 0x0311380d    Greške koje je moguće ponovno pokrenuti (problemi s Internetom, nepoznate greške)
  - 0x0311380e    Greške koje nije moguće ponovno pokrenuti (istekla obvezujuća ponuda)
  - 0x0311380f    Ostale greške (licenciranje nije moguće)
  - 0x03104111    Nije uspjelo provaljivanje PIN-a za Office, poslano s poljem PinValidationResult

- **WpkBindingFailure** – upućuje nas na kôd pogreške prilikom dobivanja PIN-a za Office vezanog uz WPK za računalo.

### <a name="officelicensingtelemetryflowshowafodialogs"></a>Office.Licensing.TelemetryFlow.ShowAFODialogs

Nakon uspješnog dobivanja valjanog PIN-a za Office vezanog uz uređaj koji je unaprijed u paketu sa sustavom Office, korisniku smo prikazali dijaloški okvir za prijavu ili okvir otkupa.  Kada se PIN otkupi, prikazat će se dijaloški okvir EULA.  U sklopu naše modernizacijske značajke AFO osvježili smo dva dijaloška okvira da bismo prenijeli dodatne informacije o proizvodu sustava Office koji se isporučuje uz uređaj.  Ta telemetrija prati smanjuje li naša značajka uspješno korisnikovo trenje u otkupljenju proizvoda praćenjem tokova i izlaznih točaka procesa otkupa (za što je dijaloški okvir odbijen).

Prikupljaju se sljedeća polja:

- **ActionActivate** – signal da je korisnik kliknuo gumb „Aktiviraj”.

- **ActionChangeAccount** – signal da je korisnik kliknuo hipervezu „Upotrijebi drugi račun”.

- **ActionCreateAccount** – signal da je korisnik kliknuo gumb „Stvori račun”.

- **ActionSignIn** – signal da je korisnik kliknuo gumb „Prijava”.

- **CurrentView** – vrsta dijaloškog okvira koji je korisnik zatvorio.

- **DialogEULA** – signal da smo prikazali dijaloški okvir „Prihvati EULA-u”. 

- **DialogRedemption** – signal da smo prikazali dijaloški okvir za iskorištavanje AFO-a.

- **DialogSignIn** – signal da smo prikazali dijaloški okvir za prijavu u AFO-a.

- **EmptyRedemptionDefaults** – signal da nismo uspjeli dohvatiti zadane informacije o iskorištavanju.
 
- **GetRedemptionInfo** – signal da dohvaćamo demografske podatke ili podatke o iskorištavanju PIN-a.

- **MalformedCountryCode** – signal da je kôd države koji je potreban za iskorištavanje PIN-a pogrešno oblikovan.

- **OExDetails** – pojedinosti pogreške koju ćemo vratiti kada je odbijen dijaloški okvir za prijavu identiteta.

- **OExType** – vrsta pogreške koju ćemo vratiti kada je odbijen dijaloški okvir za prijavu identiteta.

- **Tag** – govori nam u kojem trenutku korisnik izlazi iz procesa AFO otkupa. Moguće oznake:
    - 0x0311380b    Korisnik je odbacio dijaloški okvir za prijavu iz dijaloškog okvira za otkup
    - 0x0311380c    Nije uspjelo automatsko učitavanje prijave za prijavu identiteta korisnika iz dijaloškog okvira za otkup
    - 0x03113810    Nije uspjelo učitavanje demografskih informacija o računu (pozivni broj za državu, jezične, valutne i marketinške preferencije te probna ponuda)
    - 0x03113805    Korisnik je odbacio dijaloški okvir za prijavu identiteta iz dijaloškog okvira za prijavu
    - 0x03113806    Nije uspjelo automatsko učitavanje prijave identiteta korisnika iz dijaloškog okvira za prijavu
    - 0x03113807 Nije uspjelo automatsko učitavanje identiteta
    - 0x03113811 Korisnik je završio dijaloški okvir za prijavu/otkup
    - 0x03113812 Korisnik je završio dijaloški okvir Prihvati EULA
    - 0x03113808 Korisnik je prihvatio EULA
    - 0x03113811 Korisnik je zatvorio dijaloški okvir
    - 0x2370e3a0 Korisnik je zatvorio dijaloški okvir
    - 0x2370e3c1 Idite na web-mjesto za iskorištavanje PIN-a
    - 0x2370e3a1 Idite na web-mjesto za iskorištavanje PIN-a
    - 0x2370e3c0 Petlja dijaloških sekvenci koja je uzrokovana korisnikovim pomicanjem unatrag i unaprijed u dijaloškom toku
    - 0x2370e3a3 Korisnik je kliknuo vezu „Ne sada” kojom se preskače ponuda AFO-a za tu sesiju
    - 0x2370e3a2 Korisnik je kliknuo hipervezu „Nikad mi to ne prikazuj” kojom se onemogućuje ponuda AFO-a


- **UseInAppRedemption** – govori nam držimo li korisnike u aplikaciji za otkup ili ih šaljemo na web da bi iskoristili svoj dohvaćeni PIN (unaprijed popunjeni).

- **UseModernAFO** – govori nam koristimo li novo ili staro iskustvo za AFO.

### <a name="officelicensingtelemetryflowshowtrybuydialogforoobe"></a>Office.Licensing.TelemetryFlow.ShowTryBuyDialogForOOBE

Kada novi aparati imaju unaprijed instaliranu verziju sustava Office, a korisnik nema pravo, prikazat će se dijaloški okvir koji korisniku omogućuje da proba, kupi ili unese ključ proizvoda kako bi se licencirao i taj događaj prati je li prikazan dijaloški okvir. Taj će vam događaj pomoći da saznate je li korisniku prikazao dijaloški okvir za isprobavanje, kupnju ili unos ključa za proizvoda, a time ćete nam pomoći da utvrdimo je li korisnik imao mogućnost kupnje licenciranog sustava.

Prikupljaju se sljedeća polja: 

- **ActiveView** – daje ID dijaloškog okvira koji se prikazuje korisniku

- **CurrentOOBEMode**- govori koji je način rada za pred-instaliranje (način rada OOBE, npr. AFO, OEM itd.)

- **NotInitializedBeforeWhileAdding** – to je samo informativno i govori da je događaj dodan u mapu telemetrijskog upravitelja bez eksplicitnog registriranja za nju.

- **SentOnDestruction** – to je samo informativno i govori da je događaj dodan u mapu telemetrijskog upravitelja bez eksplicitnog slanja

- **ShowTryButton** – govori je li gumb Try prikazan korisniku u dijaloškom okviru ili nije

- **Tag** – koristi se za određivanje mjesta u kodu s kojeg je poslan događaj

### <a name="officelicensingtelemetryflowtrialflow"></a>Office.Licensing.TelemetryFlow.TrialFlow

Kada nelicencirani korisnik sustava Office koji je unaprijed instaliran na stroju proba doći do probne verzije, taj će se događaj aktivirati.  Koristi se da bi se prikazala putanja koju korisnik slijediti da bi dobio probnu verziju i ako je došlo do grešaka prilikom dobivanja probne verzije putem kupnje u aplikaciji.  Ovisno o korisnikovoj akciji i rezultatu kupnje u aplikaciji, korisnik može završiti kao da nije licenciran.

Prikupljaju se sljedeća polja:

- **HasConnectivity** – govori ima li korisnik internetsku vezu, a u slučaju da ona ne postoji, korisnik možda koristi licencu za poček za pet dana ili je možda u načinu rada s smanjenom funkcionalnošću

- **InAppTrialPurchase** – upućuje na to je li za pokretanje SDK za kupnju u trgovini omogućeno snimanje PI-a i kupnja iz probne aplikacije *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

- **IsRS1OrGreater** – upućuje na to je li verzija sustava veća od RS1 ili ne, jer se SDK za kupnju u trgovini može koristiti samo ako je verzija OS-a veća od RS1

- **NotInitializedBeforeWhileAdding** – to je samo informativno i govori da je događaj dodan u mapu telemetrijskog upravitelja bez eksplicitnog registriranja za nju

- **OEMSendToWebForTrial** – upućuje na to je li omogućen let za slanje korisnika na web radi iskorištavanja probne verzije

- **StoreErrorConditions** – upućuje na različite uvjete u kojima je SDK za kupnju u trgovini možda neuspio *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

- **StoreErrorHResult** – upućuje na kôd pogreške vraćen iz SDK za kupnju u trgovini *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

- **StorePurchaseStatusResult** – daje rezultat poziva SDK za kupnju u trgovini i je li korisnik obavio kupnju ili nije, što će pomoći odrediti hoće li korisnik imati licencu za korištenje sustava Office *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

- **Tag** – upotrebljava se za određivanje mjesta u kodu s kojeg je poslan događaj

- **UserSignedInExplicitly** – govori je li se korisnik potpisao eksplicitno jer ćemo u tomu slučaju ponovno usmjeriti korisnike na web-mjesto za probnu verziju *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

### <a name="officelicensingusegracekey"></a>Office.Licensing.UseGraceKey

Ako zbog nekog razloga ne možemo licencirati korisnika, instaliramo privremeni ključ i šaljemo signal koji to označava. Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **OpportunisticTokenRenewalAttempted** – označava jesmo li pokušali oportunistički obnoviti korisnika u načinu rada za licenciranje zajedničkog računala

  - **ReArmResult** – označava rezultat ponovne aktivacije instalacijskog ključa koji može produljiti vrijeme do isteka trenutne licence

### <a name="onenoteenrollmentresult"></a>OneNote.EnrollmentResult
 
Tim se događajem zapisuje status prilikom uključivanja u Intune.  Taj je scenarij specifičan za korištenje računa omogućenih za Intune.
 
Prikupljaju se sljedeća polja:
 
- **EnrollmentResult**- rezultat upisa u Intune

## <a name="microsoft-autoupdate-mau-events"></a>Događaji Microsoftova automatskog ažuriranja (MAU)

### <a name="additionalappinfoinvalidpreference"></a>additionalappinfo.invalidpreference

Tim se događajem izvješćuje nevažeća preferencija koja je postavljena za prikaz dodatnih informacija u pogledu završetka pružanja usluge za proizvod. Te podatke upotrebljavamo da bismo korisnike savjetovali da postavke točne preferencije kako bi vidjeli dodatne informacije.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije koji šalje događaj

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **Reason** – Pojedinosti o nevažećem unosu u preferencama

- **SessionId** – Identifikator sesije

### <a name="appdelegatelaunch"></a>appdelegate.launch

Taj događaj označava da je došlo do pokušaja pokretanja aplikacije. Evidentiramo rezultat (neuspjeh ili uspjeh). Koristimo ovaj događaj da identificiramo slučajeve u kojima se MAU ne uspije pokrenuti

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja
    
- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Skup statičnog teksta koji pokazuje stanje pokretanja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="appdelegateterminate"></a>appdelegate.terminate

Ovaj događaj znači da se dogodio skladni izlaz iz aplikacije. Koristimo ovaj događaj za razlikovanje skladnog izlaza iz aplikacije od neskladnog.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku
    
- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja
    
- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Statični tekst koji ukazuje na to da je Microsoftovo automatsko ažuriranje prekinuto.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="appinstallconnecttoxpc"></a>appinstall.connecttoxpc

Ovaj događaj označava da je došlo do pogreške prilikom povezivanja s MAU pomagačem (komponentom koja izvodi instalaciju aplikacije).  Ovaj događaj označava potencijalnu korupciju aplikacije MAU. Uređaj neće moći instalirati ažuriranja.

Prikupljaju se sljedeća polja:    

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži podatke o pogrešci problema s povezivanjem.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="appinstalllogscanned"></a>appinstall.logscanned

Taj se događaj upotrebljava da bi se utvrdilo je li datoteka zapisnika uspješno obrađena. Taj događaj upotrebljavamo da bismo utvrdili i riješili sve probleme koji nastaju tijekom instalacije aplikacije. 
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije koji šalje događaj

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Izvješća o pogreškama koje su pronađene tijekom instalacije aplikacije i/ili statusa dovršavanja skeniranja 

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="appregistryconfig"></a>appregistry.config

Ovaj događaj izvješćuje o svim pogreškama koje se javljaju tijekom učitavanja podataka o registru aplikacije. Ovim izvješćem savjetujemo IT administratore o ispravnom formatu postavljanja registracija klijentske aplikacije.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije koji šalje događaj

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži informacije o vrsti pogreške koja je pronađena u okviru registracije aplikacije.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="appregistryinfo"></a>appregistry.info

Ovaj događaj označava pokretanje aplikacije. Ovaj događaj koristimo za popis aplikacija za koje MAU može kontrolirati ažuriranja, broj dostupnih primjeraka kao i njihovu verziju te lokaciju instaliranja (zadanu ili drugu).

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – sadrži podatke o popisu identifikatora koje aplikacija koristi za registraciju na uslugu Microsoftova automatskog ažuriranja i broj instalacija registriranih za aplikaciju.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="appregistryremove"></a>appregistry.remove

Ovaj događaj označava da je došlo do pokušaja uklanjanja aplikacije s popisa aplikacija kojima upravlja MAU. Ovim događajem potvrđujemo da se putem MAU-a upravlja samo aplikacijama koje su izdane u MAU-u (ovdje se ne smiju pojavljivati AppStore aplikacije).

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Naziv i identifikator uklonjene aplikacije, bilo da se aplikacija i dalje nalazi na registriranom mjestu i je li aplikacija instalirana iz servisa AppStore.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="catalogerrorsignature"></a>catalog.errorsignature

Ovaj događaj znači da je došlo do neuspjeha tijekom izvođenja provjere autentičnosti koda na datoteci za ažuriranje elemenata osiguranja.  Svaka provjera autentičnosti neispravnih elemenata osiguranja treba se smatrati nevažećom.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži naziv datoteke kataloga s nevažećim potpisom. Različiti statični tekst opisuje različite uvjete pogreške.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="cloningtaskbegin"></a>cloningtask.begin

Ovaj događaj označava početak zadatka kloniranja prije ažuriranja aplikacije. Ovim događajem u kombinaciji s događajem cloningtask.status utvrđujemo količinu neuspjelih kloniranja kako bismo utvrdili je li značajku kloniranja potrebno ograničiti na različitim kanalima publike.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije koji šalje događaj

- **AppID** – Identifikator aplikacije.

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator za ažuriranje.


### <a name="cloningtaskhelpertoolconnection"></a>cloningtask.helpertoolconnection

Ovaj događaj bilježi probleme s instalacijom na klon (tj. ili se nećemo uspjeti povezati s pomagačem da primijenimo ažuriranje ili ćemo se povezati, ali pomagač ne može primijeniti ažuriranje) Ako ikada dobijemo zapis prijave, to znači da instalacija na klon nije uspjela i da će se morati izvršiti povratno ažuriranje na mjestu.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži ID za identificiranje pojedinačne aktivnosti ažuriranja i pogrešku proxy poslužitelja prijavljenu tijekom postupka kloniranja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="cloningtaskstatus"></a>cloningtask.status

Ovaj događaja označava status procesa kloniranja za aplikaciju koju je potrebno ažurirati. Ovim događajem utvrđujemo stopu uspjeha te vrste pronađenih pogrešaka koje uzrokuju neispravnosti. Ovim događajem utvrđujemo je li značajku kloniranja potrebno ograničiti na različitim kanalima publike.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator aplikacije.

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Error** – Niz sadrži informacije o pogrešci ako se pogreška pojavila tijekom zadatka kloniranja.

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **Success** – Niz zastupljenosti Booleove varijable.

- **UpdateID** – Identifikator za ažuriranje.

### <a name="cloningtaskstatusfinish"></a>cloningtask.status.finish

Ovaj događaj izvješćuje o dovršavanju zadatka „kloniranja”. Ovaj događaj predstavlja dio izvješća o lijevku ažuriranja i mi ga upotrebljavamo za utvrđivanje stanja ažuriranja aplikacije.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator aplikacije

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **Success** – označava je li zadatak kloniranja uspio

- **UpdateID** – Identifikator ažuriranja.


### <a name="configurationchannel"></a>configuration.channel

Ovaj događaj bilježi pokušaje prebacivanja kanala (grupa publike) u alatu MAU.  To koristimo za bilježenje pokušaja i njihovih rezultata (uspjeha ili neuspjeha).

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži odabran naziv kanala.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="configurationmetadata"></a>configuration.metadata

Ovaj se događaj bilježi svaki put kada se MAU inicijalizira. To je MAU impulsna vrsta događaja

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Statični tekst koji označava da se pojedinačni metapodaci inicijaliziraju ili se inicijalizira konfiguracija.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije.

### <a name="configurationsystemversion"></a>configuration.systemVersion

Ovaj događaj označava da je pokušaj dohvaćanja verzije sustava bio neuspješan. On također sadrži podatke o informacijama koje je Microsoftovo automatsko ažuriranje (MAU) uspjelo prikupiti iz sustava. Ovim događajem utvrđujemo je li značajka MAU uzročnik pogrešaka. Napominjemo da se verzija sustava upotrebljava za utvrđivanje može li se ažuriranje primijeniti na klijentski uređaj.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži informacije o pogrešci koja je pronađena tijekom dohvaćanja niza verzije sustava macOS.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="controlleralertmanagerreinstallresponse"></a>controller.alertmanager.reinstallresponse

Ovaj događaj znači da je MAU pao u neupotrebljivo/nepopravljivo stanje i da ga treba ponovno instalirati. Ovaj događaj označava nepopravljivu pogrešku i potrebna je intervencija korisnika.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka provjere ažuriranja

- **Payload** – Sadrži popis nabrojanih korisnika.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="controlleralertmanagertmpdiskfull"></a>controller.alertmanager.tmpdiskfull

Ovaj događaj označava da je otkriveno nedovoljno prostora na disku. Nećemo moći instalirati ažuriranja zbog nedovoljno prostora na disku.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Statični tekst. 

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="controlleralertmanagertmpdiskfullretry"></a>controller.alertmanager.tmpdiskfullretry

Ovaj događaj znači da je pokrenut ponovni pokušaj instaliranja ažuriranja nakon što je otkriveno nedovoljno prostora na disku. Ponovno pokrećemo instalaciju nakon što ne možemo instalirati ažuriranja zbog nedovoljnog prostora na disku.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Statični tekst. 

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije
    

### <a name="controlleralertmanagertmpdiskfullretrycancel"></a>controller.alertmanager.tmpdiskfullretrycancel

Ovaj događaj znači da je pokrenuto otkazivanje pokušaja instaliranja nakon što je otkriveno nedovoljno prostora na disku. Koristimo ovaj događaj da bismo utvrdili je li naš rezervni mehanizam dovoljan da vodi korisnika kroz postupak ažuriranja kada je otkriveno nedovoljno prostora na disku.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)
    
- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja
    
- **Payload** – Statični tekst. 

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="controllercheckwindownoupdatefoundok"></a>controller.checkwindow.noupdatefoundok

Ovaj događaj označava da provjera ažuriranja nije našla ažuriranja. Koristimo ovaj događaj za osiguravanje ispravne ponude ažuriranja, optimiziranje opterećenja usluge i definiranje koliko učestale bi trebale biti provjere ažuriranja. Također želimo optimizirati naš ritam izdanja na temelju očekivanja korisnika o ažuriranjima.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Statični tekst. 

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    

### <a name="controllercheckwindowupdatecheck"></a>controller.checkwindow.updatecheck

Ovaj događaj označava da je izvršena provjera ažuriranja. Koristimo ovaj događaj za osiguravanje ispravne ponude ažuriranja, optimiziranje opterećenja usluge i definiranje koliko učestale bi trebale biti provjere ažuriranja. Također želimo optimizirati naš ritam izdanja na temelju očekivanja korisnika o ažuriranjima.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja
    
- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Statični tekst. 

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="controllercheckwindowupdatecheckcancel"></a>controller.checkwindow.updatecheckcancel

Ovaj događaj označava da je postupak provjere ažuriranja otkazan (ili od korisnika ili od sustava). Koristimo ovaj događaj za osiguravanje ispravne ponude ažuriranja, optimiziranje opterećenja usluge i definiranje koliko učestale bi trebale biti provjere ažuriranja. Također želimo optimizirati naš ritam izdanja na temelju očekivanja korisnika o ažuriranjima.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Statični tekst. 

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="controllercheckwindowupdatecheckcanceluser"></a>controller.checkwindow.updatecheckcanceluser

Ovaj događaj označava da je postupak provjere ažuriranja otkazao korisnik.  Koristimo ovaj događaj za osiguravanje ispravne ponude ažuriranja, optimiziranje opterećenja usluge i definiranje koliko učestale bi trebale biti provjere ažuriranja. Također želimo optimizirati naš ritam izdanja na temelju očekivanja korisnika o ažuriranjima.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije
    
- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Statični tekst. 

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="controllercheckwindowupdatesfound"></a>controller.checkwindow.updatesfound

Ovaj događaj označava da je postupak provjere ažuriranja rezultirao pronalaskom ažuriranja.  Koristimo ovaj događaj za osiguravanje ispravne ponude ažuriranja.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Statični tekst. 

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="controllercheckwindowuptodate"></a>controller.checkwindow.uptodate

Ovaj događaj označava da postupak provjere ažuriranja nije doveo do ažuriranja jer su aplikacije na uređaju ažurne.  Koristimo ovaj događaj za osiguravanje ispravne ponude ažuriranja.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Statični tekst. 

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="controllerdownloadwindowapplaunchwithpendingupdate"></a>controller.downloadwindow.applaunchwithpendingupdate

Ovaj događaj znači da je pokrenuta aplikacija koja je u tijeku ažuriranja. Koristimo ovaj događaj za osiguravanje ispravne ponude ažuriranja. Trebali bismo spriječiti da otvorene aplikacije preuzimaju ažuriranja. Aplikacije moraju biti zatvorene prije ažuriranja.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Statični tekst. 

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese
    
- **SessionId** – Identifikator sesije

    
### <a name="controllerdownloadwindowcloseapplicationdialog"></a>controller.downloadwindow.closeapplicationdialog

Ovaj događaj znači da je pokrenuta aplikacija koja je u tijeku ažuriranja. Koristimo ovaj događaj za osiguravanje ispravne ponude ažuriranja. Trebali bismo spriječiti da otvorene aplikacije preuzimaju ažuriranja. Aplikacije moraju biti zatvorene prije ažuriranja.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Statični tekst. 

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="controllerdownloadwindowcurtasknull"></a>controller.downloadwindow.curtasknull

Ovaj događaj označava da je došlo do neočekivane pogreške tijekom pokušaja primjene ažuriranja. Koristimo ovaj događaj za osiguravanje ispravne ponude ažuriranja.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Statični tekst. 

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="controllerdownloadwindowdownloadcancel"></a>controller.downloadwindow.downloadcancel

Ovaj događaj označava da je postupak preuzimanja otkazao korisnik.  Koristimo ovaj događaj za osiguravanje ispravne ponude ažuriranja.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Statični tekst. 

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="controllerdownloadwindowdownloadfailed"></a>controller.downloadwindow.downloadfailed

Ovaj događaj označava da je došlo do pogreške prilikom preuzimanja ažuriranja. Koristimo ovaj događaj za osiguravanje ispravne ponude i preuzimanja ažuriranja.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="controllerdownloadwindowdownloadfailedok"></a>controller.downloadwindow.downloadfailedok

Ovaj događaj znači da je došlo do pogreške prilikom preuzimanja ažuriranja, a korisnik je obaviješten. Koristimo ovaj događaj za osiguravanje ispravne ponude i preuzimanja ažuriranja, te da se u slučaju neuspjeha korisniku pošalje obavijest.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="controllerdownloadwindowdownloadpathmissing"></a>controller.downloadwindow.downloadpathmissing

Ovaj događaj označava da je došlo do pogreške prilikom preuzimanja ažuriranja. Koristimo ovaj događaj za osiguravanje ispravne ponude i preuzimanja ažuriranja. Ovaj događaj ukazuje da nedostaje URL za preuzimanje.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="controllerdownloadwindowdownloadtasknull"></a>controller.downloadwindow.downloadtasknull

Ovaj događaj označava da je došlo do pogreške prilikom preuzimanja ažuriranja. Koristimo ovaj događaj za osiguravanje ispravne ponude i preuzimanja ažuriranja. Ovaj događaj označava da je od Microsoftova automatskog ažuriranja zatraženo da zaustavi/nastavi preuzimanje, ali nije mogao pronaći odgovarajućeg upravitelja preuzimanja.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="controllerdownloadwindowfilesignaturenotverified"></a>controller.downloadwindow.filesignaturenotverified

Ovaj događaj označava da je došlo do pogreške prilikom preuzimanja ažuriranja. Ovaj događaj označava da alat Microsoftovo automatsko ažuriranje nije mogao provjeriti je li ovo ažuriranje objavio Microsoft. Koristimo ovaj događaj za osiguravanje ispravne ponude i preuzimanja ažuriranja. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji sadrži URL za preuzimanje. Ovo je mjesto za preuzimanje Microsofta, osim ako je kanal postavljen na Prilagođeno. Za prilagođeni kanal ova je vrijednost postavljena na "Prilagođena lokacija".

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="controllerdownloadwindowinstallcomplete"></a>controller.downloadwindow.installcomplete

Ovaj događaj označava da je instalacija svih ažuriranja koje nudi Microsoftovo automatsko ažuriranje dovršena. Koristimo ovaj događaj za osiguravanje ispravne ponude i preuzimanja ažuriranja. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi
    
- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="controllerdownloadwindownetworkunavailablealert"></a>controller.downloadwindow.networkunavailablealert

Ovaj događaj označava da je prilikom preuzimanja ažuriranja izgubljena mrežna povezivost.  Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="controllerdownloadwindownetworkunavailablealertok"></a>controller.downloadwindow.networkunavailablealertok

Ovaj događaj označava da je prilikom preuzimanja ažuriranja izgubljena mrežna povezivost. Također označava da je korisnik obaviješten o ovoj pogrešci. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="controllerdownloadwindownoconnectionok"></a>controller.downloadwindow.noconnectionok

Ovaj događaj označava da je prilikom preuzimanja ažuriranja izgubljena mrežna povezivost. Također označava da je korisnik obaviješten o ovoj pogrešci. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="controllerdownloadwindowrepairrequired"></a>controller.downloadwindow.repairrequired

Ovaj događaj označava da postupak ažuriranja nije uspio. Također označava da je ažuriranje dovršeno, ali je Microsoftovo automatsko ažuriranje pronašlo problem s ažuriranom aplikacijom i potreban je popravak. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)
    
- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja
    
- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="controllerdownloadwindowupdateaborted"></a>controller.downloadwindow.updateaborted

Ovaj događaj označava da je postupak ažuriranja prekinut. Također označava da je ažuriranje već bilo u tijeku u program Daemon, a korisnik je kliknuo U redu da prekine preuzimanje. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="controllerdownloadwindowupdatefailed"></a>controller.downloadwindow.updatefailed

Ovaj događaj označava da jedno ili više ažuriranja iz trenutne serije nije uspjelo. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.
    
- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="controllerdownloadwindowupdatesuccessful"></a>controller.downloadwindow.updatesuccessful

Ovaj događaj označava da su sva ažuriranja iz trenutne serije bila uspješna. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="controllerdownloadwindowuserpaused"></a>controller.downloadwindow.userpaused

Ovaj događaj označava da su sva ažuriranja iz trenutne serije bila uspješna. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="controllerdownloadwindowuserresumed"></a>controller.downloadwindow.userresumed

Ovaj događaj označava da je postupak ažuriranja za preuzimanje uspješno nastavljen nakon pauze. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja
    
- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="controllermainwindowsetautomaticchecking"></a>controller.mainwindow.setautomaticchecking

Ovaj događaj označava da je uređaj registriran u način automatskog ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.

Prikupljaju se sljedeća polja:

 - **App** – Proces aplikacije koji šalje događaj

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – država uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – prva tri okteta IP adrese

- **SessionId** – identifikator sesije


### <a name="controllermainwindowsetautomaticdownloadinstall"></a>controller.mainwindow.setautomaticdownloadinstall

Ovaj događaj označava da je uređaj registriran u način automatskog ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="controllermainwindowsetmanualchecking"></a>controller.mainwindow.setmanualchecking

Ovaj događaj označava da je uređaj registriran u način ručnog ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="controllertemplateawindowcancel"></a>controller.templateawindow.cancel

Ovaj događaj označava da je korisnik odlučio odustati ili zanemariti pruženu poruku upozorenja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="controllertemplateawindowenroll"></a>controller.templateawindow.enroll

Ovaj događaj označava da je korisnik odlučio slijediti pružene preporuke upozorenja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja
    
- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije



### <a name="controllertemplateawindowinstall"></a>controller.templateawindow.install

Ovaj događaj označava da je korisnik odlučio slijediti pruženu preporuku upozorenja koja se odnosi na pokretanje postupka instalacije softvera. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="controllerupdatewindowbegindownloadingapps"></a>controller.updatewindow.begindownloadingapps

Ovaj događaj označava da je preuzimanje ažuriranja započet putem prozora za ažuriranje. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži rječnik dostupnih paketa za ažuriranje i naznaku je li korisnik odabrao da instalira taj unos.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="controllerupdatewindownetworkretry"></a>controller.updatewindow.networkretry

Ovaj događaj označava da je pokušaj ponovnog pokretanja aktiviran na listu za ažuriranje zbog kvara na mreži. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="controllerupdatewindownetworkretrycancel"></a>controller.updatewindow.networkretrycancel

Ovaj događaj označava da pokušaj ponovnog pokretanja ne može biti aktiviran na listu za ažuriranje zbog kvara na mreži. Ovaj događaj označava korisnika izabranog da otkaže ažuriranja nakon što je upozoren da mreža postaje nedostupna. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="controllerupdatewindownetworkunavailable"></a>controller.updatewindow.networkunavailable

Ovaj događaj označava da je mrežna povezivost odjednom izgubljena. Ovaj događaj ukazuje na to da poslužitelj nije dostupan pri pokušaju preuzimanja paketa za ažuriranje. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="controllerupdatewindownoupdateavailable"></a>controller.updatewindow.noupdateavailable

Ovaj događaj označava da je bilo traženja ažuriranja koje je rezultiralo time da nema dostupnih ažuriranja. Ovaj događaj označava da Microsoftovo automatsko ažuriranje nije pronašlo nikakva dostupna ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="controllerupdatewindownoupdatestoselect"></a>controller.updatewindow.noupdatestoselect

Ovaj događaj označava da je došlo do pogreške koja je rezultirala praznim popisom ažuriranja. Ovaj događaj označava da Microsoftovo automatsko ažuriranje prikazuje prazan list za ažuriranje. To se ne bi smjelo dogoditi. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="controllerupdatewindowupdateavailable"></a>Controller.UpdateWindow.UpdateAvailable

Ovaj događaj označava da je bilo traženja ažuriranja koje je rezultiralo time da su ponuđena ažuriranja. To koristimo čak i da utvrdimo nude li se ažuriranja za pregled korisnika, prikazuju li se ispravna ažuriranja ili funkcionira li blokiranje ažuriranja kako se očekuje. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži rječnik dostupnih paketa za ažuriranje i status odabira korisnika za svaki.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="controllerupdatewindowupdateavailablecancel"></a>controller.updatewindow.updateavailablecancel

Ovaj događaj označava da je korisnik otkazao nakon što smo prikazali listu ažuriranja s popisom ažuriranja. Ovaj događaj koristimo da objasnimo razloge za neažuriranje (tj. korisnik ih svojevoljno otkaže). Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="downloadactorpause"></a>downloadactor.pause

Ovaj događaj označava da je korisnik izdao zahtjev za pauziranje preuzimanja. Ovaj događaj koristimo i da objasnimo razloge za ažuriranja koja očito nisu dovršena. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="downloadactorredirect"></a>downloadactor.redirect

Ovaj događaj označava da je agent za preuzimanje usmjeren na krajnju točku koja izdaje URL preusmjeravanje za zahtjev za preuzimanje. To koristimo čak i da objasnimo razloge za neuspjeh u preuzimanju i dijagnosticiranje problema proxy poslužitelja. Također može pomoći u dijagnosticiranju razloga zbog kojih je primijećeno da korisnici instaliraju starije verzije. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži preusmjereni URL. Ovo je mjesto za preuzimanje Microsofta, osim ako je kanal postavljen na Prilagođeno. Za prilagođeni kanal ova je vrijednost postavljena na "Prilagođena lokacija".

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="downloadactorresume"></a>downloadactor.resume

Ovaj događaj označava da korisnik postavlja zahtjev za nastavak zaustavljenog preuzimanja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="downloadactorresumeerror"></a>downloadactor.resumeerror

Ovaj događaj označava da korisnik postavlja zahtjev za nastavak zaustavljenog preuzimanja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži put URL-a za preuzimanje. Ovo je mjesto za preuzimanje Microsofta, osim ako je kanal postavljen na Prilagođeno. Za prilagođeni kanal ova je vrijednost postavljena na "Prilagođena lokacija".

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="downloadactorstatus"></a>downloadactor.status

Ovaj događaj bilježi da postoje pokušaji dohvaćanja datoteka elemenata osiguranja i njihovih rezultata (uspjeh ili neuspjeh). Želimo znati elemente osiguranja i pakete koji se preuzimaju. Dobivena pogrešna datoteka može ukazivati na problem međuverzije/elementa osiguranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži URL za preuzimanje te kôd pogreške u slučaju neuspjeha. URL za preuzimanje je mjesto za preuzimanje Microsofta, osim ako je kanal postavljen na Prilagođeno. Za prilagođeni kanal ova je vrijednost postavljena na "Prilagođena lokacija".

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="downloadmanifestconfiguration"></a>downloadmanifest.configuration

Ovaj događaj izvješćuje o pogrešci s konfiguracijom značajke Microsoftovo automatsko ažuriranje (MAU) – bez obzira na to je li riječ o postavljanju prilagođenog poslužitelja ili definicijama krajnjih točaka u pomoćniku za ažuriranje u instaliranim komponentama MAU-a. Ovim događajem savjetujemo IT administratore za postavljanje točnih krajnjih točaka poslužitelja manifesta.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **Payload** – Označava je li pogreška povezana s postavljanjem prilagođenog poslužitelja ili instaliranim komponentama MAU-a

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="downloadmanifestdownloadcatalogfail"></a>downloadmanifest.downloadcatalogfail

Ovaj događaj označava da je došlo do pogreške pri preuzimanju. Datoteka koja nije uspjela preuzeti je zabilježena. Želimo znati elemente osiguranja i pakete koji se preuzimaju. Neuspjeh u preuzimanju manifesta može značiti ili neuspjeh generiranja verzije elementa osiguranja, pogrešku u konfiguraciji CDN-a, pogrešku u konfiguraciji klijenta i mrežnu pogrešku. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži kôd pogreške i URL datoteke za preuzimanje. Ovo je mjesto za preuzimanje Microsofta, osim ako je kanal postavljen na Prilagođeno. Za prilagođeni kanal ova je vrijednost postavljena na "Prilagođena lokacija".

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="downloadmanifestdownloadcatalogsuccess"></a>downloadmanifest.downloadcatalogsuccess

Ovaj događaj označava da je datoteka uspješno preuzeta. Neuspjeh u preuzimanju manifesta može značiti ili neuspjeh generiranja verzije elementa osiguranja, pogrešku u konfiguraciji CDN-a, pogrešku u konfiguraciji klijenta i mrežnu pogrešku. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja
    
- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži kôd pogreške i URL datoteke za preuzimanje. Ovo je mjesto za preuzimanje Microsofta, osim ako je kanal postavljen na Prilagođeno. Za prilagođeni kanal ova je vrijednost postavljena na "Prilagođena lokacija".

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="downloadmanifestdownloadfail"></a>downloadmanifest.downloadfail

Ovaj događaj znači da je došlo do pogreške pri preuzimanju. Evidentira se datoteka manifesta ili paketa koja nije uspjela biti preuzeta, kao i detalji pogreške. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži kôd pogreške i URL datoteke za preuzimanje. Ovo je mjesto za preuzimanje Microsofta, osim ako je kanal postavljen na Prilagođeno. Za prilagođeni kanal ova je vrijednost postavljena na "Prilagođena lokacija".

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="downloadmanifestdownloadfromurl"></a>downloadmanifest.downloadfromurl

Ovaj događaj označava da je počelo preuzimanje datoteke kataloga. Evidentiramo URL s kojeg se datoteka kataloga preuzima. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži kôd pogreške i URL datoteke za preuzimanje. Ovo je mjesto za preuzimanje Microsofta, osim ako je kanal postavljen na Prilagođeno. Za prilagođeni kanal ova je vrijednost postavljena na "Prilagođena lokacija".

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="downloadmanifestdownloading"></a>downloadmanifest.downloading

Ovaj događaj označava da je počelo preuzimanje datoteke kataloga. Evidentiramo URL s kojeg se datoteka kataloga preuzima. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži kôd pogreške i URL datoteke za preuzimanje. Ovo je mjesto za preuzimanje Microsofta, osim ako je kanal postavljen na Prilagođeno. Za prilagođeni kanal ova je vrijednost postavljena na "Prilagođena lokacija".

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="downloadmanifestdownloadsuccess"></a>downloadmanifest.downloadsuccess

Ovaj događaj označava da je preuzimanje XML datoteke i datoteke paketa uspjelo. Evidentiramo URL s kojeg se datoteka preuzima. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži kôd pogreške i URL datoteke za preuzimanje. Ovo je mjesto za preuzimanje Microsofta, osim ako je kanal postavljen na Prilagođeno. Za prilagođeni kanal ova je vrijednost postavljena na "Prilagođena lokacija".

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="downloadmanifestdownloadurl"></a>downloadmanifest.downloadurl

Ovaj događaj označava da je došlo do zahtjeva za preuzimanje datoteke. Evidentiramo URL s kojeg se datoteka preuzima. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja
    
- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži kôd pogreške i URL datoteke za preuzimanje. Ovo je mjesto za preuzimanje Microsofta, osim ako je kanal postavljen na Prilagođeno. Za prilagođeni kanal ova je vrijednost postavljena na "Prilagođena lokacija".

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="downloadmanifestfilenameerror"></a>downloadmanifest.filenameerror

Ovaj događaj označava da je došlo do neočekivane pogreške. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="downloadmanifestinvalidhash"></a>downloadmanifest.invalidhash

Ovaj događaj označava sigurnosnu provjeru datoteka koje nisu uspjele. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži naziv preuzete datoteke s nevažećom vrijednošću raspršivanja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="downloadmanifestmissingdaemon"></a>downloadmanifest.missingdaemon

Ovaj događaj označava da je korisnik pokušao provjeriti ima li ažuriranja, a otkrili smo da alatu MAU nedostaje osnovna komponenta (daemon). Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="downloadmanifestsignatureerror"></a>downloadmanifest.signatureerror

Ovaj događaj označava da provjera autentičnosti kôda nije uspjela za paket. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži naziv preuzete datoteke s nevažećom vrijednošću raspršivanja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="downloadmanifeststatus"></a>downloadmanifest.status

Ovaj događaj evidentira sažeto skupljanje pokušaja/neuspjeha na koje se naišlo tijekom postupka preuzimanja datoteka manifesta i paketa. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži podatke uključujući URL (Microsoftova adresa), prefiks datoteke koja se preuzima, uočene pogreške itd.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="downloadmgrdownloadend"></a>downloadmgr.downloadend

Ovaj događaj evidentira oznaku koja pokazuje da je postupak preuzimanja dovršen sam. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži podatke uključujući URL (Microsoftova adresa), prefiks datoteke koja se preuzima, uočene pogreške itd.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="downloadmgrdownloadstart"></a>downloadmgr.downloadstart

Ovaj događaj evidentira ažuriranje koje će se uskoro preuzeti. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži naziv ažuriranja koje se preuzima.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="downloadtaskdownloadbegin"></a>downloadtask.downloadbegin

Ovaj događaj označava početak aktivnosti preuzimanja za ažuriranje aplikacije. On predstavlja dio lijevka ažuriranja i mi ga upotrebljavamo za utvrđivanje stanja ažuriranja aplikacije.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **BundleVersion** – Verzija aplikacije koja se ažurira

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **PreviousUpdateID** – Identifikator za ažuriranje aplikacije

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator za ažuriranje aplikacije

- **UpdatePkg** – Naziv paketa ažuriranja koji se primjenjuje

- **UpdateVersion** – Verzija aplikacije nakon ažuriranja


### <a name="downloadtaskdownloadfailure"></a>downloadtask.downloadfailure

Ovaj događaj evidentira da je došlo do pogreške prilikom preuzimanja datoteke paketa. Evidentiramo put ažuriranja te pogrešku. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator aplikacije čije preuzimanje nije uspjelo.

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Error** – Pogreška koja je uočena tijekom preuzimanja.

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži naziv ažuriranja koje se preuzima i uočenu pogrešku. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator ažuriranja koje se preuzima.


### <a name="downloadtaskdownloadsuccess"></a>downloadtask.downloadsuccess

Uspješno preuzimanje datoteke paketa. Evidentiramo korišten put ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator aplikacije.

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži put ažuriranja za uspješno preuzimanje.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator preuzetog ažuriranja.

### <a name="downloadtaskupdatertypeerror"></a>downloadtask.updatertypeerror

Ovaj događaj izvješćuje o zatipku alata za ažuriranje u preuzetoj datoteci manifesta. Ovim događajem obavještavamo vlasnika datoteke manifesta kako bi se ta pogreška mogla ispraviti.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator za ažuriranje aplikacije

- **UpdaterType** – Vrsta alata za ažuriranje specificirana u preuzetoj datoteci manifesta

- **UpdateURL** – URL paketa ažuriranja koji treba primijeniti

### <a name="downloadtaskurlerror"></a>downloadtask.urlerror

Ovaj događaj izvješćuje o pogrešci u URL-u specificiranom u preuzetoj datoteci manifesta. Ovim događajem obavještavamo vlasnika datoteke manifesta kako bi se ta pogreška mogla ispraviti.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **Error** – Označava vrstu pogreške koja se pojavljuje

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator za ažuriranje aplikacije

- **UpdateURL** – URL paketa ažuriranja koji treba primijeniti

### <a name="fbachangelastupdate"></a>fba.changelastupdate

Ovaj događaj izvješćuje o tome kada je značajka Microsoftovo automatsko ažuriranje (MAU) provjerila ažuriranja. Ovim događajem ispravljamo pogreške kada određenom uređaju nije bilo ponuđeno ažuriranje tijekom duljeg razdoblja.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **Payload** – Sadrži datum i vrijeme kada je značajka MAU provjerila ima li ažuriranja

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbacheckforupdate"></a>fba.checkforupdate

Ovaj događaj označava da pozadinski postupak provjerava postoje li ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbacheckforupdateskip"></a>fba.checkforupdateskip

Ovaj događaj označava da je pozadinski proces preskočio ažuriranje zbog otvaranja grafičkog korisničkog sučelja MAU. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbaforceinstallmsgsent"></a>fba.forceinstallmsgsent

Ovaj događaj označava da je pokrenuto prisilno ažuriranje putem korisničkog sučelja. Ovaj događaj tvori dio lijevka i upotrebljava se za utvrđivanje stanja značajke prisilnog ažuriranja.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="fbaforceupdatecheck"></a>fba.forceupdatecheck

Ovaj događaj označava da je provjera ima li ažuriranja prisilna. Ovim događajem utvrđujemo količinu provjera ima li prisilnih ažuriranja koje se događaju izvan normalnog ciklusa provjere ima li ažuriranja.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="fbaguiappopen"></a>fba.guiappopen

Ovaj događaj označava da se korisničko sučelje pokreće u načinu rada Automatska provjera jer je aplikacija s primjenjivim ažuriranjem trenutačno otvorena. Ovim se događajem utvrđuje količina pokretanja korisničkog sučelja iz načina rada Automatska provjera za budući razvoj značajki.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="fbainstallpending"></a>fba.installpending

Ovaj događaj označava da je značajka Microsoftovo automatsko ažuriranje (MAU) poslala obavijest u vezi s ažuriranjima na čekanju. Ovim se događajem utvrđuje količina ažuriranja koja se pokreću iz korisničkih obavijesti i on se upotrebljava za poboljšanje korisničkog doživljaja smanjenjem prekida za korisnika u budućim izdanjima.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="fbalaunch"></a>fba.launch

Ovaj događaj označava pokretanje Microsoftova pomoćnika za ažuriranje s pomoću postupka pokretanja. Ovim se događajem utvrđuje pokreće li se Microsoftov pomoćnik za ažuriranje u neodgovarajućem kontekstu.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="fbalaunchbyagent"></a>fba.launchbyagent

Ovaj događaj označava da je Microsoftov pomoćnik za ažuriranje pokrenut putem agenta za pokretanje. Ovim se događajem utvrđuje količina pokretanja Microsoftova pomoćnika za ažuriranje iz korisničkog sučelja za budući razvoj.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="fbalaunchfromprotocol"></a>fba.launchfromprotocol

Ovaj događaj označava da je Microsoftov pomoćnik za ažuriranje pokrenut putem protokola URL-a. Ovim se događajem utvrđuje količina pokretanja Microsoftova pomoćnika za ažuriranje putem URL-a za budući razvoj.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Sadrži informacije o shemi URL-a i domaćinu URL-a

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="fbalaunchgui"></a>fba.launchgui

Ovaj događaj označava da Microsoftov pomoćnik za ažuriranje pokušava pokrenuti grafičko korisničko sučelje (GUI). Ovim se događajem utvrđuje količina pokretanja korisničkog sučelja koja su pokrenuta putem Microsoftova pomoćnika za ažuriranje radi pružanja pomoći za budući razvoj, uključujući smanjenje smetnji za korisnika uslijed čestih pokretanja korisničkog sučelja.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbalaunchstatus"></a>fba.launchstatus

Ovaj događaj evidentira neuspjehe MAU daemona prilikom pokušaja pokretanja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Error** – Sadrži OSStatus (Apple statusni kôd) koji odražava status pokretanja.

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži OSStatus (Apple statusni kôd) koji odražava status pokretanja. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

- **Success** – Booleov niz koji označava je li postupak MAU daemon uspješno pokrenut.


### <a name="fbamausilentupdate"></a>fba.mausilentupdate

Ovaj događaj označava da Microsoftov pomoćnik za ažuriranja pokreće tiha ažuriranja. Ovim se događajem utvrđuje količina ažuriranja koja se primjenjuju bez intervencije korisnika kako bi se olakšala poboljšanja korisničkog doživljaja.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije
 
- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="fbamoreinfofromappnotification"></a>fba.moreinfofromappnotification

Ovaj događaj izvješćuje o informacijama koje registrirana aplikacija usmjerava putem značajke Microsoftova automatska ažuriranja (MAU). Na primjer, poruke o završetku pružanja usluge izdaju se putem obavijesti MAU-a. Ovim događajem utvrđujemo količinu uređaja na kojima se prikazuje ta obavijest radi utvrđivanja uspjeha distribucije podataka.

Prikupljaju se sljedeća polja:

- **AdditionalInfoID** – Jedinstveno prepoznaje „Dodatne informacije” koje se izdaju putem MAU-a.

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **NotificationEvent** – Statični tekst koji označava koja se vrsta obavijesti primjenjuje.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="fbamultipledaemon"></a>fba.multipledaemon

Ovaj događaj označava da je prepoznata dodatna instanca Microsoftova pomoćnika za ažuriranje i da će se trenutačna instanca okončati. Ovim ćemo događajem utvrđivati količinu uređaja koji pokušavaju pokrenuti višestruke instance pomoćnika za ažuriranja i, po potrebi, stvoriti zaobilazno rješenje.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="fbanofifyappclosed"></a>fba.nofifyappclosed

Ovaj događaj označava da Microsoftov pomoćnik za ažuriranja izdaje obavijest za ažuriranja na čekanju jer ne postoje otvorene registrirane aplikacije, a ažuriranja se mogu provesti bez ometanja korisnika. Ovim događajem utvrđujemo količinu ažuriranja koja se mogu primijeniti, no za što im je potrebna radnja korisnika. Ovim se događajem potiču poboljšanja korisničkog doživljaja.

Prikupljaju se sljedeća polja: 
    
- **App** – Proces aplikacije za slanje događaja
    
- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi
    
- **AppversionLong** – Verzija aplikacije
    
- **Channel** – Preference za publiku
    
- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)
    
- **DeviceID** – Identifikator uređaja
    
- **DeviceInfo_Model** – Hardverski model uređaja
    
- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)
    
- **DeviceInfo_OsBuild** – Verzija operacijskog sustava
    
- **Event_ReceivedTime** – Vrijeme primanja telemetrije
    
- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje
    
- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 
    
- **HowToCheck** – Način provjere postavke
    
- **Payload** – Statični tekst
    
- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)
    
- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese
    
- **SessionId** – Identifikator sesije

### <a name="fbanofifyappopen"></a>fba.nofifyappopen

Ovaj događaj označava da Microsoftov pomoćnik za ažuriranja izdaje obavijest za ažuriranja na čekanju jer postoje otvorene registrirane aplikacije, a za instalaciju ažuriranja te će se aplikacije morati zatvoriti.  Ovim događajem utvrđujemo količinu ažuriranja za koje je potrebna radnja korisnika.  Ovim se događajem potiču poboljšanja korisničkog doživljaja.

Prikupljaju se sljedeća polja:  

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi
    
- **AppversionLong** – Verzija aplikacije
    
- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="fbasettimerfail"></a>fba.settimerfail  

Ovaj događaj označava neuspjeli pokušaj za postavljanje brojača za pokretanje budućeg ažuriranja. Ovaj je događaj ključan, a mi tim događajem utvrđujemo količinu pogreški kako bismo, po potrebi, stvorili zaobilazno rješenje.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Sadrži informacije o vremenu zadnjeg ažuriranja i upotrebi kalendara

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdateoptin"></a>fba.silentupdateoptin

Ovaj događaj označava da se korisnik odlučio za tiha ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="fbaskipforcedupdate"></a>fba.skipforcedupdate

Ovaj događaj ukazuje na to da se prisilna provjera ažuriranja preskače zbog otvorenih aplikacija. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbastartforcedupdate"></a>fba.startforcedupdate

Ovaj događaj označava da je došlo do pokušaja primjene prinudnog ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbaterminate"></a>fba.terminate

Ovaj događaj označava da se MAU daemon normalno prekinuo. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbaupdatefound"></a>fba.updatefound

Ovaj događaj ukazuje da je MAU daemon pronašao dostupna ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži broj dostupnih ažuriranja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="fbaupdatetimer"></a>fba.updatetimer

Ovaj događaj ukazuje na to da je proces Microsoftovo automatsko ažuriranje Daemon postao aktivan za provjeru ažuriranja nakon spavanja određeno vrijeme. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži podatke o trenutnom datumu i vremenu.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdateallappsclosed"></a>fbasilentupdate.allappsclosed

Ovaj se događaj evidentira ako su sve aplikacije bile zatvorene prije instalacije. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku
    
- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdateapplaunchafterupdate"></a>fbasilentupdate.applaunchafterupdate

Ovaj događaj bilježi pokušaj ponovnog pokretanja aplikacije nakon tihog ažuriranja i načina ažuriranja (klon ili ne). Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator aplikacije.

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Error** – Pojedinosti o pogrešci do koje je došlo prilikom pokretanje aplikacije nakon ažuriranja.

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja i naziva aplikacije koja se pokreće. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*
    
- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)
    
- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdateapplaunchwileinstalling"></a>fbasilentupdate.applaunchwileinstalling

Evidentiramo kada je došlo do pokretanja aplikacije tijekom instalacije ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdateappneedtoclose"></a>fbasilentupdate.appneedtoclose

Evidentiramo kada je započeo postupak ažuriranja i utvrđujemo da je aplikacija za ažuriranje otvorena. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja, naziva ažuriranja i ID paketa aplikacije.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdateappterminationeventreceived"></a>fbasilentupdate.appterminationeventreceived

Ovaj događaj označava da Microsoftovo automatsko ažuriranje primilo Apple događaj kojim se obavještava da je aplikacija prekinuta. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator aplikacije.

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Error** – Pojedinosti o pogrešci do koje je došlo prilikom ukidanja aplikacije.

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja i ID paketa aplikacije. Može također sadržavati niz pogrešaka ako Microsoftovo automatsko ažuriranje utvrdi da aplikacija i dalje radi iako je zaprimljen događaj prekida. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator ažuriranja aplikacije.


### <a name="fbasilentupdateclientsession"></a>FBASilentUpdate.ClientSession

Ovaj se događaj upotrebljava za izračunatu metriku stanja ključnih ažuriranja za značajku Microsoftova automatska ažuriranja (MAU). Ovaj nam događaj omogućava saznati koju sesiju ažuriranja (preuzimanje ili instalacija) pozadinski sustav trenutačno obrađuje.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije koji šalje događaj

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Označava koju sesiju ažuriranja (preuzimanje ili instalacija) pozadinski sustav trenutačno obrađuje.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdatecodesignfailure"></a>fbasilentupdate.codesignfailure

Ovaj događaj bilježi rezultat provjere autentičnosti kôda nakon primjene ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži rezultat operacije provjere autentičnosti kôda.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdatedownload"></a>fbasilentupdate.download

Ovaj događaj označava da se preuzima ažuriranje. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja i naziva ažuriranja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **ScreenLocked** – indikacija je li preuzimanje pokrenuto iza zaključanog zaslona

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdatedownloadfailed"></a>fbasilentupdate.downloadfailed

Ovaj događaj označava da je došlo do pogreške tijekom preuzimanja ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator aplikacije.

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Error** – Pojedinosti o pogrešci do koje je došlo prilikom preuzimanja ažuriranja aplikacije.

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja i naziva ažuriranja. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator ažuriranja aplikacije.

- **UpdateName** – Naziv ažuriranja aplikacije.


### <a name="fbasilentupdatedownloadinbackground"></a>fbasilentupdate.downloadinbackground

Ovaj događaj označava da započinjemo s preuzimanjem skupa ažuriranja u pozadini (bilježimo broj istodobnih preuzimanja). Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži broj ažuriranja u redu čekanja.

    - **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdatedownloadingrepairupdate"></a>fbasilentupdate.downloadingrepairupdate

Ovaj događaj označava da smo pokrenuli pokušaj preuzimanja popravka zbog neuspjelog ažuriranja. Evidentiramo verziju i ažuriranje. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja i naziva ažuriranja.
    
- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **ScreenLocked** – indikacija je li preuzimanje pokrenuto iza zaključanog zaslona

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdateduplicatedownloadattempted"></a>fbasilentupdate.duplicatedownloadattempted

Ovaj događaj označava da je došlo do pogreške. Istovremeno trebamo preuzeti samo jedno ažuriranje za određenu aplikaciju. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdateinstallattemptfailed"></a>fbasilentupdate.installattemptfailed

Ovaj događaj znači da pokušaja instalacije ažuriranja (verzije) nije uspio. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdateinstallcomplete"></a>fbasilentupdate.installcomplete

Ovaj događaj označava da su sva ažuriranja u grupi završena instalacijom. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdateinstalled"></a>fbasilentupdate.installed

Ovaj događaj označava da je pojedinačno ažuriranje uspješno instalirano. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja. Sadrži identifikator ažuriranja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="fbasilentupdateinstalling"></a>fbasilentupdate.installing

Ovaj događaj označava da je pokrenuto pojedinačno ažuriranje. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja, naziva ažuriranja i naziva paketa ažuriranja.
    
- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="fbasilentupdateinstallstatus"></a>fbasilentupdate.installstatus

Ovaj događaj izvješćuje o statusu zadatka ažuriranja aplikacije. Ovaj događaj predstavlja dio lijevka za ažuriranje aplikacije i mi ga upotrebljavamo za nadzor stanja ažuriranja aplikacije.

Prikupljaju se sljedeća polja: 

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Sadrži informacije o tome prikazuje li se prikaz napretka

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **Success** – Označava je li ažuriranje aplikacije bilo uspješno

- **UpdateID** – Identifikator za ažuriranje aplikacije

- **UpdateName** – Naziv ažuriranja u obliku koji se prikazuje u preuzetoj datoteci manifesta

- **UpdatePkg** – Naziv paketa ažuriranja koji se primjenjuje

### <a name="fbasilentupdatenotificationerror"></a>fbasilentupdate.notificationerror

Ovaj događaj izvješćuje o pogrešci koja se pojavila tijekom pokušaja slanja korisničke obavijesti. Ovim događajem ispravit će se pogreške uzroka pogreške i poduzeti mjere za ispravljanje.

Prikupljaju se sljedeća polja:  

- **App** – Proces aplikacije za slanje događaja
 
- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **ErrType** – Označava vrstu pogreške koja se pojavljuje

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Message** – Sadržaj obavijesti

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **Title** – Naslov obavijesti

- **Type** – Vrsta obavijesti

### <a name="fbasilentupdatenotificationremoved"></a>fbasilentupdate.notificationremoved

Ovaj događaj označava da ažuriranje koje je bilo blokirano više nije blokirano. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži ID aplikacije (identifikator se aplikacija koristi za registraciju na uslugu Microsoftova automatskog ažuriranja) za prethodno blokiranu aplikaciju
    
- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdatequeueinstall"></a>fbasilentupdate.queueinstall

Ovaj događaj znači da će ažuriranje biti u redu čekanja za tihu instalaciju. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja i naziva ažuriranja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdaterequiredappsclosed"></a>fbasilentupdate.requiredappsclosed

Evidentiramo kada je aplikacija koja ima ažuriranje na čekanju zatvorena. To označava vrijeme tijekom kojeg je moguće nastaviti s instalacijom. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja i ID paketa aplikacije.
    
- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="fbasilentupdatetimerforapptermination"></a>FBASilentUpdate.TimerForAppTermination

Ovaj se događaj upotrebljava za izračunatu metriku stanja ključnih ažuriranja za značajku Microsoftova automatska ažuriranja (MAU). Ovaj nam događaj omogućava praćenje događaja prekida otvorene aplikacije i trajanje razdoblja tijekom kojeg je bila otvorena.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije koji šalje događaj

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Označava je li za otvorenu aplikaciju bio postavljen brojač kada je aktivirana instalacija njezina ažuriranja. 

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="fbasilentupdateupdateavailablenotification"></a>fbasilentupdate.updateavailablenotification

Ovaj događaj označava da se aktivira obavijest o dostupnosti ažuriranja. Moramo osigurati da se tijek upita za ažuriranja aktivira kada se otkrije ažuriranje. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdateuserclicknotification"></a>fbasilentupdate.userclicknotification

Ovaj događaj ukazuje da je korisnik kliknuo na odjeljak sa sadržajem obavijesti o dostupnom ažuriranju i pokrenuto je grafičko korisničko sučelje Microsoftova automatskog ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdateuserselectinstalllater"></a>fbasilentupdate.userselectinstalllater

Ovaj događaj ukazuje na to da se korisnik odlučio instalirati kasnije nakon prikazane obavijesti o dostupnom ažuriranju. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdateuserselectinstallnow"></a>fbasilentupdate.userselectinstallnow

Ovaj događaj ukazuje na to da se korisnik odlučio instalirati odmah nakon prikazane obavijesti o dostupnom ažuriranju. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="guidashboardviewappisopendialogdisplay"></a>gui.dashboardview.appisopendialog.display 

Ovaj događaj označava da je korisničko sučelje prikazalo dijaloški okvir za zatvaranje otvorene aplikacije radi nastavka ažuriranja aplikacije. Ovim se događajem utvrđuje količina ažuriranja koja se odgađaju kako bi se pružila buduća poboljšanja za smanjenje prekida korisnika.

Prikupljaju se sljedeća polja: 

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator za ažuriranje aplikacije

- **UpdateName** – Naziv ažuriranja u obliku koji se prikazuje u preuzetoj datoteci manifesta

### <a name="guidashboardviewappisopendialogbuttonclicked"></a>gui.dashboardview.appisopendialogbutton.clicked

Ovaj događaj označava je li ažuriranje aplikacije preskočeno ili se nakon prikazivanja otvorenog dijaloškog okvira aplikacije provodi drugi pokušaj. Ovim se događajem utvrđuje količina ažuriranja koja se preskaču i upotrebljavaju kako bi se pružila buduća poboljšanja za smanjenje prekida korisnika.

Prikupljaju se sljedeća polja:   

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **ButtonType** – Preskakanje ili ponovni pokušaj

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja 

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator za ažuriranje aplikacije

- **UpdateName** – Naziv ažuriranja u obliku koji se prikazuje u preuzetoj datoteci manifesta

### <a name="guidashboardviewupdateinprogressdialogdisplay"></a>gui.dashboardview.updateinprogressdialog.display

Ovaj događaj bilježi je li dijaloški okvir koji označava da je ažuriranje već u tijeku bio prikazan korisnicima.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije koji šalje događaj

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="guidashboardviewupdatemodebuttonclicked"></a>gui.dashboardview.updatemodebutton.clicked

Ovaj događaj označava način rada ažuriranja koji je promijenjen iz korisničkog sučelja. Ovim se događajem utvrđuje količina uređaja koji prelaze iz jednog načina rada u drugi i on se upotrebljava kao pomoć za utvrđivanje zašto korisnici odustaju od automatskih ažuriranja. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja
 
- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Označava je li automatsko preuzimanje isključeno

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="guifeedbackwindowbuttonclicked"></a>gui.feedbackwindow.buttonclicked

Ovaj događaj izvješćuje o tome jesu li povratne informacije poslane ili otkazane prije slanja. Ovim se događajem utvrđuje količina povratnih informacija koje se šalju za dotičnu verziju izdanja. To omogućuje prijevremenu izolaciju potencijalnih problema.

Prikupljaju se sljedeća polja: 

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **ButtonType** – Označava jesu li povratne informacije poslane ili otkazane

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava
 
- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="guipreferenceviewconsentsheetdisplay"></a>gui.preferenceview.consentsheet.display

Ovaj događaj označava da se prikazuje list za privolu za određeni kanal ako postoji. Ovim se događajem utvrđuje količina uređaja koji su novo upisani u primjenjivi kanal publike (raniji Insider / kasniji Insider). Također, taj događaj upotrebljavamo da bismo osigurali da prikaz dijaloškog okvira za suglasnost funkcionira za prikaz uvjeta korištenja korisnicima.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **ChannelName** – kanal za koji se prikazuje dijaloški okvir za pristanak

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="guipreferenceviewconsentsheetlicenseerror"></a>gui.preferenceview.consentsheet.licenseerror

Ovaj događaj izvješćuje o pogrešci koja se pojavila tijekom pokušaja prikaza dijaloškog okvira za suglasnost. Ovaj je događaj ključan i upotrebljava se za ispravljanje svih problema uzrokovanih promjenom proizvoda ako je to primjenjivo.

Prikupljaju se sljedeća polja: 

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **ErrorCode** – Pronađeni kôd pogreške

- **ErrorDomain** – Domena pogreške

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="guipreferenceviewswitchchannel"></a>gui.preferenceview.switchchannel

Ovaj događaj izvješćuje o prijelazu između kanala koje je odabrao korisnik. Ovim se događajem utvrđuje zašto korisnici odustaju od kanala Insidera.  

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **PickedFrom** – Stari kanal

- **PickedTo** – Novi kanal

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="guiupdatemanagerapplaunchduringupdate"></a>gui.updatemanager.applaunchduringupdate

Ovaj događaj izvješćuje da je aplikacija pokrenuta dok se ažurirala, a značajka Microsoftovo automatsko ažuriranje prekida pokrenutu aplikaciju. Napominjemo da pokretanje aplikacije dok se ona ažurira može dovesti do oštećenja aplikacije. Ovim događajem osiguravamo da pokretanje aplikacije ne utječe na proces ažuriranja prije no što ona ude spremna za upotrebu.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator aplikacije koja je pokrenuta tijekom ažuriranja.

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **Success** – Vrijednost Booleova niza koja označava je li aplikacija uspješno zatvorena.

- **UpdateID** – Identifikator ažuriranja aplikacije.

### <a name="guiupdatemanagerdownloadupdateforapp"></a>gui.updatemanager.downloadupdateforapp

Ovaj događaj izvješćuje o statusu dovršavanja preuzimanja za ažuriranje. Ovim događajem osiguravamo stanje procesa ažuriranja i pratimo/rješavamo točku pogreške.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator aplikacije.

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **IsRepair** – Booleov niz označava je li određeno ažuriranje preuzimanje popravka.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **isRepair** – Označava je li preuzimanje bilo za preuzimanje popravka za prethodno neuspješno ažuriranje.

- **UpdateID** – Identifikator ažuriranja.

- **UpdateName** – Naziv ažuriranja.


### <a name="guiupdatemanagererror"></a>gui.updatemanager.error

Ovaj događaj izvješćuje o svim pogreškama koje se javljaju tijekom ažuriranja aplikacije. On može označavati pogrešku u slijedu izvršavanja značajke Microsoftovo automatsko ažuriranje (MAU).  Ovim izvješćem primjenjujemo ažuriranja za MAU kako bismo riješili scenarije uobičajenih pogrešaka.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije koji šalje događaj

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži informacije o pogreškama koje se pojavljuju tijekom ažuriranja aplikacije.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **Success** – Vrijednost Booleova niza koja označava je li aplikacija uspješno zatvorena.

### <a name="guiupdatemanagerinstallcleanupforapp"></a>gui.updatemanager.installcleanupforapp

Ovaj događaj označava da su privremene datoteke koje su stvorene tijekom instalacije aplikacije uspješno očišćene. On predstavlja dio lijevka ažuriranja koji se upotrebljava za utvrđivanje stanja ažuriranja aplikacije.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije koji šalje događaj

- **AppID** – Identifikator aplikacije.

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppState** – Cijeli broj označava stanje aplikacije nakon pokušaja ažuriranja.

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator ažuriranja.


### <a name="guiupdatemanagerinstallsuccessforapp"></a>gui.updatemanager.installsuccessforapp

Ovaj događaj označava uspješno ažuriranje aplikacije. Ovaj događaj predstavlja dio lijevka ažuriranja koji upotrebljavamo za utvrđivanje stanja ažuriranja.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator aplikacije.

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **Success** – Booleov niz označava jesu li ažuriranja uspješno instalirana.

- **UpdateID** – Identifikator ažuriranja.

### <a name="guiupdatemanagerinstallupdateforapp"></a>gui.updatemanager.installupdateforapp

Ovaj događaj označava početak stvarnog instalacijskog procesa za ažuriranje aplikacije. Ovaj događaj predstavlja dio lijevka ažuriranja aplikacije koji upotrebljavamo za utvrđivanje stanja ažuriranja.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator aplikacije.

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator ažuriranja.

### <a name="guiupdatemanagerqueueinstallforapp"></a>gui.updatemanager.queueinstallforapp

Ovaj događaj označava početak stvarnog instalacijskog procesa za ažuriranje aplikacije. Ovaj događaj predstavlja dio lijevka ažuriranja aplikacije koji upotrebljavamo za utvrđivanje stanja ažuriranja.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator aplikacije.

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator ažuriranja.

### <a name="guiupdatemanagerrelaunchapp"></a>gui.updatemanager.relaunchapp

Ovaj događaj zapisuje jesu li aplikacije uspješno ponovno pokrenute nakon ažuriranja.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator aplikacije.

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **Success** – Vrijednost Booleova niza koja označava je li aplikacija uspješno zatvorena.

- **UpdateID** – Identifikator ažuriranja.

- **UpdateName** – Naziv ažuriranja.

### <a name="installdatacheckrunning"></a>installdata.checkrunning

Ovaj događaj evidentira rezultat provjere između aplikacija za instaliranje i hoće li se postupak instalacije nastaviti na temelju otvaranja aplikacije. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="installdatacleanup"></a>installdata.cleanup

Datoteke paketa treba ukloniti nakon instalacije. Ovaj događaj bilježi slučajeve u kojima ih ne uspijemo ukloniti. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži naziv preuzete datoteke i podatke o pogrešci.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="installedappinvalidbundle"></a>installedapp.invalidbundle

Ovaj događaj upućuje da Microsoftovo automatsko ažuriranje ne može dohvatiti podatke o paketu za registriranu aplikaciju na zadanom putu. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži naziv aplikacije.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="installedappinvalidpreference"></a>installedapp.invalidpreference

Ovaj događaj evidentira slučajeve u kojima osobni odabir korisnika sadrži nevažeći unos aplikacije. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka provjere ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="installedappnilbundleid"></a>installedapp.nilbundleid

Ovaj događaj evidentira slučajeve u kojima nedostaje ID paketa za aplikaciju. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži naziv aplikacije.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="installedappnilbundlename"></a>installedapp.nilbundlename

Ovaj događaj evidentira slučajeve u kojima nedostaje naziv paketa za aplikaciju. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži naziv aplikacije.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="installedappsendcoreappleevent"></a>installedapp.sendcoreappleevent

Ovaj događaj označava da značajka Microsoftovo automatsko ažuriranje (MAU) šalje događaj tvrtke Apple registriranoj aplikaciji za prekid aplikacije radi nastavka s ažuriranjem aplikacije na čekanju. Ovaj događaj trenutačno se upotrebljava kao pomoć za razvoj budućih poboljšanja radi smanjenja prekida korisnika tijekom ažuriranja aplikacije. 

Prikupljaju se sljedeća polja:

- **Acknowledged** – Označava je li dotična aplikacija priznala primanje događaja

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppleEventClass** – Označava vrstu događaja koji se šalje/priznaje

- **AppleEventID** – Jedinstveni identifikator događaja koji se šalje/priznaje

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Sadrži količinu ponovnih pokušaja

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **Success** – Označava je li dotična aplikacija prijavila uspjeh operacije

    
### <a name="installstatuscodesign"></a>installstatus.codesign

Ovaj događaj evidentira status OS binarnog alata za potpisivanje kôda. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja
    
- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="installstatusdaemon"></a>installstatus.daemon

Ovaj događaj evidentira stanje daemona Microsoftova automatskog ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži naznaku postoji li komponenta Daemon na očekivanom mjestu i je li potpisan kôd.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="installstatushelper"></a>installstatus.helper

Ovaj događaj evidentira stanje pomoćnog alata Microsoftova automatskog ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži naznaku postoji li komponenta PrivilegedHelperTool na očekivanom mjestu i je li potpisan kôd.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="installupdatestaskapplaunched"></a>installupdatestask.applaunched

Ovaj događaj znači da je alat Microsoftovo automatsko ažuriranje otkrio pokretanje aplikacije za blokirano ažuriranje, ali nije mogao pronaći odgovarajući instalacijski program. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži naziv pokrenute aplikacije.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="installupdatestaskapplaunchwithpendingupdate"></a>installupdatestask.applaunchwithpendingupdate

Ovaj događaj ukazuje da je alat Microsoftovo automatsko ažuriranje otkrio pokretanje aplikacije za aplikaciju koja čeka na ažuriranje. Pokrenuta će se aplikacija prekinuti. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="installupdatestaskcodesignverificationfail"></a>installupdatestask.codesignverificationfail

Ovaj događaj označava da provjera autentičnosti potpisa koda nije uspjela za ažuriranje aplikacije. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja, naziva ažuriranja i kôda pogreške.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="installupdatestaskcodesignverificationstart"></a>installupdatestask.codesignverificationstart

Ovaj događaj označava da je započela provjera autentičnosti potpisa koda za ažuriranje aplikacije. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja i naziva ažurirane aplikacije.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="installupdatestaskcodesignverificationsuccess"></a>installupdatestask.codesignverificationsuccess

Ovaj događaj označava uspjeh provjere autentičnosti potpisa koda za ažuriranje aplikacije. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja i naziva ažurirane aplikacije.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="installupdatestaskfailsilentinstall"></a>installupdatestask.failsilentinstall

Ovaj događaj evidentira neuspjehe tijekom primjene tihih ažuriranja bez obzira je li u pitanju klonirana ili uobičajena instalacija. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 
    
- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja i vrste ažuriranja.
    
- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="installupdatestaskmultiplerelocatablepackage"></a>installupdatestask.multiplerelocatablepackage

Ovaj događaj znači da je alat Microsoftovo automatsko ažuriranje pronašao više primjera unosa aplikacije za određeni paket ažuriranja u preuzetom manifestu. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja i naziva ažuriranja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="installupdatestaskremoveclone"></a>installupdatestask.removeclone

Ovaj događaj označava da je klon uklonjen. Klon uklanjamo kada je proces instaliranja na klon završen ili kada se pokrene novi postupak i u njemu se nađe starija inačica klonirane verzije. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja, naziva ažuriranja, naziva paketa ažuriranja, detalja o statusu uklanjanja klona / pogreške.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="installupdatestaskretryfail"></a>installupdatestask.retryfail

Ovaj događaj označava da su se pojavile pogreške tijekom postupka ponovnog pokušaja instalacije. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja, naziva ažuriranja i treba li se instalirati putem instalacije na klon

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

   
### <a name="installupdatestaskretryproxyerror"></a>installupdatestask.retryproxyerror

Ovaj događaj evidentira komunikacijske pogreške unutar procesa (komunikacija s pomoćnim alatom MAU). Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja, naziva ažuriranja i detalja o prijavljenoj pogrešci proxy poslužitelja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    

### <a name="installupdatestaskretryresponse"></a>installupdatestask.retryresponse

Ovaj događaj evidentira da pokušaj nije uspio. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja, naziva ažuriranja, verzije aplikacije, naziva paketa ažuriranja i indikacija je li instalacija na klon bila uključena, je li instalacija uspjela i jesu li prijavljene pogreške kod neuspjeha.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="installupdatestaskretrysuccess"></a>installupdatestask.retrysuccess

Ovaj događaj evidentira uspješnu instalaciju ažuriranja nakon ponovnog pokušaja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja, naziva ažuriranja, verzije aplikacije, naziva paketa ažuriranja i indikacija je li instalacija na klon bila uključena.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="installupdatestasksetreopengui"></a>installupdatestask.setreopengui

Ovaj događaj pokazuje je li postavljanje postavke za ponovno otvaranje grafičkog korisničkog sučelja nakon instalacije bilo uspješno. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava uspješnost operacije.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="installupdatestaskupdatestatus"></a>installupdatestask.updatestatus

Ovaj događaj izvješćuje o stanju zadatka instalacije. Ovaj događaj predstavlja dio lijevka ažuriranja i upotrebljava se za utvrđivanje stanja ažuriranja aplikacije.

Prikupljaju se sljedeća polja: 

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Error** – Označava sve pogreške koje su pronađene tijekom postupka ažuriranja ako je popunjen

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **IOC** – Označava je li bila upotrijebljena značajka Instalacija na klon

- **Payload** – Statični tekst koji označava početak postupka instalacije ako postoji

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **Success** – Označava je li postupak instalacije uspješno dovršen

- **UpdateID** – Identifikator za ažuriranje aplikacije

- **UpdateName** – Naziv ažuriranja u obliku koji se prikazuje u preuzetoj datoteci manifesta

- **UpdatePkg** – Naziv paketa ažuriranja koji se primjenjuje

### <a name="lifecyclecomplimentproclaunch"></a>Lifecycle.complimentproclaunch

Ovaj događaj označava pokušaj pokretanja Microsoftovog pomoćnika za ažuriranje iz servisa Microsofta AutoUpdate ili iz servisa Microsofta AutoUpdate putem Microsoftovog pomoćnika za ažuriranje. Taj se događaj koristi za utvrđivanje i osiguravanje radnog stanja servisa Microsoft AutoUpdate i Microsoftovog pomoćnika za ažuriranje.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Error** – sve pogreške prijavljene tijekom pokušaja pokretanja

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **Reason** – razlog pokušaja pokretanja procesa davanja komplimenta

- **SessionId** – identifikator sesije

- **Success** – označava je li pokušaj pokretanja bio uspješan

### <a name="lifecyclelaunch"></a>Lifecycle.launch

Ovaj događaj označava pokretanje servisa Microsoft AutoUpdate ili Microsoftovog pomoćnika za ažuriranje. Taj se događaj koristi i za izvješćivanje o svim problemima utvrđenim tijekom postupka pokretanja te kao način izvješćivanja za pokretanje u slučaju Microsoftovog pomoćnika za ažuriranje.

*[Taj događaj zamjenjuje događaje fba.launch i appdelegate.launch events.]*

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – verzija aplikacije

- **Channel** – preference za publiku

- **Device_NetworkCountry** – država uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Pogreška** – bilo koja pogreška pronađena pri pokretanju

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **LaunchedBy** – metoda koja se koristi za pokretanje Microsoftovog pomoćnika za ažuriranje, ako je primjenjivo

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="lifecycleperiodiccheck"></a>Lifecycle.periodiccheck

Taj događaj povremeno javlja o statusu postupka MicrosoftAutoUpdate. Konkretno, javlja o preostalim zadacima za koje postupak čeka radi završetka Pomoćnika za ažuriranje, a u slučaju korisničkog sučelja javlja je li postupak završio zbog korisničke neaktivnosti.  Ovaj događaj omogućuje nam da odredimo što sprječava Pomoćnik za ažuriranje da dovrši ažuriranja i završi s radom te je li korisničko sučelje prestalo s radom zbog neaktivnosti korisnika.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **dataCollectionDialog** – Booleova vrijednost pokazuje čeka li proces na odgovor korisnika u dijaloškom okviru za prikupljanje podataka

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **forcedUpdateDialog** – Booleova vrijednost pokazuje čeka li proces na odgovor korisnika u dijaloškom okviru za prisilno ažuriranje

- **HowToCheck** – način provjere postavke

- **isBusy** – Booleova vrijednost koja pokazuje je li proces zauzet s aktivnim ažuriranjem

- **isInactive** – Booleova vrijednost koja pokazuje čeka li proces radnju korisnika tijekom dužeg vremena

- **isWaiting** – Booleova vrijednost pokazuje čeka li proces na odgovor korisnika nakon obavijesti

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

- **SessionLength** – trajanje sesije trenutačnog procesa u sekundama


### <a name="lifecycleterminate"></a>Lifecycle.terminate

Ovaj događaj označava isključivanje servisa Microsoft AutoUpdate ili Microsoftovog pomoćnika za ažuriranje. Taj se događaj koristi za utvrđivanje radnog stanja servisa Microsoft AutoUpdate i Microsoftovog pomoćnika za ažuriranje.

*[Taj događaj zamjenjuje događaje fba.terminate i appdelegate.terminate.]*

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **SessionLength** – trajanje sesije trenutačnog procesa u sekundama



### <a name="msupdateclieventhandler"></a>msupdate.cli.eventhandler

Ovaj se događaj upotrebljava za izračun upotrebe raznih vrsta API-ja sučelja naredbenog retka značajke Microsoftovo automatsko ažuriranje (MAU).

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – identifikator aplikacije koja šalje API sučelja naredbenog retka MAU-u.

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **EventType** – vrsta događaja koji aplikacija šalje MAU-ovom API-ju sučelja naredbenog retka.

- **HowTocheck** – Postavka za provjeru ažuriranja

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="msupdateclieventhandlerapplyupdatesappids"></a>msupdate.cli.eventhandler.applyupdates.appids

Ovaj događaj označava da je za primjenu ažuriranja izdana naredba CLI (sučelje retka klijenta). Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži popis ID-ova aplikacija koje treba ažurirati.
    
- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="msupdateclieventhandlerconfig"></a>msupdate.cli.eventhandler.config

Ovaj događaj označava da je modul sučelja naredbenog retka Microsoftova automatskog ažuriranja primio Apple događaj koji treba konfigurirati. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="msupdateclieventhandlerupdates"></a>msupdate.cli.eventhandler.updates

Ovaj događaj označava da je modul sučelja naredbenog retka Microsoftova automatskog ažuriranja primio Apple događaj za popis ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="msupdatemonitorprogressdownloaded"></a>msupdate.monitor.progress.downloaded

Ovaj događaj ukazuje da su ažuriranja preuzeta. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži popis preuzetih ažuriranja

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="msupdatemonitorprogressfailure"></a>msupdate.monitor.progress.failure

Ovaj događaj evidentira popis ažuriranja u redu čekanja koje nisu uspješno primijenjena. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži popis ažuriranja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="msupdatemonitorprogressfinished"></a>msupdate.monitor.progress.finished

Ovaj događaj evidentira popis ažuriranja u redu čekanja koja su uspješno instalirana. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži popis ažuriranja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="msupdatemonitorprogressqueued"></a>msupdate.monitor.progress.queued

Ovaj događaj evidentira popis ažuriranja u redu čekanja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži popis ažuriranja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="optinnotificationaction"></a>Optinnotificationaction

Ovaj događaj evidentira odgovor korisnika na uključivanje dijaloškog okvira za ulazak u tiha ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži statični tekst koji predstavlja odabir korisnika za uključivanje u automatsko preuzimanje i instalaciju.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="sauforcedupdateautodismiss"></a>sauforcedupdate.autodismiss

Ovaj događaj označava da se prikazani dijaloški okvir za prisilno ažuriranje odbacuje zbog neaktivnosti korisnika. Ovim se događajem utvrđuje količina prisilnih ažuriranja koja se provode bez ikakve reakcije korisnika u vezi s prikazanom obaviješću. Ovim se događajem poboljšava korisničko sučelje za smanjenje prekida.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja
  
- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="sauforcedupdateclose"></a>sauforcedupdate.close

Ovaj događaj označava da je korisnik odabrao zatvaranje dijaloškog okvira prisilnog ažuriranja. Ovaj se događaj upotrebljava za određivanje količine prisilnih ažuriranja koja se odgađaju radnjom korisnika. Ovim se događajem poboljšava korisničko sučelje za smanjenje prekida. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="sauforcedupdatecompleteautodismiss"></a>sauforcedupdate.completeautodismiss

Ovaj događaj označava da se prikazani dijaloški okvir za prisilno ažuriranje iz značajke roka za dovršetak odbacuje zbog neaktivnosti korisnika. Ovim se događajem utvrđuje količina prisilnih ažuriranja koja se provode bez ikakve reakcije korisnika u vezi s prikazanom obaviješću. Ovim se događajem poboljšava korisničko sučelje za smanjenje prekida za značajku roka za dovršetak.

Prikupljaju se sljedeća polja: 

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="sauforcedupdatecompleteclose"></a>sauforcedupdate.completeclose

Ovaj događaj označava uspješno dovršavanje prisilnog ažuriranja. Ovim se događajem utvrđuje stanje značajke prisilnog ažuriranja. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="sauforcedupdatedisplay"></a>sauforcedupdate.display

Ovaj događaj označava da je dijaloški okvir za prisilno ažuriranje bio prikazan.  Ovaj događaj predstavlja dio lijevka za prisilno ažuriranje i upotrebljava se za utvrđivanje zdravlja značajke prisilnog ažuriranja.

Prikupljaju se sljedeća polja: 

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="sauforcedupdatedisplayfinalhour"></a>sauforcedupdate.displayfinalhour

Ovaj događaj označava da je dijaloški okvir za prisilno ažuriranje za zadnji sat bio prikazan. Ovaj događaj predstavlja dio lijevka za prisilno ažuriranje i upotrebljava se za utvrđivanje zdravlja značajke prisilnog ažuriranja.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="sauforcedupdatedone"></a>sauforcedupdate.done

Ovaj događaj označava da je prisilno ažuriranje uspješno dovršeno. Ovaj događaj predstavlja dio lijevka za prisilno ažuriranje i upotrebljava se za utvrđivanje zdravlja značajke prisilnog ažuriranja. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="sauforcedupdateenabled"></a>sauforcedupdate.enabled

Ovaj se događaj aktivira kada Microsoftovo automatsko ažuriranje (MAU) utvrdi da je prisilno ažuriranje primjenjivo.  Taj se događaj upotrebljava za utvrđivanje stanja značajke prisilnog ažuriranja. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Enabled** – Označava je li prisilno ažuriranje omogućeno

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **InvalidUpdates** – Količina prisilnih ažuriranja koja su postavljena s nevažećim verzijama ažuriranja

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="sauforcedupdateforcedupdatedismiss"></a>sauforcedupdate.forcedupdatedismiss

Ovaj događaj označava da se prikazani dijaloški okvir za prisilno ažuriranje za zadnji sat odbacuje zbog neaktivnosti korisnika. Ovim se događajem utvrđuje količina prisilnih ažuriranja koja se provode bez ikakve reakcije korisnika u vezi s prikazanom obaviješću. Ovim se događajem poboljšava korisničko sučelje za smanjenje prekida. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="sauforcedupdateforcequitandupdatenow"></a>sauforcedupdate.forcequitandupdatenow

Ovaj događaj označava početak prisilnog ažuriranja koje je pokrenuo korisnik. Ovaj događaj tvori dio lijevka i upotrebljava se za utvrđivanje stanja značajke prisilnog ažuriranja. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije 

### <a name="sauforcedupdateforceterminate"></a>sauforcedupdate.forceterminate

Ovaj događaj označava početak prisilnog ažuriranja uz prisilno završavanje aplikacije.  Ovaj događaj tvori dio lijevka i upotrebljava se za utvrđivanje stanja značajke prisilnog ažuriranja.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Sadrži broj aplikacija koje će se prekinuti

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="sauforcedupdatequitandupdatenow"></a>sauforcedupdate.quitandupdatenow

Ovaj događaj označava da je korisnik odabrao zatvaranje aplikacije i primjenu ažuriranja. Ovaj događaj predstavlja dio lijevka i upotrebljava se za utvrđivanje zdravlja značajke prisilnog ažuriranja. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="sauforcedupdatesnooze"></a>sauforcedupdate.snooze

Ovaj događaj označava da je korisnik odabrao odgodu prisilnog ažuriranja. Ovaj događaj tvori dio lijevka i upotrebljava se za utvrđivanje stanja značajke prisilnog ažuriranja. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="sauforcedupdateterminate"></a>sauforcedupdate.terminate

Ovaj događaj označava početak prisilnog ažuriranja uz završavanje aplikacije. Ovaj događaj tvori dio lijevka i upotrebljava se za utvrđivanje stanja značajke prisilnog ažuriranja.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Sadrži broj aplikacija koje će se prekinuti

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="sauforcedupdateupdatenow"></a>sauforcedupdate.updatenow

Ovaj događaj označava da je korisnik odabrao ažurirati aplikaciju sada.  Ovaj događaj tvori dio lijevka i upotrebljava se za utvrđivanje stanja značajke prisilnog ažuriranja.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="sauupdateinfoprovider"></a>sauupdateinfoprovider

Ovaj događaj evidentira kad god nedostaje ključ manifesta elementa osiguranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži niz koji se koristi za traženje lokacije ili veličine ažuriranja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="updateapplaunchdetected"></a>update.applaunchdetected

Ovaj događaj označava da je aplikacija bila pokrenuta dok je ažuriranje bilo u tijeku. Ovim se događajem utvrđuje količina aplikacija koje se pokreću tijekom ažuriranja i upotrebljava se za poboljšavanje korisničkog iskustva u budućim izdanjima.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **Success** – Označava je li pokrenuta aplikacija uspješno završena

- **UpdateID** – Identifikator za ažuriranje aplikacije

### <a name="updateappterminationreceived"></a>update.appterminationreceived

Ovaj događaj označava da je aplikacija s blokiranim ažuriranjem završena te može li Microsoftovo automatsko ažuriranje (MAU) nastaviti s ažuriranjem. Ovaj događaj predstavlja dio lijevka i upotrebljava se za utvrđivanje stanja ažuriranja aplikacije.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Error** – Označava postoje li druge instance aplikacije koje su i dalje pokrenute, čime se sprječava nastavak rada MAU-a

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst koji označava da MAU nastavlja s ažuriranjem

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator za ažuriranje aplikacije

### <a name="updateblockedappclosed"></a>update.blockedappclosed

Ovaj događaj označava da je Microsoftovo automatsko ažuriranje (MAU) prepoznalo da je aplikacija s blokiranim ažuriranjem zatvorena i da je moguće nastaviti s ažuriranjem. Ovaj događaj predstavlja dio lijevka i upotrebljava se za utvrđivanje stanja ažuriranja aplikacije. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije.

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje.

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja. 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator za ažuriranje aplikacije

### <a name="updateblockedinstallskip"></a>update.blockedinstallskip

Ovaj događaj zapisuje pogrešku koja se pojavila tijekom pokušaja preskakanja ažuriranja aplikacije. Ovaj je događaj ključan i upotrebljava se za istragu prijavljenih pogrešaka.  

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Sadrži informacije o pogreškama koje se pojavljuju

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="updateclientsession"></a>update.clientsession

Ovaj se događaj prijavljuje kada se promijeni status korisničkog uređaja, zbog čega dolazi do pauziranja Microsoftova pomoćnika za ažuriranje ili nastavka postupka ažuriranja. Ovaj događaj predstavlja dio lijevka i upotrebljava se za utvrđivanje stanja ažuriranja aplikacije. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Označava pauziranje ili nastavak Microsoftova automatskog ažuriranja (MAU)

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="updatedownloadbegin"></a>update.download.begin 

Ovaj događaj označava početak postupka ažuriranja aplikacije. Ovaj događaj predstavlja dio lijevka ažuriranja i upotrebljava se za utvrđivanje stanja ažuriranja aplikacije. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **IsRepair** – Označava je li ažuriranje namijenjeno za popravak neuspješna ažuriranja

- **Payload** – Označava je li prethodno bilo pokušano preuzimanje

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateName** – Naziv ažuriranja u obliku koji se prikazuje u preuzetoj datoteci manifesta

### <a name="updatedownloadfinish"></a>update.download.finish

Ovaj događaj označava dovršavanje faze preuzimanja za ažuriranje aplikacije. Ovaj događaj predstavlja dio lijevka ažuriranja i upotrebljava se za utvrđivanje stanja ažuriranja aplikacije.  

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **IsRepair** – Označava je li ažuriranje namijenjeno za popravak neuspješna ažuriranja

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator za ažuriranje aplikacije

- **UpdateName** – Naziv ažuriranja u obliku koji se prikazuje u preuzetoj datoteci manifesta

### <a name="updatedownloadresume"></a>update.downloadresume

Ovaj događaj izvješćuje o pogrešci koja je pronađena tijekom pokušaja nastavka pauziranog zadatka preuzimanja. Ovaj je događaj ključan i upotrebljava se za istragu prijavljenih pogrešaka. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Error** – Označava vrstu pogreške koja se pojavljuje

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator za ažuriranje aplikacije

### <a name="updateerror"></a>update.error

Ovaj događaj izvješćuje o pogrešci koja je pronađena tijekom pokušaja ažuriranja registrirane aplikacije.  Ovaj je događaj ključan i upotrebljava se za istragu prijavljenih pogrešaka. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Error** – Sadrži informacije o vrsti pogreške koja se pojavljuje

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Sadrži informacije o vrsti pogreške koja se pojavljuje

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="updateinstallcleanupforapp"></a>update.installcleanupforapp

Ovaj događaj označava da je instalacija ažuriranja dovršena i da Microsoftovo automatsko ažuriranje (MAU) provodi čišćenje.  Ovaj događaj predstavlja dio lijevka ažuriranja i upotrebljava se za utvrđivanje stanja ažuriranja aplikacije.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppState** – Stanje registrirane aplikacije. Može označavati pogrešku, popravak na čekanju itd.

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator za ažuriranje aplikacije

### <a name="updateinstallupdateforapp"></a>update.installupdateforapp

Ovaj se događaj upotrebljava za izvješćivanje o početku postupka instalacije ažuriranja aplikacije. Ovaj događaj predstavlja dio lijevka ažuriranja i upotrebljava se za utvrđivanje stanja ažuriranja aplikacije. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Error** – Pronađene pogreške ako postoje

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator za ažuriranje aplikacije

- **UpdateName** – Naziv ažuriranja u obliku koji se prikazuje u preuzetoj datoteci manifesta

### <a name="updateinstallupdateforappsuccess"></a>update.installupdateforapp.success

Ovaj događaj izvješćuje o stanju zadatka instalacije. Ovaj događaj predstavlja dio lijevka ažuriranja i upotrebljava se za utvrđivanje stanja ažuriranja aplikacije. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Označava je li tijekom postupka instalacije prikazan prikaz napretka

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **Success** – Oznaka o uspjehu koju vraća zadatak instalacije

- **UpdateID** – Identifikator za ažuriranje aplikacije

### <a name="updateinstallvariance"></a>Update.InstallVariance

Ovaj se događaj upotrebljava za izračun metrike stanja za MAU. Ovaj nam događaj omogućuje utvrđivanje uspjeha metrike za instalaciju prioritetne značajke i provjeru cjelovitosti značajke.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži popis ID-ova aplikacije i njihov povezani prioritet instalacije prikazan u brojevima.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="updatemultipleappupdates"></a>update.multipleappupdates 

Ovaj događaj označava da je u pozadini u tijeku više ažuriranja aplikacija. Ovaj događaj predstavlja dio lijevka ažuriranja i upotrebljava se za utvrđivanje stanja ažuriranja aplikacije.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja 

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Sadrži informacije o broju aplikacija koje se ažuriraju

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="updatepreviousidnil"></a>update.previousidnil

Ovaj događaj označava da se preuzima paket ažuriranja popravka, no ne postoje prethodne informacije o preuzimanju. Ovaj je događaj ključan i upotrebljava se za istragu prijavljenih pogrešaka. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Error** – Označava vrstu pogreške koja se pojavljuje

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="updatequeueinstallforapp"></a>update.queueinstallforapp 

Ovaj događaj označava da je preuzeti paket ažuriranja uvršten u red čekanja za instalaciju.  Ovaj događaj predstavlja dio lijevka ažuriranja i upotrebljava se za utvrđivanje stanja ažuriranja aplikacije.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst koji označava da se aplikacija mora zatvoriti ako postoji

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator za ažuriranje aplikacije

- **UpdateName** – Naziv ažuriranja u obliku koji se prikazuje u preuzetoj datoteci manifesta

### <a name="updaterelaunchafterupdate"></a>update.relaunchafterupdate 

Ovaj događaj označava da je ažuriranje aplikacije dovršeno i da se ona ponovno pokreće. Ovaj događaj predstavlja dio lijevka ažuriranja i upotrebljava se za utvrđivanje stanja ažuriranja aplikacije. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Error** – Sadrži informacije o svim pogreškama koje su pronađene tijekom pokušaja ponovnog pokretanja aplikacije

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **UpdateID** – Identifikator za ažuriranje aplikacije

### <a name="updatetimerforapptermination"></a>update.timerforapptermination 

Ovaj događaj označava početak/kraj brojača za provjeru statusa aplikacije. Ovaj se događaj pojavljuje u paru i upotrebljava za utvrđivanje jesu li svi objekti brojača uklonjeni tijekom nastavka postupka ažuriranja aplikacije.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Označava je li brojač bio dodan ili uklonjen

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="updatecoreappregistration"></a>updatecore.appregistration

Ovaj događaj evidentira pokušaje registracije aplikacije i rezultat/razlog. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži identifikator koji se koristi za praćenje aktivnosti ažuriranja, naznaka je li prednost dostupna, je li riječ o ponovnoj registraciji i je li registracija potrebna.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="updatecoreloadinglaunchagent"></a>updatecore.loadinglaunchagent

Ovaj događaj označava da se agent za pokretanje učitava. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="updatecorerunnstaskcommand"></a>updatecore.runnstaskcommand

Ovaj događaj izvješćuje o pogrešci tijekom pokušaja pokretanja zadatka. Ovaj je događaj ključan i upotrebljava se za istragu prijavljenih pogrešaka.  

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Sadrži put do naredbe koja se izvršava

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="updatecoreserverconnectionfail"></a>updatecore.server.connectionfail

Ovaj događaj evidentira pogreške na koje se naišlo na putu do poslužitelja CDN. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži podatke o nazivu poslužitelja i je li poslužitelj valjan i dostupan.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="updatecoreservernullurl"></a>updatecore.server.nullurl

Ovaj događaj izvješćuje o pogrešci koja označava da se određeni poslužitelj nije mogao doseći. Ovim se događajem utvrđuje stopa neuspjeha ažuriranja koju je uzrokovao mrežni problem. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="updatefilterhelpercannotretrievebuilddate"></a>updatefilterhelper.cannotretrievebuilddate

Ažuriranja putem usluge MAU možemo filtrirati samo ako ažuriranje koje se nudi nije starije od određenog broja dana. Ovdje evidentiramo kako nismo mogli dohvatiti datum iz metapodataka aplikacije. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži ID aplikacije.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="updatefilterhelperinvalidappid"></a>updatefilterhelper.invalidappid

Ovaj događaj izvješćuje o pogrešci koja ukazuje na to da nije bilo moguće pronaći odgovarajuće datoteke manifesta s pomoću ID-a aplikacije dohvaćenog iz web-odgovora. Ovaj se upotrebljava za istragu prijavljenih pogrešaka.

Prikupljaju se sljedeća polja: 

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Sadrži ID aplikacije u web-odgovoru

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="updatefilterhelperinvalidappidfromwebservices"></a>updatefilterhelper.invalidappidfromwebservices

Ovaj događaj izvješćuje o pogrešci koja ukazuje na to da ID aplikacije dohvaćen iz web-odgovora nije u očekivanom formatu. Ovaj se upotrebljava za istragu prijavljenih pogrešaka.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Statični tekst

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="updatefilterhelperinvalidresponsefromupdatefiltering"></a>updatefilterhelper.invalidresponsefromupdatefiltering

Ažuriranja putem usluge MAU možemo filtrirati samo ako ažuriranje koje se nudi nije starije od određenog broja dana. Ovdje evidentiramo da iz metapodataka aplikacije nedostaje datum. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 
    
- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži ID aplikacije.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="updatefilterhelpermissingbuilddate"></a>updatefilterhelper.missingbuilddate

Ažuriranja putem usluge MAU možemo filtrirati samo ako ažuriranje koje se nudi nije starije od određenog broja dana. Ovdje evidentiramo da iz metapodataka aplikacije nedostaje datum. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži ID aplikacije.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="updatefilterhelperupdatebypassedoldage"></a>updatefilterhelper.updatebypassedoldage

Ažuriranja putem usluge MAU možemo filtrirati samo ako ažuriranje koje se nudi nije starije od određenog broja dana. Ovdje evidentiramo da je usluga zaobiđena zbog starog datuma ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži ID aplikacije.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="updatefindercheckerror"></a>updatefinder.check.error

Ovaj događaj izvješćuje o pogrešci koja je pronađena tijekom traženja ažuriranja. Ovaj je događaj ključan i upotrebljava se za istragu prijavljene pogreške. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Code** – Kôd pogreške 

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Domain** – Domena pogreške

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

 
### <a name="updatefindercheckstart"></a>updatefinder.check.start

Ovaj događaj evidentira svaki put kada pokrenemo operaciju provjere ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja
    
- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži podatke o ponuđenim ažuriranjima, registriranim aplikacijama i privremenom mjestu gdje će preuzete datoteke biti spremljene.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="updatefindercheckstatus"></a>updatefinder.check.status

Ovaj događaj objedinjuje status provjere za operacije ažuriranja (kanal od pretraživanja do preuzimanja). Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži podatke o ponuđenim ažuriranjima, registriranim aplikacijama i privremenom mjestu gdje će preuzete datoteke biti spremljene.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="updatefindercheckupdatefound"></a>updatefinder.check.updatefound

Evidentiramo kad god provjera ažuriranja rezultira pronađenim ažuriranjima. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="updatefindercheckupdatenotfound"></a>updatefinder.check.updatenotfound

Evidentiramo kad god provjera ažuriranja rezultira time da nema ažuriranja jer nije pronađeno nijedno ažuriranje. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="updatefindercheckuptodate"></a>updatefinder.check.uptodate

Evidentiramo kad god provjera ažuriranja rezultira time da nema ponuđenih ažuriranja jer su sve aplikacije već ažurne. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="updatefinderofferupdatesinvalidappid"></a>updatefinder.offerupdates.invalidappid

Ovaj događaj izvješćuje o pogrešci tijekom pokušaja procjene je li određeno ažuriranje primjenjivo. Ovaj je događaj ključan i upotrebljava se za istragu prijavljene pogreške.  

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **CatalogID** – Identifikator kataloga kojem se pristupa

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **IsNullID** – Označava je li ID nula

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="updatefinderofferupdatesminoscheckfail"></a>updatefinder.offerupdates.minoscheckfail

Evidentiramo kad god smo blokirali ažuriranje zbog neispunjavanja preduvjeta OS-a. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži minimalne preduvjete verzije OS-a kako je navedeno u preuzetoj datoteci manifesta.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="updatefinderofferupdatesmissingtrigger"></a>updatefinder.offerupdates.missingtrigger

Ovaj događaj izvješćuje o pogrešci tijekom pokušaja procjene okidača od preuzetog manifesta za ažuriranje aplikacije. On je ključan i upotrebljava se za istragu prijavljene pogreške.  

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **TriggerKey** – Ključ okidača koji je pronađen u manifestu

- **Triggers** – Rječnik okidača pronađenih u manifestu

### <a name="updatefinderofferupdatesnullbundleforappid"></a>updatefinder.offerupdates.nullbundleforappid

Ovaj događaj znači da alat Microsoftovo automatsko ažuriranje nije uspio učitati informacije o paketu za ID aplikacije navedene u preuzetoj datoteci manifesta. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži ID aplikacije.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="updatefinderofferupdatesupdaterulematched"></a>updatefinder.offerupdates.updaterulematched

Ovaj događaj označava da je pronađeno ažuriranje za aplikaciju i osnovnu verziju. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži ID aplikacije i podatke o verziji paketa.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="updatefinderregisteredapps"></a>updatefinder.registeredapps

Evidentiramo aplikacije koje instalira/registrira/kontrolira MAU. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži ID aplikacije i podatke o verziji paketa.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="updatefindersuiteinvalidsuiteversion"></a>updatefinder.suite.invalidsuiteversion

Ovaj događaj izvješćuje o pogrešci verzije paketa tijekom procjene je li određeno ažuriranje primjenjivo. Ovaj je događaj ključan i upotrebljava se za istragu prijavljene pogreške.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **Suite** – Naziv paketa koji se razmatra

### <a name="updatefindersuitekeyvaluemissing"></a>updatefinder.suite.keyvaluemissing

Ovaj događaj izvješćuje o pogrešci tijekom pokušaja dodavanja aplikacije paketu. Ovaj je događaj ključan i upotrebljava se za istragu prijavljene pogreške.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije 

- **Suite** – Potrebno je dodati naziv aplikacije paketa

    
### <a name="updatefindersuitemissingcollateral"></a>updatefinder.suite.missingcollateral

Ažuriranje paketa – evidentiramo svaki put kada ažuriranje paketa nije primjenjivo zbog nedostatka elementa osiguranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Tekst koji označava prirodu događaja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="updatefindersuitestaleversion"></a>updatefinder.suite.staleversion

Ažuriranje paketa – evidentiramo svaki put kada ažuriranje paketa nije primjenjivo jer je osnovna verzija prestara. Evidentiramo osnovnu verziju i ID aplikacije paketa. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži naziv paketa.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="updatefindersuiteupdateapplicable"></a>updatefinder.suite.updateapplicable

Ažuriranje paketa – evidentiramo svaki put kada je ažuriranje paketa primjenjivo. Evidentiramo osnovnu verziju i ID aplikacije paketa. Evidentiramo osnovnu verziju i ID aplikacije paketa. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži naziv, osnovnu verziju i ažuriranu verziju paketa.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="updatefindersuiteupdatenotapplicabledefaultpath"></a>updatefinder.suite.updatenotapplicabledefaultpath

Ažuriranje paketa – evidentiramo svaki put kada ažuriranje paketa nije ponuđeno jer nisu sve aplikacije paketa instalirane na temelju zadanog puta. Evidentiramo osnovnu verziju i ID aplikacije paketa. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži naziv, osnovnu verziju i ažuriranu verziju paketa.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="updatefindersuiteupdatenotapplicableversion"></a>updatefinder.suite.updatenotapplicableversion

Ažuriranje paketa – evidentiramo svaki put kada ažuriranje paketa nije ponuđeno jer nisu sve aplikacije paketa u istoj osnovnoj verziji. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži naziv, osnovnu verziju i ažuriranu verziju paketa.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="updatefindersuiteupdatenotoffered"></a>updatefinder.suite.updatenotoffered

Ažuriranje paketa – evidentiramo svaki put kada ažuriranje paketa nije ponuđeno jer je veličina paketa veća od pojedinačnih ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži naziv paketa.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="updatefindersuiteupdateoffered"></a>updatefinder.suite.updateoffered

Ažuriranje paketa – evidentiramo svaki put kada je ažuriranje paketa ponuđeno. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži naziv, osnovnu verziju i ažuriranu verziju paketa.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="updatemanagercheckupdate"></a>updatemanager.checkupdate

Ovaj događaj evidentira broj ažuriranja koje je pronašao alat Microsoftovo automatsko ažuriranje tijekom provjere dostupnih ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži broj pronađenih dostupnih ažuriranja.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="updatemanagerupdatespending"></a>updatemanager.updatespending

Ovaj događaj označava da su pronađena ažuriranja i da čekaju instalaciju. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži indikaciju je li se zadatak izvodi na glavnoj niti i broju ažuriranja na čekanju.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="updatestatuscodesign"></a>UpdateStatus.Codesign

Ovaj događaj izvješćuje o stanju potvrde suoblikovanja koje Microsoftov pomoćnik za ažuriranje pokreće nakon instalacije ažuriranja klijentskih aplikacija. Ovim događajem osiguravamo da pružamo pakete koji su valjani i nadogradit ćemo instaliranu aplikaciju na najnoviju verziju.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppID** – Identifikator za aplikaciju koja se ažurira

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Error** – Sve pogreške koje su pronađene tijekom postupka potvrde suoblikovanja

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

- **Success** – Označava je li potvrda suoblikovanja bila uspješna

- **UpdateID** – Jedinstveno prepoznaje primijenjeno ažuriranje 

- **UpdateName** – Naziv ažuriranja kao što je opisano u manifestu ažuriranja

- **UpdatePkg** – Naziv paketa ažuriranja koji je primijenjen

### <a name="urlutilitiesgetmauinfo"></a>urlutilities.getmauinfo

Ovaj događaj izvješćuje o pogrešci koja se pojavljuje tijekom pristupa paketu aplikacije Microsoftovo automatsko ažuriranje (MAU). Ovaj je događaj ključan i upotrebljava se za istragu prijavljene pogreške.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Sadrži informacije o pogreškama koje se pojavljuju

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije
   
### <a name="webservicescheckforsilentupdates"></a>webservices.checkforsilentupdates

Ovaj događaj označava da su pronađeni kandidati za tiho ažuriranje. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži broj pronađenih ažuriranja i ID aplikacije.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="webservicesdeltaupdater"></a>webservices.deltaupdater

Ovaj događaj evidentira interakciju između klijentskog kôda i značajki koja kontrolira hoće li klijent omogućiti Delta ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži odgovor web-servisa i vrste ažuriranja koje se primjenjuje.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="webservicesserviceaction"></a>webservices.serviceaction

Evidentiramo bilo kakve pogreške koje nastaju uslijed neočekivanog odgovora web-servisa. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži detalje o prosljeđivanju akcije s web-servisa.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije


### <a name="webservicesserviceresponse"></a>webservices.serviceresponse

Ovaj događaj evidentira zahtjeve za uslugu MAU službu, vrijeme odgovora i pogreške. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži ID zahtjeva, naziv aplikacije, vrijeme odgovora i/ili kod statusa.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

    
### <a name="webservicessilentupdate"></a>webservices.silentupdate

Evidentiramo zahtjeve kako bismo provjerili postoje li pravila primjenjivosti za "prisilno ažuriranje", npr. moramo prebaciti korisnika iz verzije N na verziju N+1 zbog nekog velikog problema. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži ID zahtjeva, naziv aplikacije, vrijeme odgovora i/ili kod statusa.

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="webservicesupdatefiltering"></a>webservices.updatefiltering

Ovaj događaj označava provedeno filtriranje na popisu primjenjivih ažuriranja putem web-usluga. Ovaj događaj upotrebljavamo da bismo osigurali da blokiranja aplikacije pravilno funkcioniraju ako moramo blokirati ažuriranje.

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppversionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Sadrži informacije o broju ažuriranja blokiranih putem web-usluga

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="webserviceswebcontent"></a>webservices.webcontent

Evidentiramo zahtjeve i odgovore primljene u web-servis. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije za slanje događaja

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowTocheck** – Postavka za provjeru ažuriranja

- **Payload** – Sadrži ID pozivatelja web-servisa

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva 3 okteta IP adrese

- **SessionId** – Identifikator sesije

### <a name="webserviceswhatsnew"></a>webservices.whatsnew

Ovaj se događaj aktivira kada Microsoftovo automatsko ažuriranje (MAU) provodi upit za web-usluge u značajci „Što je novo” za registrirane aplikacije. Ovim se događajem utvrđuje stanje značajke „Što je novo”. 

Prikupljaju se sljedeća polja:

- **App** – Proces aplikacije koji šalje događaj

- **AppInfo_Language** – Jezik pod kojim se aplikacija izvodi

- **AppVersionLong** – Verzija aplikacije

- **Channel** – Preference za publiku

- **Device_NetworkCountry** – Zemlja uređaja (na temelju IP adrese)

- **DeviceID** – Identifikator uređaja

- **DeviceInfo_Model** – Hardverski model uređaja

- **DeviceInfo_NetworkType** – Vrsta mreže (Wi-Fi, ožičena, nepoznata)

- **DeviceInfo_OsBuild** – Verzija operacijskog sustava

- **Event_ReceivedTime** – Vrijeme primanja telemetrije

- **EventInfo_Name** – Naziv telemetrijskog događaja koji se zapisuje

- **EventInfo_Time** – Vrijeme odvijanja zapisanog događaja 

- **HowToCheck** – Način provjere postavke

- **Payload** – Sadrži informacije o broju aplikacija s informacijama o tome što je novo

- **PipelineInfo_ClientCountry** – Zemlja uređaja (na temelju IP adrese)

- **PipelineInfo_ClientIp** – Prva tri okteta IP adrese

- **SessionId** – Identifikator sesije

## <a name="onenote-sync-events"></a>Sinkronizacija događaja u programu OneNote

### <a name="officeonenotestoragenotebooksyncresult"></a>Office.OneNote.Storage.NotebookSyncResult
 
Ovaj događaj zapisuje rezultat sinkronizacije bilježnice. Koristi se za otkrivanje broja jedinstvenih ciljeva sinkronizacije tijekom izračuna rezultata sinkronizacije aplikacije OneNote.
 
Prikupljaju se sljedeća polja

- **CachedError_Code** – numerirani ili alfanumerički kod koji se koristi za određivanje prirode predmemorirane pogreške i/ili razloga pojave

- **CachedError_Description** – opis predmemorirane pogreške

- **CachedError_Tag** – označava mjesto na kojem se predmemorirana pogreška prikazuje u kodu

- **CachedError_Type** – vrsta predmemorirane pogreške, npr. Win32Error itd.

- **ExecutionTime** – vrijeme u milisekundama potrebno za repliciranje bilježnice

- **Gosid** – globalni ID prostora objekta

- **IdentityType** – vrsta identiteta, npr. Windows Live, Org ID itd.

- **InitialReplicationInSession** – označava je li ova replikacija prva replikacija bilježnice nakon otvaranja ili nije

- **IsBackgroundSync** – označava je li ovo sinkronizacija u pozadini ili nije

- **IsCachedErrorSuppressed** – označava je li predmemorirana pogreška potisnuta ili nije

- **IsCachedErrorUnexpected** – označava je li predmemorirana pogreška neočekivana ili nije

- **IsNotebookErrorSuppressed** – označava je li pogreška sinkronizacije na razini bilježnice potisnuta ili nije

- **IsNotebookErrorUnexpected** – označava je li pogreška sinkronizacije na razini bilježnice neočekivana ili nije

- **IsSectionErrorSuppressed** – označava je li pogreška sinkronizacije odjeljka potisnuta ili nije

- **IsSectionErrorUnexpected** – označava je li pogreška sinkronizacije odjeljka neočekivana ili nije

- **IsUsingRealtimeSync** – označava koristi li sinkronizacija bilježnice suvremenu sinkronizaciju sadržaja stranice ili ne

- **LastAttemptedSync** – vremenska oznaka za trenutak kada se proveo posljednji pokušaj sinkronizacije bilježnice

- **LastBackgroundSync** – vremenska oznaka za trenutak kada se proveo posljednji pokušaj sinkronizacije u pozadini

- **LastNotebookViewedDate** – datum kada je bilježnica posljednji put prikazana

- **LastSuccessfulSync** – vremenska oznaka za trenutak kada se bilježnica uspješno prethodno sinkronizirala

- **NeedToRestartBecauseOfInconsistencies** – treba li se sinkronizacija ponovno pokrenuti zbog nedosljednosti ili ne

- **NotebookErrorCode** – kod pogreške sinkronizacije na razini bilježnice spremljen je na prostoru grafikona bilježnice

- **NotebookId** – ID bilježnice

- **NotebookType** – vrsta bilježnice

- **ReplicatingAgainBecauseOfInconsistencies** – pokreće li se sinkronizacija ponovno zbog nedosljednosti ili ne

- **SectionError_Code** – numerirani ili alfanumerički kod koji se koristi za određivanje prirode pogreške sinkronizacije odjeljka i/ili razloga pojave

- **SectionError_Description** – opis pogreške sinkronizacije odjeljka

- **SectionError_Tag** – označava mjesto na kojem se pogreška sinkronizacije odjeljka prikazuje u kodu

- **SectionError_Type** – vrsta pogreške sinkronizacije odjeljka, npr. Win32Error itd.

- **Success** – je li bilježnica uspješno sinkronizirana ili nije

- **SyncDestinationType** – vrsta odredišta sinkronizacije, npr. OneDrive ili SharePoint Online

- **SyncId** – broj jedinstven svakoj sinkronizaciji bilježnice

- **SyncWasFirstInSession** – označava je li ova sinkronizacija prva sinkronizacija u trenutnoj sesiji

- **SyncWasUserInitiated** – označava je li korisnik sinkronizacije pokrenut ili nije

- **TenantId** – ID klijenta sustava SharePoint

- **TimeSinceLastAttemptedSync** – vrijeme proteklo od posljednjeg pokušaja sinkronizacije bilježnice

- **TimeSinceLastSuccessfulSync** – vrijeme proteklo od posljednje uspješne sinkronizacije bilježnice

### <a name="officeonenotestoragerealtimewebsocketsessioninfo"></a>Office.OneNote.Storage.RealTime.WebSocketSessionInfo
 
Ovaj događaj evidentira rezultat sinkronizacije web-utičnice za obje sinkronizacije aplikacije OneNote: suvremenu sinkronizaciju sadržaja stranice i suvremenu sinkronizaciju hijerarhije. Koristi se za otkrivanje broja jedinstvenih ciljeva sinkronizacije tijekom izračuna rezultata sinkronizacije aplikacije OneNote. Također se koristi za suvremenu sinkronizaciju performansi nadzorne ploče u aplikaciji OneNote.
 
Prikupljaju se sljedeća polja:
 
- **CloseReason** – Razlog zatvaranja web-utičnice, npr. neuobičajeno zatvaranje, itd.

- **DataIsFreshCount** – broj uspješnih zahtjeva za reviziju koda u sesiji web-utičnice

- **DeviceSessionId** – ID sesije uređaja

- **DownloadCount** – broj preuzimanja u sesiji web-utičnice

- **Error** – u osnovi je Exception_Type + Exception_Description + Exception_Code + Exception_Tag

- **Exception_Code** – numerirani ili alfanumerički kod koji se koristi za određivanje prirode pogreške i/ili razloga pojave

- **Exception_Description** – opis pogreške

- **Exception_Tag** – označava mjesto na kojem se pogreška prikazuje u kodu

- **Exception_Type** – vrsta pogreške, npr. Win32Error itd.

- **FirstUpdateSize** – prva duljina ažuriranja poruke

- **HasError** – postoji li pogreška tijekom sesije web-utičnice 

- **IsEducationNotebook** – označava je li trenutna bilježnica obrazovna bilježnica ili nije

- **IsHierarchyResource** – označava je li trenutni resurs stranica ili odjeljak

- **Notebookid** – ID bilježnice programa OneNote

- **OperationWithError** – u kojoj se operaciji dogodila pogreška, npr. WebSocket.Close, WebSocket.Open, itd.

- **ResourceId** – ID resursa stranice ili odjeljka aplikacije OneNote

- **SectionId** – ID odjeljka aplikacije OneNote

- **ServerSessionId** – ID sesije koji se koristi za povezivanje zahtjeva web-utičnice s web-mjestom onenote.com

- **SessionDurationInMs** – trajanje sesije web-utičnice u milisekundama

- **TenantId** – ID klijenta sustava SharePoint

- **TimeToFirstUpdateInMs** – vrijeme u milisekundama potrebno za primanje prvog ažuriranja sa strane poslužitelja nakon uspostavljanja sesije web-utičnice

- **UploadAckCount** – broj potvrda za prijenos u sesiji web-utičnice

- **WebUrl** – PII čišćenje web URL-a 

### <a name="officeonenotestoragesectionsyncresult"></a>Office.OneNote.Storage.SectionSyncResult
 
Ovaj događaj zapisuje rezultat sinkronizacije odjeljka. Koristi se za otkrivanje broja jedinstvenih ciljeva sinkronizacije tijekom izračuna rezultata sinkronizacije aplikacije OneNote. Također se koristi za suvremenu sinkronizaciju performansi nadzorne ploče u aplikaciji OneNote.
 
Prikupljaju se sljedeća polja

- **Error_Code** – numerirani ili alfanumerički kod koji se koristi za određivanje prirode pogreške i/ili razloga pojave

- **Error_Description** – opis pogreške

- **Error_Tag** – označava mjesto na kojem se pogreška prikazuje u kodu

- **Error_Type** – vrsta pogreške, npr. Win32Error itd.

- **ErrorLast** – kôd pogreške posljednje viđene pogreške 

- **ExecutionTime** – vrijeme u milisekundama potrebno za repliciranje odjeljka

- **InitialReplicationInSession** – označava je li ova replikacija prva replikacija bilježnice nakon otvaranja ili nije

- **IsAttachedViaShortcut** – je odjeljak priložen putem prečaca ili ne

- **IsBackgroundSync** – označava je li ovo sinkronizacija u pozadini ili nije

- **IsEncrypted** – označava je li odjeljak šifriran ili nije

- **IsErrorSuppressed** – označava je li pogreška potisnuta ili nije 

- **IsErrorTransient** – označava je li ta pogreška prolazna ili nije

- **IsErrorUnexpected** – označava je li pogreška neočekivana ili nije

- **IsUsingRealtimeSync** – označava koristi li sinkronizacija odjeljka suvremenu sinkronizaciju sadržaja stranice ili ne

- **NotebookId** – ID bilježnice

- **NotebookPath** – PII čišćenje URL-a bilježnice

- **SectionPath** – PII čišćenje URL-a odjeljka

- **SectionReplicatingIsOutbound** – označava je li ova replikacija izlazna replikacija ili nije

- **SectionReplicatingIsSameIdentity** – označava je li se ova replikacija temelji na istom identitetu datoteke ili ne

- **SectionResourceId** – ID resursa odjeljka aplikacije OneNote

- **Success** – je li odjeljak uspješno sinkroniziran ili nije

- **SyncDestinationType** – vrsta odredišta sinkronizacije, npr. OneDrive ili SharePoint Online

- **SyncId** – broj jedinstven svakoj sinkronizaciji odjeljka

- **SyncWasFirstInSession** – označava je li ova sinkronizacija prva sinkronizacija u trenutnoj sesiji

- **SyncWasUserInitiated** – označava je li korisnik sinkronizacije pokrenut ili nije

- **TenantId** – ID klijenta sustava SharePoint

- **UnmappedGosid** – ID odjeljka prije primjene GUID mapiranja


### <a name="officeonenotestoragesyncscore"></a>Office.OneNote.Storage.SyncScore
 
Ovaj događaj evidentira sve negativne čimbenike u iskustvu sinkronizacije koji su vidljivi korisnicima. Koristi se za izračunavanje rezultata sinkronizacije programa OneNote, što je kritična metrika za procjenu iskustva sinkronizacije korisnika programa OneNote.
 
Prikupljaju se sljedeća polja

- **AutoShowSyncStatus** – označava je li status sinkronizacije automatski prikazan ili nije

- **Cause** – što je uzrokovalo da se stranice/odjeljci programa OneNote premjeste u pogrešno smještene odjeljke

- **Context** – identifikator kategorizira što korisnik pokušava učiniti, npr. preimenovati odjeljak, ponovno otvoriti bilježnicu itd.

- **Error_Code** – numerirani ili alfanumerički kod koji se koristi za određivanje prirode pogreške i/ili razloga pojave

- **Error_Description** – opis pogreške

- **Error_Tag** – označava mjesto na kojem se pogreška prikazuje u kodu

- **Error_Type** – vrsta pogreške, npr. Win32Error itd.

- **ErrorText** – tekst pogreške prikazan u korisničkom sučelju

- **Explanation** – objašnjava koje izlazne promjene na čekanju je potrebno premjestiti u pogrešno smještene odjeljke

- **fishbowlType** – vrsta akvarija, npr. stranica akvarija, odjeljak akvarija, itd.

- **IDS** – identifikator cijelog broja za tekst prikazan u korisničkom sučelju

- **idsFishbowl** – identifikator cijelog broja za pogrešku u akvariju prikazanu u korisničkom sučelju

- **IsUsingRealtimeHierarchySync** – označava koristi li suvremenu sinkronizaciju hijerarhije ili ne

- **NotebookId** – ID bilježnice

- **PageSyncUIState** – niz statusa sinkronizacije stranice, npr. ažurna, sinkronizira se, spremanje izvan mreže, pogreška prilikom sinkronizacije itd. 

- **ServerGosid** – ID resursa za novostvorenu stranicu sa sukobima

- **Source** – identifikator označava koji je događaj pokrenuo korisničko sučelje, tj. stvorio novu Redx sliku, pogrešku sinkronizacije u sučelju za sinkronizaciju, prikazan dijalog pogreške itd.

### <a name="onenoteappprovisioningmovelocalnotebooktoonlinenotebookfailed"></a>OneNote.App.Provisioning.MoveLocalNotebookToOnlineNotebookFailed
 
Taj se događaj bilježi kada premještanje lokalne bilježnice na pogon ne uspijeva.  Taj je scenarij specifičan za korisnika s odgođenom prijavom. Kada se korisnik prijavi, lokalna bilježnica će se prenijeti na spremište servisa OneDrive. 
 
Prikupljaju se sljedeća polja:
 
- **ErrorMsg** – poruka o pogrešci koja odgovara kvaru.

### <a name="onenotestorageconnectivitychanged"></a>OneNote.Storage.ConnectivityChanged

Događaj se evidentira bez obzira da li korisnik ima vezu sa internetom. Ta se funkcija koristi za povezivanje ostalih metrika performansi sinkronizacije i omogućuje nam ignoriranje događaja koji se javljaju dok korisnik ne koristi internetsku vezu jer ne očekujemo da će naše kašnjenje usluge biti prihvatljivo bez povezivanja s internetom. To nam omogućuje izračun točnog broja sesija za naš metrički broj na kriške korisnika (po-klijentu, po-sektorima). Pomoću nje možemo filtrirati i izvješća o pogreškama jer postoje brojne pogreške pri sinkronizaciji za koje očekujemo da će se pojavljivati bez mrežnog povezivanja, ali ta istraga ne jamči ništa.

Ako ne primimo te podatke ne možemo točno nadgledati performanse proizvoda ili odrediti hoće li se očekivati pogreške koje je iskusio korisnik ili zahtijevati daljnju istragu.

Prikupljaju se sljedeća polja:

- **InternetConnectivityNowAvailable** – ako je stanje povezivanja izmijenjeno, pa je sada Internet

### <a name="onenotestoragelegacyinboundlatency"></a>OneNote.Storage.LegacyInboundLatency

Kritični znak koji se koristi za praćenje operacija ulaznog sinkroniziranja koje komuniciraju izravno sa SharePoint sustavom, uključujući povezane informacije koje omogućuju praćenje i istraživanje performansi prijenosa podataka iz naše usluge. Ovaj se signal prikuplja samo za najgoru izvedbu u posljednjih 300 sekundi (broj sekundi može biti konfiguriran od strane Microsoft Corporation, ovisno o performansama i uvjetu usluge).

To se koristi da bi se osiguralo stanje usluge omogućujući nam da vidimo koji klijenti proživljavaju neprihvatljivo spore ulazne podatke za našu uslugu, informacije o podacima koje šalju kada su doživjeli spor ulaz i koliko je rasprostranjen problem s kašnjenjem unutar klijenta. Također se koristi za izvješćivanje o stanju i performansama servisa u svim našim korisnicima radi mjerenja trendova tijekom vremena i automatskog uzbunjivanja pitanja za inženjersko ublažavanje. Ako nemamo te podatke, to će nas spriječiti da osiguravamo odgovarajuće performanse kada se sinkronizacije korisnika promijene iz sustavu SharePoint na njihovo računalo.

Prikupljaju se sljedeća polja: 

- **IsEducationNotebook** – Booleova vrijednost koja ukazuje je li bilježnica za obrazovanje

- **SectionId** – ID bilježnice čiji je dio ovaj prijenos

- **TimeToConfirmSyncedWithServerInMs** – vrijeme u milisekundama koje je potrebno za obavljanje prijenosa

### <a name="onenotestoragelegacyoutboundlatency"></a>OneNote.Storage.LegacyOutboundLatency

Kritični znak koji se koristi za praćenje performansi operacija odlaznog sinkroniziranja koje komuniciraju izravno sa SharePoint sustavom, uključujući povezane informacije koje omogućuju praćenje i istraživanje performansi prijenosa podataka iz naše usluge. Ovaj se signal prikuplja samo za najgoru izvedbu u posljednjih 300 sekundi (broj sekundi može biti konfiguriran od strane Microsoft Corporation, ovisno o performansama i uvjetu usluge).

To se koristi da bi se osiguralo stanje usluge omogućujući nam da vidimo koji klijenti proživljavaju neprihvatljivo spore izlazne podatke ka našoj usluzi, informacije o podacima koje su slali kada su doživjeli spor izlaz i koliko je rasprostranjen problem s kašnjenjem unutar klijenta. Također se koristi za izvješćivanje o stanju i performansama servisa u svim našim korisnicima radi mjerenja trendova tijekom vremena i automatskog uzbunjivanja pitanja za inženjersko ublažavanje. Ako nemamo te podatke, to će nas spriječiti da osiguravamo odgovarajuće performanse kada se sinkronizirajući korisnici promijene u sustavu SharePoint. 

Prikupljaju se sljedeća polja: 

- **IsEducationNotebook** – Booleova vrijednost koja ukazuje je li bilježnica za obrazovanje

- **SectionId** – ID bilježnice čiji je dio ovaj prijenos

- **TimeToConfirmSyncedWithServerInMs** – vrijeme u milisekundama koje je potrebno za obavljanje prijenosa

### <a name="onenotestoragerealtimefiledataobjectdownload"></a>OneNote.Storage.RealTime.FileDataObjectDownload 

Kritični signal koji se koristi za praćenje performansi kada korisnik upisuje objekt podataka datoteke (npr. umetnuta datoteka ili slika) koja se preuzima izravno iz našeg servisa, a ne u sklopu postupka sinkronizacije na stranici, u odjeljku ili u bilježnici. Ovaj se signal prikuplja samo za najgoru izvedbu u posljednjih 300 sekundi (broj sekundi može biti konfiguriran od strane Microsoft Corporation, ovisno o performansama i uvjetu usluge).

To se koristi da bi se osiguralo stanje usluge i performanse omogućujući nam da vidimo koji klijenti proživljavaju neprihvatljivo sporo preuzimanje podataka iz naše usluge, i koliko je rasprostranjen problem s kašnjenjem unutar klijenta, te izvještava o našem ponašanju tijekom vremena i omogućuje nam da mjerimo trendove performansi usluge. Ako vam se prikaže neprihvatljivo kašnjenje za objekt datoteke, te ćemo podatke koristiti i za povezivanje s drugim signalima klijenta i servisa koji se tiču objekta radi poboljšanja našeg procesa preuzimanja. Podijelili smo i podatke na temelju proširenja preuzetog objekta datoteke kao što imamo različita očekivanja koja se temelje na tome je li datoteka prikazana u okviru našeg platna (npr. slika) ili je datoteka koja se ne umetne u obliku teksta (npr. tekstni dokument). Ako ne primimo te podatke, onemogućit će nam praćenje performansi tih preuzimanja

Prikupljaju se sljedeća polja: 

- **Datoteka** – veličina datoteke preuzete u bajtovima 

- **IsImage** – A Booleova vrijednost koja određuje je li preuzeta datoteka ima proširenje koje se podudara s unaprijed definiranim popisom uobičajenih formata slika (.bmp, .emf, .gif, .jpe, .jpeg, .jpg, .png) koje smo prikazali u sklopu platna

- **TimeToDownload** – trajanje uspješnog preuzimanja FDO-a s našeg prostora za pohranu bloka na uređaj 

### <a name="onenotestoragerealtimewebsocketdownload"></a>OneNote.Storage.RealTime.WebSocketDownload

Ključni znak koji se koristi za praćenje performansi ulaznog sinkroniziranja sustava, uključujući povezane podatke koji omogućuju praćenje i proučavanje performansi preuzimanja podataka iz našeg servisa (onenote.com). Ovaj se signal prikuplja samo za najgoru izvedbu u posljednjih 300 sekundi (broj sekundi može biti konfiguriran od strane Microsoft Corporation, ovisno o performansama i uvjetu usluge).

To se koristi da bi se osiguralo stanje usluge omogućujući nam da vidimo koji klijenti proživljavaju neprihvatljivo spore ulazne podatke iz naše usluge, informacije o podacima koje su preuzimali kada su doživjeli spor ulaz i koliko je rasprostranjen problem s kašnjenjem unutar klijenta. Također se koristi za izvješćivanje o stanju i performansama servisa u svim našim korisnicima radi mjerenja trendova tijekom vremena i automatskog uzbunjivanja pitanja za inženjersko ublažavanje. 

Ako uočimo neprihvatljivo kašnjenje za odjeljak ili bilježnicu, te ćemo podatke koristiti i za povezivanje s drugim signalima klijenta i usluge koji se odnose na isti dokument radi identificiranja regresija performansi na strani klijenta, što nam omogućuje pružanje usluge s boljim performansama.

Ako ne primimo te podatke, nećemo moći pratiti performanse tog aspekta naše usluge ni učinak promjena na strani poslužitelja koje možda smatramo potrebnim zbog korištenja ili drugih faktora.

Prikupljaju se sljedeća polja:

- **DeviceSessionId**  – ID sesije uređaja

- **IsEducationNotebook** – Booleova vrijednost koja ukazuje je li bilježnica za obrazovanje

- **IsHierarchyResource** – Booleova vrijednost koja ukazuje da li je resurs hijerarhijski

- **SectionId** – ID bilježnice čiji je dio ovaj prijenos

- **ResourceId** – ID resursa koji prenosimo

- **SectionId** – ID odjeljka čiji je dio ovaj prijenos

- **ServerSessionId** – ID sesije poslužitelja čiji je dio ovaj prijenos

- **TimeToConfirmSyncedWithServerInMs** – vrijeme u milisekundama između korisnika koji se nalazi na stranici i stoga replikacije koji potvrduje da se stranica sinkronizira s poslužiteljem.

- **TimeToFirstUpdateInMs** – vrijeme u milisekundama između sustava za sinkronizaciju koji počinje ulaznu replikaciju stranice te funkcije replikacije pri sinkronizaciji s stanjem poslužitelja.

### <a name="onenotestoragerealtimewebsocketupload"></a>OneNote.Storage.RealTime.WebSocketUpload

Ključni znak koji se koristi za praćenje performansi ulaznog sinkroniziranja sustava, uključujući povezane informacije koje omogućuju praćenje i proučavanje performansi preuzimanja podataka iz našeg servisa (onenote.com).

To se koristi da bi se osiguralo stanje usluge omogućujući nam da vidimo koji klijenti proživljavaju neprihvatljivo spore izlazne podatke ka našoj usluzi, informacije o podacima koje su slali kada su doživjeli spor izlaz i koliko je rasprostranjen problem s kašnjenjem unutar klijenta. Također se koristi za izvješćivanje o stanju i performansama servisa u svim našim korisnicima radi mjerenja trendova tijekom vremena i automatskog uzbunjivanja pitanja za inženjersko ublažavanje. Te ćemo podatke koristiti i za praćenje učinka i djelotvornosti poboljšanja koja smo napravili klijentima i uslugama. 

Ako vidimo neprihvatljivo kašnjenje za odjeljak ili bilježnicu, te ćemo podatke koristiti i za povezivanje s drugim signalima klijenta i usluge koji se odnose na isti dokument radi identificiranja regresija performansi koja nam omogućuje da isporučimo doživljaj s boljim performansama.

Ako ne primimo te podatke, nećemo moći pratiti performanse tog aspekta naše usluge ni učinak promjena na strani poslužitelja koje možda smatramo potrebnim zbog korištenja ili drugih faktora.

Prikupljaju se sljedeća polja: 

- **DeviceSessionId** – ID sesije uređaja

- **IsEducationNotebook** – Booleova vrijednost koja ukazuje je li bilježnica za obrazovanje

- **IsHierarchyResource** – Booleova vrijednost koja ukazuje da li je resurs hijerarhijski

- **IsWorstTime** – Booleova vrijednost koji upućuje na to da li je vrijeme redovnog prijenosa događaja obično ili najgore vrijeme koje smo vidjeli na tom klijentu u posljednjih 300 sekundi (broj sekundi može biti konfiguriran od strane Microsoft Corporation ovisno o performansama i uvjetu usluge).

- **SectionId** – ID bilježnice čiji je dio ovaj prijenos

- **RecommendedPutIntervalInMs** – vrijeme koje je servis prenio klijentu kao preporučeno vremensko razdoblje

- **ResourceId** – ID resursa koji prenosimo

- **SectionId** – ID odjeljka čiji je dio ovaj prijenos

- **SenderRequestId** – ID pošiljaoca koji izvršava prijenos

- **ServerSessionId** – ID sesije poslužitelja čiji je dio ovaj prijenos

- **UploadNonSuspendedTimeInMs** – vrijeme u milisekundama koje je potrebno za izvršavanje prijenosa izuzevši vrijeme kada je aplikacija suspendirana

- **UploadTimeInMs** – vrijeme u milisekundama koje je potrebno za obavljanje prijenosa

- **WaitTimeInMs** – vrijeme u milisekundama između zatraženog prijenosa i pokretanja prijenosa

- **WebUrl** – Web URL prijenosa (prijavljeni kao PiiWz)

### <a name="onenotestoragesynchealth"></a>OneNote.Storage.SyncHealth

Ključni znak koji se koristi za praćenje pogrešaka i iznimki koje su se dogodile unutar stoga za sinkronizaciju u klijentu programa OneNote koji nam omogućuje praćenje i ublažavanje tih neočekivanih uvjeta.

To se koristi da bi se osiguralo dobro stanje usluge, a omogućuje nam pregled izvješća o pogreškama iz klijenata u gotovo stvarnom vremenu, što nam pruža mogućnost reakcije na probleme sa sinkronizacijom čim se pojave. Također se koristi da bi se utvrdilo koliko je rasprostranjen problem te koliko je ozbiljan, unakrsnim referenciranjem oznake pogreške s klijentskim kodom da bi se utvrdio izvor pogreške. Također smo skupili te podatke da bismo dobili informacije o našim performansama tijekom vremena i utjecaju i djelotvornosti poboljšanja koja dajemo klijentima i uslugama. Ako nemamo te podatke, nećemo moći proaktivno reagirati na uvjete pogreške u našem servisu za sinkronizaciju bez porasta eskalacije korisnika.

Prikupljaju se sljedeća polja: 

- **Service** – servis za sinkronizaciju koji je klijent koristio kada se dogodila pogreška (naslijeđena ili moderna sinkronizacija)

- **Tag** – Oznaka (identifikacijska vrijednost) koja predstavlja pogrešku na koju je klijent naišao tijekom postupka sinkronizacije

### <a name="onenotesynccreatenotebookfailed"></a>OneNote.Sync.CreateNotebookFailed
 
Taj se događaj bilježi kad stvaranje bilježnice ne uspije.  
 
Prikupljaju se sljedeća polja:
 
- **NetworkConnection**- Zapisuje vrstu veze na kojoj se uređaj trenutno nalazi, npr. Wi-Fi, izvanmrežni rad, 3G 

- **ServerType**- Zapisuje vrstu poslužitelja gdje će se stvoriti bilježnica.

### <a name="onenotesyncfirstrunerror"></a>OneNote.Sync.FirstRunError
 
Taj se događaj bilježi kada sinkronizacija za Brze napomene ne uspije za korisnika tijekom prvog pokretanja sustava na uređaju.  To je specifično za scenarij prvog izvođenja.
 
Prikupljaju se sljedeća polja:
 
- **NetworkConnection**- Zapisuje vrstu veze na kojoj se uređaj trenutno nalazi, npr. Wi-Fi, izvanmrežni rad, 3G

- **ServerType**- Zapisuje vrstu poslužitelja gdje će se stvoriti bilježnica za brze bilješke.

## <a name="services-configuration-events"></a>Događaji konfiguracije servisa

Konfiguracija servisa ne prikuplja događaje vezane uz obavezne servisne podatke.

## <a name="telemetry-events"></a>Telemetrijski događaji

### <a name="officeandroiddocsuipaywallcontrolpaywalloperationmetrics"></a>Office.Android.DocsUI.PaywallControl.PaywallOperationMetrics

*[Taj se događaj prije zvao Office.Android.DocsUI.Views.PaywallOperationMetrics.]*

Microsoft to koristi za dobivanje ispravnosti značajke, uspjeha ili stope pogrešaka za korisnike pri kupnjama, kako bi osigurao odgovarajuća ulaganja za poboljšanje korisničkog iskustva kupca na mobilnim platformama.

Prikupljaju se sljedeća polja:

- **OperationTimeInMs** – vrijeme potrebno za završetak postupka kupnje (dugo – millisekunde)

- **PaywallOperationResult** – Uspjeh/ šifra pogreške / korisnik otkazan (Enum / int – konačna)

- **PaywallOperationType** – označava vrstu Paywall operacije (enum/ int – konačna)

### <a name="officeandroiddocsuipaywallcontrolpaywallsessiondata"></a>Office.Android.DocsUI.PaywallControl.PaywallSessionData

*[Taj se događaj prije zvao Office.Android.DocsUI.Views.PaywallSessionData.]*

Metapodaci koji se temelje na sesiji kada se korisniku prikazuje korisničko sučelje Paywall. Microsoft to koristi kako bi dobio putovanje korisnika i razumio koje verzije uređaja i OS-a korisnik upotrebljava, kao pomoć u donošenju odluka o ulaganjima u poboljšanja iskustva u tim područjima.

Prikupljaju se sljedeća polja:

- **App Version** – šifra verzije drugih programa

- **ClientId** – anoniman jedinstven identifikator uređaja koji ne otkriva identitet krajnjeg korisnika (guid/niz)

- **Entry Point** – jedinstveni identifikator za kontekstualne ili konstante točke ulaza iz drugih programa

- **isTablet** – prikazuje li uređaj korisničko sučelje tableta

- **OSVersion** – verzija OS-a Android za uređaj

- **SessionId** – Guid: jedinstveni identifikator sesije Paywall


### <a name="officefirstrunappletelemetryoptin"></a>Office.FirstRun.Apple.TelemetryOptIn

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za nadziranje stanja telemetrijske funkcije uključivanja u iskustvo prvog pokretanja. Prikupljamo kôd koji označava vrstu mogućnosti za prikupljanje dijagnostičkih podataka koju je korisnik odabrao.

Prikupljaju se sljedeća polja:

- **Data_EventId** – Kôd koji pokazuje preferenciju prikupljanja podataka koju je odabrao korisnik.

### <a name="officeiospaywallprovisioningresponse"></a>Office.iOS.Paywall.Provisioning.Response

Telemetrija proizvoda koja se upotrebljava za usklađivanje podataka o transakcijama kupnje s Microsoftovim sustavom trgovine radi omogućivanja povezanih pogodnosti pretplate. Koristi se za olakšavanje evidentiranja transakcija i omogućavanja pretplate za buduću referencu i interno usklađivanje.

Prikupljaju se sljedeća polja:

- **entryPoint** – niz – gumb/tijek s kojeg je prikazan Paywall. Kao što je "Premium Upgrade Button" ili „First run flow“

- **failureReason** – niz – dodan samo kada je status "neuspjeh". Ukazuje na odgovor na pogrešku koji je dao RFS.

- **productId** – niz – ID proizvoda trgovine App Store za koji je izrađen zahtjev

- **stanje** – niz – uspjeh ili neuspjeh, što upućuje na to je li zahtjev uspio ili ne


### <a name="officeiospaywallstorekitresponse"></a>Office.iOS.Paywall.StoreKit.Response

Podaci se prikupljaju kao kritična inženjerska telemetrija za bilježenje rezultata pokušaja kupnje koji je korisnik pokrenuo ručno. Telemetrija proizvoda upotrebljava se za usklađivanje podataka o transakcijama kupnje s Microsoftovim sustavom trgovine radi omogućivanja povezanih pogodnosti pretplate.

Prikupljaju se sljedeća polja:

- **entryPoint** – niz – gumb/tijek s kojeg je prikazan Paywall. Kao što je "Premium Upgrade Button" ili „First run flow“

- **failureReason** – niz – dodan samo kada je status "neuspjeh". Ukazuje na odgovor na pogrešku koji je dala trgovina App-store.

- **productId** – niz – samo za „MakePurchase“, „PendingPurchase”, ID proizvoda trgovine app-store za koji je zahtjev stvoren.

- **productsCount** -Int – samo za "ProductsFetch", broj proizvoda koje trgovina vraća.

- **requestType** – niz – vrsta zahtjeva za Storekit. Kao što je "ProductsFetch", "Pendingpurchase"

- **status** – niz – uspjeh ili neuspjeh, što upućuje na uspjeh ili neuspjeh zahtjeva

### <a name="officeonenotegetsharepointidsfordocument"></a>Office.OneNote.GetSharePointIdsForDocument

Prikupljeni podaci bilježe neuspješnost ili uspješnost dohvaćanja ID-ova sustava SharePoint (SPO) za URL dokumenta. Uspješnost i neuspješnost (uključujući razlog neuspjeha) poziva bilježe se za sve platforme. Ta je oznaka obavezna za praćenje i dijagnostiku stanja poziva koji se upućuje radi pribavljanja ID-ova. ID-ovi u sažetku sadržaja moraju prikazivati podatke sa stranice programa OneNote (koja pripada bilježnicama pohranjenim u sustavu SharePoint). 

Prikupljaju se sljedeća polja:

- **ErrorCode** – cjelobrojna vrijednost pogreške

- **ErrorMessage** – niz koji opisuje pogrešku

- **FailureType** – niz za određivanje vrste pogreške

- **HTTP-statuscode** – kôd HTTTP pogreške za mrežni poziv

- **InnerErrorCode** – cjelobrojni kôd

- **InnerErrorMesage** – poruka za pogrešku

- **IsSuccess** – Booleova vrijednost za uspješnost signala

### <a name="officeonenotegetsharepointidsfordocumentw32old"></a>Office.OneNote.GetSharePointIdsForDocumentW32Old

Telemetrija bilježi scenarije neuspjeha i uspješnost dohvaćanja ID-ova sustava SharePoint (SPO) za URL dokumenta. Bilježi se uspješnost ili neuspješnost (uključujući razlog neuspjeha) poziva. To se bilježi samo na staroj platformi win32. Ta je oznaka obavezna za praćenje i dijagnostiku stanja poziva koji se upućuje radi pribavljanja ID-ova. ID-ovi u sažetku sadržaja moraju prikazivati podatke sa stranice programa OneNote (koja pripada bilježnicama pohranjenim u sustavu SharePoint). 

Prikupljaju se sljedeća polja:

- **ErrorCode** – cjelobrojna vrijednost pogreške

- **ErrorMessage** – niz koji opisuje pogrešku

- **FailureType** – niz za određivanje vrste pogreške

- **HTTP-statuscode** – kôd HTTTP pogreške za mrežni poziv

- **InnerErrorCode** – cjelobrojni kôd

- **InnerErrorMesage** – poruka za pogrešku

- **IsSuccess** – Booleova vrijednost za uspješnost signala


### <a name="officesystemgracefulexitgracefulappexitdesktop"></a>Office.System.GracefulExit.GracefulAppExitDesktop

Događaj je aktiviralo skladno ukidanje aplikacije za klijentske aplikacije sustava Office, kao što su, no ne ograničavajući se na Word, Excel, PowerPoint i Outlook. Parametre skladnog zatvaranja upotrebljavamo za mjerenje stanja proizvoda klijenata sustava Office. To je zamišljeno da bude signal ključan za poslovanje koji inženjeri sustava Office koriste za postizanje stabilnosti proizvoda.

Prikupljaju se sljedeća polja:

- **AppBuild** – identifikator međuverzije zahvaćenog procesa.
- **AppMajor** – identifikator glavne verzije zahvaćenog procesa.
- **AppMinor** – identifikator sporedne verzije zahvaćenog procesa.
- **AppRevision** – identifikator međuverzije zahvaćenog procesa.
- **Boot Completed** – dovršio je postupak pokretanja sustava Office.
- **DetectionTime** – vrijeme otkrivanja neočekivanog zatvaranja.
- **EcsETag** – identifikator eksperimenta za postupak.
- **HasEdit** – uređivanje dokumenta koje se pojavljuje tijekom postupka sustava Office.
- **HasOpen** – dokument je bio otvoren tijekom postupka sustava Office.
- **InstallMethod** – određuje je li sustav nadograđen na trenutačnu međuverziju sustava Office, vraćen na nju ili je u pitanju nova instalacija.
- **OfficeUILang** – jezik postupka sustava Office.
- **PreviousBuild** – prethodno instalirana međuverzija.
- **SafeMode** – jest postupak sustava Office u sigurnom načinu rada.
- **SessionId** – jedinstveni identifikator procesa.
- **SessionInitTime** – Vrijeme pokretanja zahvaćenog procesa.

### <a name="officesystemidentitychanged"></a>Office.System.IdentityChanged

Podaci o identitetu korisnika koji su potrebni za ispunjavanje zahtjeva ispitanika.

Prikupljaju se sljedeća polja:

  - **IdentityChanged** – uvijek ima vrijednost true. Identitet je promijenjen.

  - **TimerDetectedChange** – označava je li redovno tempiran ping otkrio promjenu.

### <a name="officesystemprivacyfallbacktosettingsstore"></a>Office.System.PrivacyFallbackToSettingsStore

Koristi se kako bi se tvrdilo ima li neuspjeha u čitanju korisničkih postavki privatnosti iz Roaming trgovine.

Prikupljaju se sljedeća polja:

  - **Tag –** oznaka koda označava koja se postavka vratila u pohranu postavki.

### <a name="officesystemsessiondatao365"></a>Office.System.SessionDataO365

Metapodaci koji su potrebni za izoliranje reprodukcije pogreške.

Prikupljaju se sljedeća polja:

  - **AppId –** identifikator aplikacije sustava Office na koju se podaci odnose.

  - **ApplicationArchitecture –** označava za koju je arhitekturu procesora Office namijenjen.

  - **AppVersionBuild –** međuverzija aplikacije sustava Office.

  - **AppVersionMajor –** glavna verzija aplikacije sustava Office.

  - **AppVersionMinor –** sporedna verzija aplikacije sustava Office.

  - **AppVersionUpdate –** revizija međuverzije aplikacije sustava Office.

  - **CollectorVersion –** identifikator verzije za logiku prikupljanja s klijenta.

  - **DeviceHash –** jednosmjerno raspršivanje identifikatora operacijskog sustava uređaja.

  - **DeviceName –** naziv uređaja na kojem je Office pokrenut.

  - **Domain –** domena uređaja na kojem je Office pokrenut.

  - **IsCeip –** označava je li instalacija sustava Office registrirana u neispravan Program unaprjeđivanja zadovoljstva korisnika.

  - **IsDebug –** označava radi li se o međuverziji sustava Office za ispravljanje pogrešaka.

  - **IsImmersive –** označava je li aplikacija sustava Office aplikacija za Universal Windows ili stopljena aplikacija.

  - **IsLaptop –** označava je li uređaj na kojem je Office pokrenut prijenosno računalo.

  - **IsMicrosoftInternal –** označava je li korisnik sustava Windows koji pokreće Office Microsoftov zaposlenik.

  - **IsO365 –** označava je li instalaciju sustava Office dio neispravnog programa Outlook 365.

  - **IsTablet –** označava je li uređaj na kojem je Office pokrenut tablet.

  - **IsTerminalServer –** vrijednost true/false koja označava je li u pitanju klijent za terminalski poslužitelj

  - **MaxMemory –** maksimalna količina dostupne radne memorije na uređaju na kojem je pokrenut Office.

  - **OsArchitecture –** arhitektura procesora za koju je Office pokrenut u operacijskom sustavu namijenjen.

  - **OsVersionBuild –** međuverzija operacijskog sustava.

  - **OsVersionMajor –** glavna verzija operacijskog sustava.

  - **OsVersionMinor –** sporedna verzija operacijskog sustava.

  - **OsVersionUpdate –** revizija međuverzije operacijskog sustava

  - **ProcessFileName –** naziv izvršne datoteke pokrenute aplikacije.

  - **ProcesorArchitecture –** arhitektura procesora u kojoj je Office pokrenut.

  - **ProcessorFrequency –** brzina procesora na uređajima na kojima je Office pokrenut u megahercima.

  - **SessionStart –** vrijeme pokretanja aktivnog sustava Office.

  - **UserName –** naziv računa koji je pokrenuo Office.

### <a name="officesystemsystemhealthcoremetadata"></a>Office.System.SystemHealthCoreMetadata

Metapodaci koji su potrebni za izoliranje reprodukcije pogreške.

Prikupljaju se sljedeća polja:

  - **AppBuild –** međuverzija aplikacije sustava Office.

  - **AppBuildRevision –** revizija međuverzije aplikacije sustava Office.

  - **AppMajorVer –** glavna verzija aplikacije sustava Office.

  - **AppMinorVer –** sporedna verzija aplikacije sustava Office.

  - **CID –** identitet korisnika u obliku pseudonima

  - **CollectibleClassifications –** skup klasifikacija podataka koje se mogu prikupiti.

  - **CollectionTime –** vrijeme kada su metapodaci prikupljeni.

  - **DeviceManufacturer –** proizvođač uređaja na kojem je Office pokrenut.

  - **DeviceModel –** model uređaja na kojem je Office pokrenut.

  - **FirstRunTime –** vrijeme prvog pokretanja aplikacije sustava Office.

  - **IsClickToRunInstall –** označava je li aplikacija sustava Office instalirana pomoću tehnologije "klikom do cilja"

  - **IsDebug –** označava radi li se o međuverziji sustava Office za ispravljanje pogrešaka.

  - **IsLabMachine –** određuje pokreće li se Office u Microsoftovu laboratoriju.

  - **IsLaptop –** označava je li uređaj na kojem je Office pokrenut prijenosno računalo.

  - **IsMsftInternal –** označava je li korisnik sustava Windows koji pokreće Office Microsoftov zaposlenik.

  - **IsSubscription –** označava je li aplikacija sustava Office instalirana pod pretplatničkom licencom.

  - **IsTablet –** označava je li uređaj na kojem je Office pokrenut tablet.

  - **IsTerminalServer –** označava pokreće li se Office na terminalskom poslužitelju.

  - **MsoAppId –** identifikator aplikacije sustava Office na koju se podaci odnose.

  - **OfficeArchitectureText –** označava za koju je arhitekturu procesora Office namijenjen.

  - **OsBuild –** međuverzija operacijskog sustava.

  - **OsBuildRevision –** revizija međuverzije operacijskog sustava

  - **OSEnvironment –** identifikator okruženja u kojem je Office pokrenut.

  - **OsMajorVer –** glavna verzija operacijskog sustava.

  - **OsMinorVer –** sporedna verzija operacijskog sustava.

  - **OSVersionString –** verzija operacijskog sustava kao niz.

  - **ProcesorArchitecture –** arhitektura procesora u kojoj je Office pokrenut.

  - **ProcessorCount –** broj procesora na uređaju na kojem je Office pokrenut.

  - **ProcSpeedMHz –** brzina procesora na uređajima na kojima je Office pokrenut u megahercima.

  - **RamMB –** količina dostupnog RAM-a na uređaju na kojem je Office pokrenut.

  - **SqmUserId –** nasumični identifikator instalacije sustava Office.

### <a name="officesystemsystemhealthdesktopsessionlifecycleandheartbeat"></a>Office.System.SystemHealthDesktopSessionLifecycleAndHeartbeat

Sadrži informacije o metrici stanja sustava.

Prikupljaju se sljedeća polja:

  - **InstallMethod** – određuje je li sustav nadograđen na trenutnu međuverziju sustava Office, vraćen na nju ili je u pitanju nova instalacija.

  - **OfficeArchitectureText** – Arhitektura proizvoda sustava Office predstavljena kao niz (npr. x86, arm).

  - **PreviousBuild** – verzija sustava Office na koju je međuverzija nadograđena ili s koje je vraćene.

  - **State** – stanje u koje je sesija promijenjena.

  - **Vrijeme** – vrijeme promjene stanja sesije.

### <a name="officesystemsystemhealthessentialidentitycount"></a>Office.System.SystemHealthEssentialIdentityCount

Prikuplja broj identiteta prijavljenih korisnika

Prikupljaju se sljedeća polja:

  - **AllIdentityCount** – broj svih identiteta

  - **ValidIdentityCount** – broj potvrđenih identiteta

### <a name="officesystemsystemhealthessentialmetadataallidentities"></a>Office.System.SystemHealthEssentialMetadataAllIdentities

Nadzire stanje računa koje je Office prepoznao u ovoj sesiji. Koristi se za izoliranja pogreške na vrstu prijave na račun ako je pogreška specifična za vrstu.

Prikupljaju se sljedeća polja:

  - **CollectionTime** – vrijeme prikupljanja podataka o identitetu.

  - **IdentityType** – vrsta provjere autentičnosti ili računa

  - **IdentityUniqueId** – identifikator identiteta u obliku pseudonima

  - **IdentityUniqueIdHashed** – jednosmjerno raspršivanje jedinstvenog ID-a identiteta

### <a name="officesystemsystemhealthmetadataapplicationadditional"></a>Office.System.SystemHealthMetadataApplicationAdditional

Metapodaci koji su potrebni za izoliranje reprodukcije pogreške.

Prikupljaju se sljedeća polja:

  - **Alias –** ako je korisnik koji pokreće Office Microsoftov zaposlenik, ovo je interni pseudonim u tvrtki.

  - **AppBuild –** međuverzija aplikacije sustava Office.

  - **AppBuildRevision –** revizija međuverzije aplikacije sustava Office.

  - **AppMajorVer –** glavna verzija aplikacije sustava Office.

  - **AppMinorVer –** sporedna verzija aplikacije sustava Office.

  - **CID –** identitet korisnika u obliku pseudonima

  - **CollectibleClassifications –** skup klasifikacija podataka koje se mogu prikupiti.

  - **DeviceManufacturer –** proizvođač uređaja na kojem je Office pokrenut.

  - **DeviceModel –** model uređaja na kojem je Office pokrenut.

  - **DeviceProcessorModel –** model procesora uređaja na kojem je Office pokrenut.

  - **DigitizerInfo –** podaci o digitalizatoru koji je priključen na uređaj na kojem je Office pokrenut.

  - **DomainName –** naziv domene kojoj je pridruženo računalo na kojem je Office pokrenut (ako postoji).

  - **FirstRunTime –** vrijeme prvog pokretanja aplikacije sustava Office.

  - **HorizontalResolution –** vodoravna razlučivost zaslona

  - **IsDebug –** označava radi li se o međuverziji sustava Office za ispravljanje pogrešaka.

  - **IsImmersive –** označava je li aplikacija sustava Office aplikacija za Universal Windows ili stopljena aplikacija.

  - **IsJoinedToDomain –** označava je li uređaj na kojem je Office pokrenut pridružen domeni.

  - **IsLabMachine –** određuje pokreće li se Office u Microsoftovu laboratoriju.

  - **IsLaptop –** označava je li uređaj na kojem je Office pokrenut prijenosno računalo.

  - **IsMsftInternal –** označava je li korisnik sustava Windows koji pokreće Office Microsoftov zaposlenik.

  - **IsOEMInstalled –** označava je li pokrenutu aplikaciju sustava Office instalirao OEM.

  - **IsRunAsAdmin –** označava je li aplikacija sustava Office pokrenuta kao administrator.

  - **IsSubscription –** označava je li aplikacija sustava Office instalirana pod pretplatničkom licencom.

  - **MsoAppId –** identifikator aplikacije sustava Office na koju se podaci odnose.

  - **NumProcPhysCores –** broj fizičkih jezgri procesora.

  - **OfficeBuild –** međuverzija zajedničkih biblioteka sustava Office.

  - **OfficeBuildRevision –** revizija međuverzije zajedničkih biblioteka sustava Office.

  - **OfficeMajorVer –** glavna verzija zajedničkih biblioteka sustava Office.

  - **OfficeMinorVer –** sporedna verzija zajedničkih biblioteka sustava Office.

  - **OsBuild –** međuverzija operacijskog sustava.

  - **OsBuildRevision –** revizija međuverzije operacijskog sustava

  - **OsMajorVer –** glavna verzija operacijskog sustava.

  - **OsMinorVer –** sporedna verzija operacijskog sustava.

  - **PowerPlatformRole –** identifikator preferirane uloge računala prema OEM-u za uređaj na kojem je Office pokrenut.

  - **ProcessFileName –** naziv izvršne datoteke pokrenute aplikacije.

  - **ProcessorCount –** broj procesora na uređaju na kojem se Office pokreće.

  - **RamMB –** količina dostupnog RAM-a na uređaju na kojem je Office pokrenut.

  - **SqmUserId –** nasumični identifikator instalacije sustava Office.

  - **StudyId –** identifikator u ispitivanju Software Quality Metrics.

  - **VerticalResolution –** okomita razlučivost zaslona

  - **WinUserActType –** označava je li korisnik sustava Windows koji pokreće Office lokalni administrator, napredni korisnik ili normalni korisnik.

### <a name="officesystemsystemhealthmetadataapplicationandlanguage"></a>Office.System.SystemHealthMetadataApplicationAndLanguage

Metapodaci su potrebni za izoliranje reprodukcije pogreške.

Prikupljaju se sljedeća polja:

  - **AppBuild –** međuverzija aplikacije sustava Office.

  - **AppBuildRevision –** revizija međuverzije aplikacije sustava Office.

  - **AppMajorVer –** glavna verzija aplikacije sustava Office.

  - **AppMinorVer –** sporedna verzija aplikacije sustava Office.

  - **AppState –** identifikator stanja u kojem se aplikacija sustava Office nalazi.

  - **Click2RunPackageVersionBuild –** međuverzija instalacijskog paketa s tehnologijom "klikom do cilja".

  - **Click2RunPackageVersionMajor –** glavna verzija instalacijskog paketa s tehnologijom "klikom do cilja".

  - **Click2RunPackageVersionMinor –** sporedna verzija instalacijskog paketa s tehnologijom "klikom do cilja".

  - **Click2RunPackageVersionRevision –** revizija međuverzije instalacijskog paketa s tehnologijom "klikom do cilja".

  - **DistributionChannel –** kanal putem kojeg je Office distribuiran.

  - **InstallType –** identifikator metode kojom je Office instaliran.

  - **IsClickToRunInstall –** označava je li aplikacija sustava Office instalirana pomoću tehnologije "klikom do cilja"

  - **IsDebug –** označava radi li se o međuverziji sustava Office za ispravljanje pogrešaka.

  - **IsImmersive –** označava je li aplikacija sustava Office aplikacija za Universal Windows ili stopljena aplikacija.

  - **IsMsftInternal –** označava je li korisnik sustava Windows koji pokreće Office Microsoftov zaposlenik.

  - **IsOEMInstalled –** označava je li pokrenutu aplikaciju sustava Office instalirao OEM.

  - **IsRunAsAdmin –** označava je li aplikacija sustava Office pokrenuta kao administrator.

  - **IsSubscription –** označava je li aplikacija sustava Office instalirana pod pretplatničkom licencom.

  - **MsoAppId –** identifikator aplikacije sustava Office na koju se podaci odnose.

  - **OfficeArchitectureText –** označava za koju je arhitekturu procesora Office namijenjen.

  - **OfficeBuild –** međuverzija zajedničkih biblioteka sustava Office.

  - **OfficeBuildRevision –** revizija međuverzije zajedničkih biblioteka sustava Office.

  - **OfficeMajorVer –** glavna verzija zajedničkih biblioteka sustava Office.

  - **OfficeMinorVer –** sporedna verzija zajedničkih biblioteka sustava Office.

  - **OfficeMuiCount –** broj instaliranih jezičnih paketa za Office.

  - **OfficeSkuLanguage –** jezik instaliranog SKU-a.

  - **OfficeSkuLanguageTag –** jezik instaliranog SKU-a.

  - **OfficeUiLang –** jezik korisničkog sučelja aplikacije sustava Office.

  - **OfficeUiLangTag –** jezik korisničkog sučelja aplikacije sustava Office.

  - **ProcessFileName –** naziv izvršne datoteke pokrenute aplikacije.

  - **SqmAppId –** identifikator aplikacije sustava Office na koju se podaci odnose.

### <a name="officesystemsystemhealthmetadatadelayedlogin"></a>Office.System.SystemHealthMetadataDelayedLogin

Podaci o identitetu korisnika koji su potrebni za ispunjavanje zahtjeva ispitanika.

Prikupljaju se sljedeća polja:

  - **CID –** identitet korisnika u obliku pseudonima

### <a name="officesystemsystemhealthmetadatadevice"></a>Office.System.SystemHealthMetadataDevice

Metapodaci koji su potrebni za izoliranje reprodukcije pogreške.

Prikupljaju se sljedeća polja:

  - **CollectionTime –** vrijeme kada su metapodaci prikupljeni.

  - **ComputerSystemProductUuidHash –** jednosmjerno raspršivanje UUID-a matične ploče.

  - **DeviceClass –** identifikator za vrstu uređaja na kojem se pokreće Office.

  - **DeviceMake –** identifikator linije hardverskog sustava za uređaj na kojem je Office pokrenut.

  - **DeviceManufacturer –** proizvođač uređaja na kojem je Office pokrenut.

  - **DeviceModel –** model uređaja na kojem je Office pokrenut.

  - **DigitizerInfo –** podaci o digitalizatoru koji je priključen na uređaj na kojem je Office pokrenut.

  - **IsLaptop –** označava je li uređaj na kojem je Office pokrenut prijenosno računalo.

  - **IsTablet –** označava je li uređaj na kojem je Office pokrenut tablet.

  - **LicensingACID –** identifikator licenciranja instalacije sustava Office.

  - **MachineName –** naziv uređaja na kojem se Office pokreće.

  - **NumProcPhysCores –** broj fizičkih jezgri procesora.

  - **NumProcShareSingleCache –** broj procesora koji zajednički koriste jednu predmemoriju na uređaju na kojem se Office pokreće.

  - **NumProcShareSingleCore –** broj procesora po fizičkoj jezgri na uređaju na kojem se Office pokreće.

  - **OlsLicenseId –** identifikator servisa za licenciranje za instalaciju sustava Office.

  - **Platform –** identifikator okruženja u kojem se Office pokreće.

  - **PowerPlatformRole –** identifikator preferirane uloge računala prema OEM-u za uređaj na kojem je Office pokrenut.

  - **ProcessorCount –** broj procesora na uređaju na kojem se Office pokreće.

  - **ProcSpeedMHz –** brzina procesora na uređaju na kojem se Office pokreće u megahercima.

  - **ProcType –** arhitektura procesora.

  - **ProcTypeText –** vrsta procesora na uređaju na kojem se Office pokreće.

  - **RamMB –** količina dostupnog RAM-a na uređaju na kojem je Office pokrenut.

  - **SusClientId –** ID za Windows Update uređaja na kojem se Office pokreće.

  - **SystemFamily –** identifikator linije hardverskog sustava za uređaj na kojem je Office pokrenut.

  - **SystemSKU –** identifikator SKU-a hardverskog sustava za uređaj na kojem je Office pokrenut.

  - **SysVolFreeSpaceMB –** količina slobodnog prostora na sistemskom disku u megabajtima.

  - **SysVolSizeMB –** količina prostora na sistemskom disku u megabajtima.

  - **WindowsErrorReportingMachineId –** identifikator računala koji je uređaju na kojem se pokreće Office dodijelilo izvješćivanje o pogreškama u sustavu Windows.

  - **WindowsSqmMachineId –** identifikator računala koji je uređaju na kojem se pokreće Office dodijelio Windows.

### <a name="officesystemsystemhealthmetadatadeviceconsolidated"></a>Office.System.SystemHealthMetadataDeviceConsolidated

Metapodaci koji su potrebni za izoliranje reprodukcije pogreške.

Prikupljaju se sljedeća polja:

  - **BootDiskType –** disk ili solid-state pogon

  - **ComputerSystemProductUuidHash –** jednosmjerno raspršivanje UUID-a matične ploče.

  - **DeviceClass –** identifikator za vrstu uređaja na kojem se pokreće Office.

  - **DeviceManufacturer –** proizvođač uređaja na kojem je Office pokrenut.

  - **DeviceModel –** model uređaja na kojem je Office pokrenut.

  - **DeviceProcessorModel –** model procesora uređaja na kojem je Office pokrenut.

  - **DigitizerInfo –** podaci o digitalizatoru koji je priključen na uređaj na kojem je Office pokrenut.

  - **HasSpectreFix –** određuje ima li procesor uređaja na kojem se pokreće Office popravak za Spectre.

  - **IsLaptop –** označava je li uređaj na kojem je Office pokrenut prijenosno računalo.

  - **IsTablet –** označava je li uređaj na kojem je Office pokrenut tablet.

  - **MachineName –** naziv uređaja na kojem se Office pokreće.

  - **NumProcPhysCores –** broj fizičkih jezgri procesora.

  - **NumProcShareSingleCache –** broj procesora koji zajednički koriste jednu predmemoriju na uređaju na kojem se Office pokreće.

  - **NumProcShareSingleCore –** broj procesora po fizičkoj jezgri na uređaju na kojem se Office pokreće.

  - **Platform –** identifikator okruženja u kojem se Office pokreće.

  - **PowerPlatformRole –** identifikator preferirane uloge računala prema OEM-u za uređaj na kojem je Office pokrenut.

  - **powerPlatformRole –** identifikator preferirane uloge računala prema OEM-u za uređaj na kojem je Office pokrenut.

  - **ProcessorCount –** broj procesora na uređaju na kojem se Office pokreće.

  - **ProcSpeedMHz –** brzina procesora na uređaju na kojem se Office pokreće u megahercima.

  - **ProcType –** arhitektura procesora.

  - **ProcTypeText –** vrsta procesora na uređaju na kojem se Office pokreće.

  - **RamMB –** količina dostupnog RAM-a na uređaju na kojem je Office pokrenut.

  - **SusClientId –** ID za Windows Update uređaja na kojem se Office pokreće.

  - **SysVolFreeSpaceMB –** količina slobodnog prostora na sistemskom disku u megabajtima.

  - **SysVolSizeMB –** količina prostora na sistemskom disku u megabajtima.

  - **sysVolSizeMB –** količina prostora na sistemskom disku u megabajtima.

  - **WindowsErrorReportingMachineId –** identifikator računala koji je uređaju na kojem se pokreće Office dodijelilo izvješćivanje o pogreškama u sustavu Windows.

  - **WindowsSqmMachineId –** identifikator računala koji je uređaju na kojem se pokreće Office dodijelio Windows.

### <a name="officesystemsystemhealthmetadataoperatingsystem"></a>Office.System.SystemHealthMetadataOperatingSystem

Metapodaci koji su potrebni za izoliranje reprodukcije pogreške.

Prikupljaju se sljedeća polja:

  - **CollectionTime** – vrijeme kad je događaj stavljen u red čekanja za prijenos

  - **IsTerminalServer –** vrijednost true/false koja označava je li u pitanju klijent za terminalski poslužitelj

  - **OsBuild –** međuverzija operacijskog sustava.

  - **OsBuildRevision –** revizija međuverzije operacijskog sustava

  - **OSEnvironment** – Windows, iOS, Mac, Android itd.

  - **OsMajorVer –** glavna verzija operacijskog sustava.

  - **OsMinorVer –** sporedna verzija operacijskog sustava.

  - **OSSDKVersionCode** – identifikator verzije SDK-a operacijskog sustava.

  - **OsSku** – SKU operacijskog sustava

  - **OsSuite2** – identifikator paketa operacijskog sustava.

  - **OSVersionString** – identifikator verzije operacijskog sustava.

  - **ServicePackMajorVer** – glavna verzija servisnog paketa operacijskog sustava

  - **ServicePackMinorVer** – sporedna verzija servisnog paketa operacijskog sustava

### <a name="officesystemsystemhealthmetadataoperatingsystemdevice"></a>Office.System.SystemHealthMetadataOperatingSystemDevice

Metapodaci koji su potrebni za izoliranje reprodukcije pogreške.

Prikupljaju se sljedeća polja:

  - **CollectionTime** – vrijeme kad je događaj stavljen u red čekanja za prijenos

  - **DeviceClass –** identifikator za vrstu uređaja na kojem se pokreće Office.

  - **DeviceManufacturer –** proizvođač uređaja na kojem je Office pokrenut.

  - **DeviceModel –** model uređaja na kojem je Office pokrenut.

  - **DigitizerInfo –** podaci o digitalizatoru koji je priključen na uređaj na kojem je Office pokrenut.

  - **IsLaptop –** označava je li uređaj na kojem je Office pokrenut prijenosno računalo.

  - **IsTablet –** označava je li uređaj na kojem je Office pokrenut tablet.

  - **IsTerminalServer –** vrijednost true/false koja označava je li u pitanju klijent za terminalski poslužitelj

  - **MachineName –** naziv uređaja na kojem se Office pokreće.

  - **NumProcPhysCores –** broj fizičkih jezgri procesora.

  - **NumProcShareSingleCache –** broj procesora koji zajednički koriste jednu predmemoriju na uređaju na kojem se Office pokreće.

  - **NumProcShareSingleCore –** broj procesora po fizičkoj jezgri na uređaju na kojem se Office pokreće.

  - **OsBuild –** međuverzija operacijskog sustava.

  - **OsBuildRevision –** revizija međuverzije operacijskog sustava

  - **OSEnvironment** – Windows, iOS, Mac, Android itd.

  - **OsMajorVer –** glavna verzija operacijskog sustava.

  - **OsMinorVer –** sporedna verzija operacijskog sustava.

  - **OSSDKVersionCode** – identifikator verzije SDK-a operacijskog sustava.

  - **OsSku** – SKU operacijskog sustava

  - **OsSuite2** – identifikator paketa operacijskog sustava.

  - **OSVersionString** – identifikator verzije operacijskog sustava.

  - **Platform –** identifikator okruženja u kojem se Office pokreće.

  - **PowerPlatformRole –** identifikator preferirane uloge računala prema OEM-u za uređaj na kojem je Office pokrenut.

  - **ProcessorCount –** broj procesora na uređaju na kojem se Office pokreće.

  - **ProcSpeedMHz –** brzina procesora na uređaju na kojem se Office pokreće u megahercima.

  - **ProcTypeText –** vrsta procesora

  - **RamMB –** količina dostupnog RAM-a na uređaju na kojem je Office pokrenut.

  - **ServicePackMajorVer** – glavna verzija servisnog paketa operacijskog sustava

  - **ServicePackMinorVer** – sporedna verzija servisnog paketa operacijskog sustava

  - **SysVolFreeSpaceMB –** količina slobodnog prostora na sistemskom disku u megabajtima.

  - **SysVolSizeMB –** količina prostora na sistemskom disku u megabajtima.

### <a name="officesystemsystemhealthmetadataos"></a>Office.System.SystemHealthMetadataOS

Metapodaci koji su potrebni za izoliranje reprodukcije pogreške.

Prikupljaju se sljedeća polja:

  - **CountryRegion –** postavka identifikatora države/regije u operacijskom sustavu.

  - **HorizontalResolution –** vodoravna razlučivost zaslona

  - **IsTerminalServer –** vrijednost true/false koja označava je li u pitanju klijent za terminalski poslužitelj

  - **KeyboardLanguage –** identifikator jezika tipkovnice uređaja

  - **KeyboardLanguageTag –** identifikator jezika tipkovnice uređaja

  - **OfficeWvd –** određuje stanje u kojem se nalazi Windows Virtual Desktop.

  - **OsBuild –** međuverzija operacijskog sustava.

  - **OsBuildRevision –** revizija međuverzije operacijskog sustava

  - **OSEnvironment** – Windows, iOS, Mac, Android itd.

  - **OsLocale –** identifikator regionalne sheme operacijskog sustava.

  - **OsLocaleTag –** identifikator regionalne sheme operacijskog sustava.

  - **OsMajorVer –** glavna verzija operacijskog sustava.

  - **OsMinorVer –** sporedna verzija operacijskog sustava.

  - **OSSDKVersionCode** – identifikator verzije SDK-a operacijskog sustava.

  - **OsSku –** identifikator SKU-a operacijskog sustava.

  - **OsSuite2** – identifikator paketa operacijskog sustava.

  - **OsUiLang –** jezik korisničkog sučelja operacijskog sustava.

  - **OSVersionString** – identifikator verzije operacijskog sustava.

  - **ScreenDepth –** dubina zaslona

  - **ScreenDpi –** DPI zaslona

  - **ServicePackMajorVer** – glavna verzija servisnog paketa operacijskog sustava

  - **ServicePackMinorVer** – sporedna verzija servisnog paketa operacijskog sustava

  - **SystemLocale –** zadana regionalna shema operacijskog sustava

  - **SystemLocaleTag –** zadana regionalna shema operacijskog sustava

  - **TimeZoneBiasInMinutes –** razlika u minutama između lokalnog vremena i UTC-a.

  - **VerticalResolution –** okomita razlučivost zaslona

### <a name="officesystemsystemhealthmetadatascreencultureusersqmid"></a>Office.System.SystemHealthMetadataScreenCultureUserSqmId

Metapodaci koji su potrebni za izoliranje reprodukcije pogreške.

Prikupljaju se sljedeća polja:

  - **Alias –** pseudonim Microsoftova zaposlenika ili automatizirani pseudonim korisnika

  - **CID –** identitet korisnika u obliku pseudonima

  - **CollectibleClassifications -** Klasifikacije podataka koje se mogu prikupljati u skladu s postavkama zaštite privatnosti klijenta

  - **CollectionTime** – vrijeme kad je događaj stavljen u red čekanja za prijenos

  - **CountryRegion –** postavka identifikatora države/regije u operacijskom sustavu.

  - **DomainName –** naziv Microsoftove domene

  - **HorizontalResolution –** vodoravna razlučivost zaslona

  - **IntegratedScreenSize –** veličina integriranog zaslona.

  - **IsJoinedToDomain –** vrijednost true/false koja označava je li klijent pridružen domeni

  - **IsLabMachine –** određuje je li u pitanju računalo iz Microsoftova laboratorija za testiranje

  - **IsMsftInternal –** vrijednost true/false koja označava je li računalo na Microsoftovoj poslovnoj domeni

  - **IsSubscription –** označava je li aplikacija sustava Office instalirana pod pretplatničkom licencom.

  - **KeyboardLanguage –** identifikator jezika tipkovnice uređaja

  - **KeyboardLanguageTag –** identifikator jezika tipkovnice uređaja

  - **OsLocale –** identifikator regionalne sheme operacijskog sustava.

  - **OsLocaleTag –** identifikator regionalne sheme operacijskog sustava.

  - **OsUiLang –** jezik korisničkog sučelja operacijskog sustava.

  - **ScreenDepth –** dubina zaslona

  - **ScreenDpi –** DPI zaslona

  - **ScreenXDpi –** X DPI zaslona

  - **ScreenYDpi –** Y DPI zaslona

  - **SqmUserId –** nasumični identifikator instalacije sustava Office.

  - **StudyId –** identifikator u ispitivanju Software Quality Metrics.

  - **SystemLocale –** zadana regionalna shema operacijskog sustava

  - **SystemLocaleTag –** zadana regionalna shema operacijskog sustava

  - **TimeZoneBiasInMinutes –** razlika u minutama između lokalnog vremena i UTC-a.

  - **VerticalResolution –** okomita razlučivost zaslona

  - **WinUserActType –** označava je li korisnik sustava Windows koji pokreće Office lokalni administrator, napredni korisnik ili normalni korisnik.

### <a name="officesystemsystemhealthofficelensidentity"></a>Office.System.SystemHealthOfficeLensIdentity

Podaci o identitetu korisnika koji su potrebni za ispunjavanje zahtjeva ispitanika.

Prikupljaju se sljedeća polja:

  - **CID –** identitet korisnika u obliku pseudonima

### <a name="officesystemsystemhealthrollbacksessionmetadata"></a>Office.System.SystemHealthRollbackSessionMetadata

Metapodaci koji su potrebni za izoliranje reprodukcije pogreške.

Prikupljaju se sljedeća polja:

  - **InstallMethod** – nova instalacija, ažuriranje ili vraćanje

  - **IsSubscription –** označava je li aplikacija sustava Office instalirana pod pretplatničkom licencom.

  - **PreviousBuild** – prethodno instalirana međuverzija

### <a name="officesystemsystemhealthsessionlifecycleandheartbeat"></a>Office.System.SystemHealthSessionLifecycleAndHeartbeat

Sadrži informacije o metrici stanja sustava.

Prikupljaju se sljedeća polja:

  - **InstallMethod** – određuje je li sustav nadograđen na trenutnu instalaciju sustava Office, vraćen na nju ili je u pitanju nova instalacija.

  - **InteractionSessionID** – identifikator sesije.

  - **PreviousBuild** – verzija sustava Office na koju je međuverzija nadograđena ili s koje je vraćene.

  - **State** – stanje u koje je sesija promijenjena.

  - **Time** – upućuje na vrijeme kad je promijenjeno stanje sesije.

### <a name="officesystemsystemhealthsessionstarttime"></a>Office.System.SystemHealthSessionStartTime

Koristi se s podacima o rušenju za odvajanje ranih i kasnih rušenja (tj. za utvrđivanje je li korisnik neko vrijeme upotrebljavao aplikaciju prije nego što se srušila)

Prikupljaju se sljedeća polja:

  - **SessionStart** – vrijeme kad telemetrija počinje obrađivati podatke.

### <a name="officesystemsystemhealthungracefulappexitdesktop"></a>Office.System.SystemHealthUngracefulAppExitDesktop

Događaj se aktivira nenormalnim zatvaranjem aplikacije (npr. zaustavljanje u upravitelju zadataka, smrzavanje aplikacije itd.) za klijentske aplikacije sustava Office kao što su, među ostalima, Word, Excel, PowerPoint i Outlook. Za mjerenje stanja klijentskih proizvoda sustava Office koristimo metriku nekontroliranog zatvaranja aplikacije. To je signal ključan za poslovanje kojim se inženjeri sustava Office koriste za postizanje stabilnosti proizvoda.

Prikupljaju se sljedeća polja:

  - **AffectedProcessAppBuild –** identifikator međuverzije zahvaćenog procesa.

  - **AffectedProcessAppBuildRevision –** identifikator revizije međuverzije zahvaćenog procesa.

  - **AffectedProcessAppMajorVer** – identifikator radne verzije zahvaćenog procesa.

  - **AffectedProcessAppMinorVer –** identifikator sporedne verzije zahvaćenog procesa.

  - **AffectedProcessAppName –** naziv zahvaćenog procesa. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **AffectedProcessExeBuildVersion –** broj međuverzije zahvaćenog procesa. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **AffectedProcessExeMajorVersion –** broj glavne verzije zahvaćenog procesa. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **AffectedProcessExeMinorVersion –** broj radne verzije zahvaćenog procesa. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **AffectedProcessExeRevisionVersion –** broj revizije međuverzije zahvaćenog procesa. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **AffectedProcessIsDebug –** određuje je li međuverzija zahvaćenog procesa verzija za ispravljanje pogrešaka. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **AffectedProcessIsLabMachine –** određuje nalazi li se zahvaćeni proces u Microsoftovu laboratoriju. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **AffectedProcessOsEnvironment –** identifikator operacijskog sustava za zahvaćeni proces. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **AppName –** naziv zahvaćene aplikacije. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **CrashedAssignedFlights –** testne verzije dodijeljene procesu koji je pao. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **CrashedConfigIds –** konfiguracija dodijeljena procesu koji je pao. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **CrashedEcsETag –** identifikator eksperimenta za srušeni proces.

  - **CrashedImpressionId –** identifikator prikaza srušenog procesa. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **CrashedModuleName –** naziv neispravnog modula.

  - **CrashedProcessSessionID –** jedinstveni identifikator srušenog procesa. 

  - **CrashedProcessSessionInitTime –** vrijeme pokretanja zahvaćenog procesa. 

  - **CrashedProcessSessionUninitTime** – vrijeme završetka zahvaćenog procesa.

  - **CrashTag** – jedinstveni identifikator kôda pada sustava.

  - **CrashType –** identifikator grupiranja za vrstu rušenja.

  - **DetectionTime –** vrijeme otkrivanja neočekivanog zatvaranja. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **ErrorString –** opis pogreške. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **ExceptionAddress –** adresa u programu na kojoj je došlo do pogreške. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **ExceptionCode –** identifikator grupiranja za iznimku.

  - **FaultAppName –** naziv aplikacije s pogreškom. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **InstallMethod** – određuje je li sustav nadograđen na trenutnu međuverziju sustava Office, vraćen na nju ili je u pitanju nova instalacija.

  - **InstallType –** identifikator metode kojom je Office instaliran. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **InstallTypeName –** identifikator metode kojom je Office instaliran. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **IsLabMachine –** određuje pokreće li se Office u Microsoftovu laboratoriju. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **IsMsftInternal –** označava je li korisnik sustava Windows koji pokreće Office Microsoftov zaposlenik. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **ModuleBaseAddress –** osnovna adresa neispravnog modula. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **ModuleBuildVersion –** broj međuverzije neispravnog modula. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **ModuleMajorVersion –** broj glavne verzije neispravnog modula. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **ModuleMinorVersion –** broj radne verzije neispravnog modula. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **ModuleName –** naziv neispravnog modula. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **ModuleOffset –** pomak u bajtovima (u heksadecimalnom obliku) od osnovne adrese na kojem je došlo do pogreške.

  - **ModuleRevisionVersion –** broj revizije međuverzije neispravnog modula. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **ModuleSize –** veličina neispravnog modula u bajtovima. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **ModuleVersion** – verzija neispravnog modula odgovornog za pad sustava.

  - **OfficeArchitectureText** – arhitektura instalacije: x64, x86 itd.

  - **OfficeUILang** – jezik korisničkog sučelja u međuverziji sustava Office.

  - **OSEnvironment –** identifikator okruženja u kojem je Office pokrenut.

  - **PreviousBuild** – prethodno instalirana međuverzija

  - **ProcessorArchitecture** – arhitektura procesora u okruženju: x64, x86 itd.

  - **SessionFlags** – određuje uvjete sesije, kao npr. je li datoteka bila otvorena ili se uređivala, je li otvoren dokument u oblaku, je li postupak pokretanja dovršen itd. 

  - **UAETypeName –** identifikator grupiranja načina na koji se aplikacija nekontrolirano zatvorila. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **UninitLibletId** – jedinstveni identifikator za neispravnu komponentu u okviru pada sustava.

  - **VerifyElseCrashTag –** jedinstveni identifikator mjesta na kojem se aplikacija srušila. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

### <a name="officesystemsystemhealthungracefulappexitimmersive"></a>Office.System.SystemHealthUngracefulAppExitImmersive

Koristi se za snimanje metrike rušenja.

Prikupljaju se sljedeća polja:

  - **AffectedProcessAppBuild –** identifikator međuverzije zahvaćenog procesa.

  - **AffectedProcessAppBuildRevision –** identifikator revizije međuverzije zahvaćenog procesa.

  - **AffectedProcessAppMajorVer –** identifikator glavne verzije zahvaćenog procesa.

  - **AffectedProcessAppMinorVer –** identifikator sporedne verzije zahvaćenog procesa.

  - **AffectedProcessAppName –** naziv zahvaćenog procesa.

  - **AffectedProcessExeBuildVersion –** broj međuverzije zahvaćenog procesa.

  - **AffectedProcessExeMajorVersion –** broj glavne verzije zahvaćenog procesa.

  - **AffectedProcessExeMinorVersion –** broj sporedne verzije zahvaćenog procesa.

  - **AffectedProcessExeRevisionVersion –** broj revizije međuverzije zahvaćenog procesa.

  - **AffectedProcessIsDebug –** određuje je li međuverzija zahvaćenog procesa verzija za ispravljanje pogrešaka.

  - **AffectedProcessIsLabMachine –** određuje nalazi li se zahvaćeni proces u Microsoftovu laboratoriju.

  - **AffectedProcessOsEnvironment –** identifikator operacijski sustav za zahvaćeni proces.

  - **AppName –** naziv zahvaćene aplikacije.

  - **CrashedAssignedFlights –** testne verzije dodijeljene srušenom procesu.

  - **CrashedConfigIds –** konfiguracija dodijeljena srušenom procesu.

  - **CrashedImpressionId –** identifikator prikaza srušenog procesa.

  - **CrashedInteractionSessionID –** identifikator sesije interakcije za zahvaćeni proces.

  - **CrashedInteractionSessionTime –** vrijeme kada je bila moguća interakcija sa zahvaćenim procesom.

  - **CrashedProcessSessionID –** jedinstveni identifikator srušenog procesa.

  - **CrashedProcessSessionInitTime –** vrijeme pokretanja zahvaćenog procesa.

  - **DetectionTime –** vrijeme otkrivanja neočekivanog zatvaranja.

  - **IsLabMachine –** određuje pokreće li se Office u Microsoftovu laboratoriju.

  - **IsMsftInternal –** označava je li korisnik sustava Windows koji pokreće Office Microsoftov zaposlenik.

  - **OSEnvironment –** identifikator okruženja u kojem je Office pokrenut.

  - **PreviousLifecycleState –** stanje zahvaćenog procesa kad se srušio.

  - **UAETypeName –** identifikator grupiranja načina na koji se aplikacija neočekivano zatvorila.

### <a name="officesystemsystemhealthungracefulapplicationexitwin32"></a>Office.System.SystemHealthUngracefulApplicationExitWin32

Događaj aktivira nenormalno ukidanje aplikacije (npr. zaustavljanje u upravitelju zadataka, prekid aplikacije, itd.) za klijentske aplikacije sustava Office, kao što su, no ne ograničavajući se na, Word, Excel, PowerPoint i Outlook. Parametre neočekivanog zatvaranja aplikacije koristimo za mjerenje stanja proizvoda klijenata sustava Office. To je signal ključan za poslovanje koji inženjeri sustava Office koriste za postizanje stabilnosti proizvoda.

Prikupljaju se sljedeća polja:

  - **AddinExecution** – zastavica koja obavještava je li se dodatak izvršavao, a nije završio s radom prilikom nekontroliranog izlaska iz aplikacije. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **AppUsedVirtualMemory** – virtualna memorija koju aplikacija sustava Office koristi

  - **BootCompleted** – je li u trenutku pada pokretanje sustava Office bilo dovršeno. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **BucketId** – identifikator pada za grupiranje u servisu Watson
 
  - **CabGuid** – globalno jedinstven identifikator (GUID) za cab servisa Watson.

  - **CrashedAppBuild** – identifikator međuverzije zahvaćenog procesa. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **CrashedAppMajor** – identifikator glavne verzije zahvaćenog procesa. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*
 
  - **CrashedAppMinor** – identifikator radne verzije zahvaćenog procesa. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **CrashedAppVersion** – identifikator verzije aplikacije za proces koji je pao.

  - **CrashedEcsETag** – identifikator eksperimenta za proces koji je pao.

  - **CrashedModuleName** – naziv neispravnog modula.

  - **CrashedProcessSessionId** – jedinstveni identifikator procesa koji je pao.

  - **CrashedProcessSessionInitTime** – vrijeme pokretanja zahvaćenog procesa.

  - **CrashedProcessSessionUninitTime** – vrijeme završetka zahvaćenog procesa.

  - **CrashTag** – jedinstveni identifikator kôda pada sustava.

  - **CrashTime** – vrijeme koje označava da je klijent nekontrolirano zatvoren. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **CrashType** – identifikator grupiranja za vrstu pada.

  - **DetectionTime** – vrijeme otkrivanja nekontroliranog zatvaranja. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **ExceptionAddress** – adresa u programu na kojoj je došlo do pogreške. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **ExceptionCode** – identifikator grupiranja za iznimku.

  - **ExceptionInfo** – informacije o sustavu za iznimku.

  - **HandOff** – je li korisnik stvorio i predao Officeov proces novoj sesiji. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **HangTypeCode** – predstavlja klasu pada ako je proces pao tijekom izvršavanja.

  - **HasEdit** – je li korisnik uređivao dokument u klijentu koji je pao. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **HasOpen** – je li u klijentu koji je pao bio otvoren dokument. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **HexCrashTag** – jedinstveni identifikator kôda pada sustava. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **HexExceptionAddress** – heksadecimalni oblik adrese u programu na kojoj je došlo do pogreške. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **HexExceptionCode** – heksadecimalni identifikator grupiranja za iznimku. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **HexModuleBaseAddress** – osnovna adresa neispravnog modula u heksadecimalnom obliku. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **HexModuleOffset** – pomak u bajtovima (u heksadecimalnom obliku) od osnovne adrese na kojem je došlo do pogreške. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **HexModuleSize** – veličina neispravnog modula u bajtovima u heksadecimalnom obliku. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **HexVerifyElseCrashTag** – jedinstveni identifikator mjesta pada aplikacije u heksadecimalnom obliku. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **InstallMethod** – određuje je li sustav nadograđen na trenutačnu međuverziju sustava Office, vraćen na nju ili je u pitanju nova instalacija.

  - **IsLabMachine** – određuje pokreće li se Office u Microsoftovu laboratoriju. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **ModuleBaseAddress** – osnovna adresa neispravnog modula. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **ModuleOffset** – pomak u bajtovima (u heksadecimalnom obliku) od osnovne adrese na kojem je došlo do pogreške.

  - **ModuleSize** – veličina neispravnog modula u bajtovima. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **ModuleStamp** – oznaka neispravnog modula.

  - **ModuleVersion** – verzija neispravnog modula odgovornog za pad sustava.

  - **OfficeArchitectureText** – arhitektura proizvoda sustava Office predstavljena kao niz (npr. x86, arm).

  - **OfficeUILang** – jezik korisničkog sučelja u međuverziji sustava Office.

  - **PreviousBuild** – prethodno instalirana međuverzija

  - **ProcessorArchitecture** – arhitektura procesora u okruženju: x64, x86 itd.

  - **SafeMode** – je li sesija bila pokrenuta u sigurnom načinu rada. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **SessionFlags** – određuje uvjete sesije, kao npr. je li datoteka bila otvorena ili se uređivala, je li otvoren dokument u oblaku, je li postupak pokretanja dovršen itd. 

  - **StackHash** – omogućuje raspršeni ID za stog kvara u sustavu Office.

  - **SystemAvailableMemory**  – dostupna memorija u operacijskom sustavu

  - **UAEOSEnvironment** – identifikator okruženja operacijskog sustava. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **UninitLibletId** – jedinstveni identifikator za neispravnu komponentu u okviru pada sustava.

  - **VerifyElseCrashTag** – jedinstveni identifikator mjesta pada aplikacije. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali će se možda i dalje pojavljivati u starijim međuverzijama.]*

  - **WatsonReportId** – identifikator izvješća poslanog Windows servisu Watson.

  - **WerEventCreatedTime** – vremenska oznaka događaja izvješćivanja o pogreškama u sustavu Windows.


### <a name="officesystemungracefulapplicationexitdesktopappexit"></a>Office.System.UngracefulApplicationExit.DesktopAppExit

Koristi se za snimanje metrike rušenja.

Prikupljaju se sljedeća polja:

  - **AppBuildVersion –** identifikator međuverzije zahvaćenog procesa.

  - **AppMajorVersion –** broj glavne verzije zahvaćenog procesa.

  - **AppMinorVersion –** identifikator sporedne verzije zahvaćenog procesa.

  - **AppName –** naziv zahvaćene aplikacije.

  - **AppRevisionVersion –** identifikator revizije međuverzije zahvaćenog procesa.

  - **CrashedAssignedFlights –** testne verzije dodijeljene srušenom procesu.

  - **CrashedConfigIds –** konfiguracija dodijeljena srušenom procesu.

  - **CrashedImpressionId –** identifikator prikaza srušenog procesa.

  - **CrashedInteractionSessionId –** identifikator sesije interakcije za proces koji se srušio.

  - **CrashedProcessSessionId –** jedinstveni identifikator srušenog procesa.

  - **CrashType –** identifikator grupiranja za vrstu rušenja.

  - **ErrorString –** opis pogreške.

  - **ExceptionAddress –** adresa u programu na kojoj je došlo do pogreške.

  - **ExceptionCode –** identifikator grupiranja za iznimku.

  - **FaultAppName –** naziv aplikacije s pogreškom.

  - **InstallMethod** – određuje je li sustav nadograđen na trenutnu međuverziju sustava Office, vraćen na nju ili je u pitanju nova instalacija.

  - **InstallType –** identifikator metode kojom je Office instaliran.

  - **IsDebug –** označava radi li se o međuverziji sustava Office za ispravljanje pogrešaka.

  - **IsHandledCrash –** određuje je li u sesiji koja se srušila aktiviran rukovatelj rušenja.

  - **IsLabMachine –** određuje pokreće li se Office u Microsoftovu laboratoriju.

  - **ModuleBaseAddress –** osnovna adresa neispravnog modula.

  - **ModuleName –** naziv neispravnog modula.

  - **ModuleOffset –** pomak u bajtovima od osnovne adrese na kojoj je došlo do pogreške.

  - **ModuleSize –** veličina neispravnog modula u bajtovima.

  - **OSEnvironment –** identifikator okruženja u kojem je Office pokrenut.

  - **PreviousBuild** – prethodno instalirana međuverzija

  - **PreviousInteractionSessionTime –** vrijeme pokretanja prethodne sesije interakcije.

  - **PreviousLifecycleState –** identifikator stanja životnog ciklusa prethodne sesije.

  - **PreviousSessionInitTime –** vrijeme pokretanja prethodne sesije.

  - **StackHash –** identifikator koji označava gdje se u kodu zahvaćeni proces srušio.

  - **VerifyElseCrashTag –** jedinstveni identifikator mjesta na kojem se aplikacija srušila.

### <a name="officesystemuserchangeddiagnosticlevel"></a>Office.System.UserChangedDiagnosticLevel

Provode se podaci koji su potrebni da bi se osigurali korisnikovi odabiri iz pravila zaštite privatnosti.

Prikupljaju se sljedeća polja:

  - **DiagnosticLevelChanged**: označava da je korisnik promijenio razinu dijagnostike.

  - **NewDiagnosticLevel**: razina nakon korisnikove promjene.

  - **OldDiagnosticLevel**: razina koju je korisnik upotrebljavao prije promjena.

### <a name="officetelemetryariaeventsinkhandlemsadevicetokenresponse"></a>Office.Telemetry.AriaEventSink.HandleMsaDeviceTokenResponse

Signal prekida isporuke servisa Microsoftova računa.

Prikupljaju se sljedeća polja:

  - **RetryCount** – broj ponovnih pokušaja povezivanja sa servisom MSA.

### <a name="officetelemetryariaeventsinkrequestmsadevicetoken"></a>Office.Telemetry.AriaEventSink.RequestMsaDeviceToken

Signal prekida isporuke servisa Microsoftova računa.

Prikupljaju se sljedeća polja:

  - **RetryCount** – broj ponovnih pokušaja povezivanja sa servisom Microsoftova računa.

### <a name="officetelemetryclientsamplingoverridden"></a>Office.Telemetry.ClientSamplingOverridden

Potrebno da bi se stope reprodukcije točno izračunale. Obično se ne odnosi na produkcijsku ciljnu skupinu.

Prikupljaju se sljedeća polja:

  - **OverriddenMeasureEnabled** – određuje je li klijent postavljen tako da šalje više od neuzorkovanih događaja

  - **OverriddenNumberlinePosition** – novi položaj u retku brojeva za uzorkovanje

  - **OverriddenReportedSampleRate** – novoprijavljena stopa uzorkovanja

  - **OverriddenSampleRate** – nova stopa uzorkovanja

  - **PreviousNumberlinePosition** položaj uzorkovanja u retku brojeva

  - **PreviousSampleRate** – stopa uzorkovanja prije nadjačavanja.

  - **WasMeasureEnabled** – određuje je li klijent postavljen tako da šalje više od neuzorkovanih događaja

### <a name="officetelemetrycomplianceeventnotinbasicallowlist"></a>Office.Telemetry.Compliance.EventNotInBasicAllowList

Prijavljuje implementacije ili provedbe telemetrije koje nisu valjane

Prikupljaju se sljedeća polja:

  - **EventName** – naziv događaja koji nije na popisu

### <a name="officetelemetrycompliancemissingdatacategory"></a>Office.Telemetry.Compliance.MissingDataCategory

Prijavljuje implementacije ili provedbe telemetrije koje nisu valjane

Prikupljaju se sljedeća polja:

  - **EventName** – naziv događaja za koji nije određena kategorija

  - **IsFromRule** – određuje potječe li događaj iz pravila telemetrije

### <a name="officetelemetrycompliancemissingdatacategoryinrule"></a>Office.Telemetry.Compliance.MissingDataCategoryInRule

Prijavljuje implementacije ili provedbe telemetrije koje nisu valjane

Prikupljaju se sljedeća polja:

  - **RuleId** –ID pravila za koje nije određena kategorija podataka

  - **RuleVersion** – verzija pravila za koje nije određena kategorija podataka

### <a name="officetelemetrydiagnosticdataviewerstatechanged"></a>Office.Telemetry.DiagnosticDataViewerStateChanged

Provjerava mogu li korisnici vidjeti podatke dok odlaze s njihova računala pomoću preglednika dijagnostičkih podataka.

Prikupljaju se sljedeća polja:

  - **DialogCancelled** –određuje je li dijaloški okvir preglednika dijagnostičkih podataka otkazan

  - **NewState** – novo stanje preglednika dijagnostičkih podataka

  - **WasDialogUsed** –određuje je li dijaloški okvir preglednika dijagnostičkih podataka korišten

### <a name="officetelemetrydynamicconfigfetchconfigs"></a>Office.Telemetry.DynamicConfig.FetchConfigs

Podaci potrebni za mjerenje stanja servisa za konfiguraciju telemetrije.

Prikupljaju se sljedeća polja:

  - **ParsedConfigCount** – broj raščlanjenih dinamičkih konfiguracija

  - **ParsedConfigs** – broj raščlanjenih dinamičkih konfiguracija

  - **RejectedConfigCount** – broj odbijenih konfiguracija

  - **RejectedConfigs** – broj odbijenih konfiguracija

  - **RejectedConfigsList** – popis odbijenih konfiguracija razdvojenih zarezom.

### <a name="officetelemetrydynamicconfigparsejsonconfig"></a>Office.Telemetry.DynamicConfig.ParseJsonConfig

Podaci potrebni za mjerenje stanja servisa za konfiguraciju telemetrije

Prikupljaju se sljedeća polja:

  - **ErrorMessage** – poruka o pogrešci s raščlanjivanjem

  - **NodeName** – čvor koji se nije uspio raščlaniti

### <a name="officetelemetrydynamicconfigpopulatedrequestignored"></a>Office.Telemetry.DynamicConfig.PopulatedRequestIgnored

Taj se događaj generira kada ne postavimo kanal telemetrijske konfiguracije.

Događaj ne prikuplja nijedno polje.

### <a name="officetelemetrydynamicconfigpopulatetreecalledagain"></a>Office.Telemetry.DynamicConfig.PopulateTreeCalledAgain

Podaci potrebni za mjerenje stanja servisa za konfiguraciju telemetrije.

Događaj ne prikuplja nijedno polje.

### <a name="officetelemetryeventquarantined"></a>Office.Telemetry.EventQuarantined

Koristili se za potvrđivanje funkcioniraju li događaji NSD-a pravilno.

Prikupljaju se sljedeća polja:

  - **EventName** – naziv događaja stavljenog u karantenu

  - **Reason** – razlog stavljanja u karantenu

### <a name="officetelemetryflusheventbuffer"></a>Office.Telemetry.FlushEventBuffer 

Prijavljuje veličinu međuspremnika događaja te može upućivati na pogreške telemetrije povezane s velikim međuspremnikom.

Prikupljaju se sljedeća polja:

  - **EventCount** – broj događaja u međuspremniku

  - **FirstPassCount** – broj događaja u prvom prolazu

  - **SecondPassCount** – broj događaja u drugom prolazu

### <a name="officetelemetrygetfilteredpayloadsfromdisk"></a>Office.Telemetry.GetFilteredPayloadsFromDisk

Provjerava funkcioniraju li određeni dijelovi naslijeđenog kanala za telemetriju na platformama koje ga još koriste.

Događaj ne prikuplja nijedno polje.

### <a name="officetelemetryinvaliddatacontractname"></a>Office.Telemetry.InvalidDataContractName

Prijavljuje implementacije ili provedbe telemetrije koje nisu valjane

Prikupljaju se sljedeća polja:

  - **DataContractName** – naziv ugovora o telemetrijskim podacima

  - **EventName** –naziv događaja za koji ugovor o podacima nije valjan

  - **IsRuleEvent** – vrijednost true/false je li događaj implementiran telemetrijskim pravilom

### <a name="officetelemetryinvaliddatafieldname"></a>Office.Telemetry.InvalidDataFieldName 

Prijavljuje implementacije ili provedbe telemetrije koje nisu valjane

Prikupljaju se sljedeća polja:

  - **DataFieldName** – naziv polja telemetrijskih podataka

  - **EventName** –-naziv događaja koji sadrži polje koje nije valjano

  - **IsRuleEvent** – vrijednost true/false je li događaj implementiran telemetrijskim pravilom.

### <a name="officetelemetryinvalideventcontractname"></a>Office.Telemetry.InvalidEventContractName 

Prijavljuje implementacije ili provedbe telemetrije koje nisu valjane

Prikupljaju se sljedeća polja:

  - **EventContractName** –naziv ugovora o telemetriji koji nije valjan

  - **EventName** –naziv događaja za koji naziv ugovora nije valjan

  - **IsRuleEvent** – vrijednost true/false je li događaj implementiran telemetrijskim pravilom

### <a name="officetelemetryloadxmlrules"></a>Office.Telemetry.LoadXmlRules

Prijavljuje je li raščlanjivanje telemetrijskih pravila uspjelo

Prikupljaju se sljedeća polja:

  - **DetachedDuration** – odvojeno trajanje u mikrosekundama

### <a name="officetelemetrymissingfielddetails"></a>Office.Telemetry.MissingFieldDetails

Prijavljuje podatke u poljima koji nedostaju radi dijagnosticiranja pogreška u pisanju konfiguracije telemetrije.

Prikupljaju se sljedeća polja:

  - **ErrorRuleId** – ID telemetrijskog pravila koje je zatražilo polje koje nedostaje

  - **ErrorRuleVersion** – verzija telemetrijskog pravila koje je zatražilo polje koje nedostaje

  - **EtwEventGuid** – GUID ETW-a zatraženog polja

  - **EtwEventGuid** – ID događaja ETW-a zatraženog polja

  - **MissingFieldName** – naziv zatraženog polja

  - **UlsTagId** – oznaka koda polja koje nedostaje

### <a name="officetelemetryprocessidlequeuejob"></a>Office.Telemetry.ProcessIdleQueueJob

Prijavljuje da je obrada telemetrije u neaktivnom stanju započela na očekivani način.

Prikupljaju se sljedeća polja:

  - **DetachedDuration** – odvojeno trajanje u mikrosekundama

  - **FailureDiagnostic** – operacija koja nije uspjela

### <a name="officetelemetryredstoneinboxsampling"></a>Office.Telemetry.RedstoneInboxSampling

Stanje uzorkovanja klijenta koje je potrebno da bi se točno protumačila ostala metrika.

Prikupljaju se sljedeća polja:

  - **MeasuresEnabled** – određuje jesu li u ovoj sesiji omogućene mjere?

  - **SamplingClientIdValue** – vrijednost uzorkovanja za ovaj klijent

  - **SamplingKey** – ključ uzorkovanja za ovaj klijent

  - **SamplingMethod** – metoda uzorkovanja za ovaj klijent

### <a name="officetelemetryredstoneinboxsamplingcritical"></a>Office.Telemetry.RedstoneInboxSamplingCritical

Stanje uzorkovanja klijenta može biti potrebno da bi se točno protumačila ostala metrika.

Prikupljaju se sljedeća polja:

  - **MeasuresEnabled** – određuje jesu li u ovoj sesiji omogućene mjere?

  - **SamplingClientIdValue** – vrijednost uzorkovanja za ovaj klijent

  - **SamplingKey** – ključ uzorkovanja za ovaj klijent

  - **SamplingMethod** – metoda uzorkovanja za ovaj klijent

### <a name="officetelemetryruleerrorsaggregated"></a>Office.Telemetry.RuleErrorsAggregated

Prijavljivanje pogrešaka u stanju telemetrije. Obavezno za provjeru valjanosti ostalih podataka (uključujući NSD).

Prikupljaju se sljedeća polja:

  - **ErrorCount** – broj pogreške u skupnom vremenskom razdoblju

  - **ErrorInfo** – informativni broj za dijagnostiku pogreške

  - **ErrorRuleId** – ID telemetrijskog pravila koje je uzrokovalo pogrešku

  - **ErrorRuleVersion** – verzija telemetrijskog pravila koje je uzrokovalo pogrešku

  - **WarningInfo** – informativni broj za dijagnostiku pogreške

  - **QueueFlushCount** – broj čišćenja reda čekanja

  - **QueueFlushDueToSizeLimit** – veličini pri kojoj telemetrija čisti red čekanja

  - **QueueFlushesDueToSize** – broj čišćenja reda čekanja uzrokovanih veličinom međuspremnika

  - **QueueHardLimit** – ograničenje za isključivanje telemetrije

  - **QueueLimitHitTime** – vrijeme dostizanja ograničenja za isključivanje

  - **ResultTime** – vrijeme događaja

### <a name="officetelemetryrulesenginediskthrottled"></a>Office.Telemetry.RulesEngineDiskThrottled

Metrika ograničavanja DQ-a. Potrebna za vjerodostojnost svih ostalih podataka.

Prikupljaju se sljedeća polja:

  - **DiskWriteLimit** – ograničenje veličine diska za telemetrijske podatke

  - **DiskWriteTotal** – ukupan prostor zapisivanja na disk za telemetrijske podatke

  - **SessionDiskWriteTotal** – ukupan prostor zapisivanja na disk tijekom sesije za telemetrijske podatke

  - **ThrottlingTimestamp** – vrijeme ograničavanja sesije

### <a name="officetelemetryrulesenginemediumcostthrottled"></a>Office.Telemetry.RulesEngineMediumCostThrottled

Metrika ograničavanja DQ-a. Potrebna za vjerodostojnost svih ostalih podataka.

Događaj ne prikuplja nijedno polje.

### <a name="officetelemetryrulesenginespikethrottled"></a>Office.Telemetry.RulesEngineSpikeThrottled

Metrika ograničavanja DQ-a. Potrebna za vjerodostojnost svih ostalih podataka.

Prikupljaju se sljedeća polja:

  - **CurrentLimit** –-trenutno ograničenje naglog porasta

  - **Trajanje** – trajanje naglog porasta

  - **Factor** – faktor naglog porasta

  - **HighestImpactingRuleBytes** – najveći broj bajtova koje je telemetrijsko pravilo zabilježilo

  - **HighestImpactingRuleId** – ID pravila koje je zabilježilo najviše bajtova

  - **HighestImpactingRuleVersion** – verzija pravila koje je zabilježilo najviše bajtova

  - **MaxLimit** – maksimalno ograničenje

  - **ThrottlingTimestamp** – vrijeme ograničavanja telemetrije

### <a name="officetelemetryrulesenginethrottled"></a>Office.Telemetry.RulesEngineThrottled

Metrika ograničavanja DQ-a. Potrebna za vjerodostojnost svih ostalih podataka.

Prikupljaju se sljedeća polja:

  - **ThrottlingTimestamp** – vrijeme ograničavanja telemetrije

### <a name="officetelemetryrulesengineulsqueuesizebackgroundprocessinglevelreached"></a>Office.Telemetry.RulesEngineUlsQueueSizeBackgroundProcessingLevelReached

Prijavljuje da u redu čekanja postoji previše događaja da bi se obradili tijekom neaktivnosti aplikacije.

Prikupljaju se sljedeća polja:

  - **BackgroundProcessingLevelInBytes** –veličina reda čekanja pri kojoj se pokreće obrada u pozadini.

  - **CurrentQueueSize** – broj događaja u redu čekanja nULS.

  - **CurrentQueueSizeInBytes** – veličina reda čekanja nULS u bajtovima.

  - **ReachedTimestamp** – vrijeme početka obrade u pozadini.

### <a name="officetelemetryrulesresultuploadlatencyrule"></a>Office.Telemetry.RulesResultUploadLatencyRule

Prosječno, minimalno i maksimalno kašnjenje prijenosa rezultata pravila uz prijenos opterećenja svakog sata

Prikupljaju se sljedeća polja:

  - **AverageLatency** – prosječno kašnjenje prijenosa.

  - **CollectionTime** – vrijeme prikupljanja podataka o prijenosu pravila.

  - **LatencyGE201LE400** – broj prijenosa čije je kašnjenje veće od 201 ms ili jednako tome, a manje od 400 ms ili jednako tome

  - **LatencyGE3001** – broj prijenosa čije je kašnjenje veće od 3001 ms ili jednako tome.

  - **LatencyGE401LE600** – broj prijenosa čije je kašnjenje veće od 401 ms ili jednako tome, a manje od 600 ms ili jednako tome

  - **LatencyGE601LE800** – broj prijenosa čije je kašnjenje veće od 601 ms ili jednako tome, a manje od 800 ms ili jednako tome

  - **LatencyLE200** – broj prijenosa čije je kašnjenje manje od 200 ms.

  - **MaxLatency** – najveće zabilježeno kašnjenje.

  - **MinLatency** – najmanje zabilježeno kašnjenje.

### <a name="officetelemetrysamplingpolicy"></a>Office.Telemetry.SamplingPolicy

Stanje uzorkovanja klijenta koje je potrebno da bi se točno protumačila ostala metrika.

Prikupljaju se sljedeća polja:

  - **MeasuresEnabled** – određuje jesu li u ovoj sesiji omogućene mjere?

  - **SamplingClientIdValue** – vrijednost uzorkovanja za ovaj klijent

  - **SamplingKey** – ključ uzorkovanja za ovaj klijent

  - **SamplingMethod** – metoda uzorkovanja za ovaj klijent

### <a name="officetelemetrysamplingpolicyeventtrigger"></a>Office.Telemetry.SamplingPolicyEventTrigger

Stanje uzorkovanja klijenta koje je potrebno da bi se točno protumačila ostala metrika.

Prikupljaju se sljedeća polja:

  - **MeasuresEnabled** – određuje jesu li u ovoj sesiji omogućene mjere?

  - **SamplingKey** – ključ uzorkovanja za ovaj klijent

  - **SamplingMethod** – metoda uzorkovanja za ovaj klijent

### <a name="officetelemetrysessiontelemetryruleschanged"></a>Office.Telemetry.SessionTelemetryRulesChanged

Prijavljuje da se skup telemetrijskih pravila promijenio

Prikupljaju se sljedeća polja:

  - **ChangedRuleId** – ID telemetrijskog pravila koje se promijenilo u trenutnom ažuriranju

  - **ChangedRuleVersion** – verzija telemetrijskog pravila koje se promijenilo u trenutnom ažuriranju

  - **OperationType** – dodavanje ili uklanjanje oznake operacije

### <a name="officetelemetrysessiontelemetryrulescount"></a>Office.Telemetry.SessionTelemetryRulesCount

Prijavljuje broj učitanih telemetrijskih pravila

Prikupljaju se sljedeća polja:

  - **CountOfLoadedRules** – broj učitanih telemetrijskih pravila

  - **HadRuleFileAtBoot** – određuje je li prilikom pokretanja aplikacije postojala datoteka telemetrijskih pravila

### <a name="officetelemetrysessiontelemetryrulesinitialstate"></a>Office.Telemetry.SessionTelemetryRulesInitialState

Prijavljuje telemetrijska pravila koja su učitana prilikom pokretanja sesije

Prikupljaju se sljedeća polja:

  - **HadRuleFileAtBoot** – određuje je li prilikom pokretanja aplikacije postojala datoteka telemetrijskih pravila

  - **LoadedRulesCount** – broj učitanih telemetrijskih pravila

  - **LoadedRulesList** – popis učitanih telemetrijskih pravila

### <a name="officetelemetrysystemhealthmetadatanetworkcost"></a>Office.Telemetry.SystemHealthMetadataNetworkCost

Trošak mreže označava našu sposobnost dohvaćanja podataka.

Prikupljaju se sljedeća polja:

  - **NetworkCost** – novi trošak mreže s ograničenim ili neograničenim prometom

  - **OldNetworkCost** – prethodni trošak mreže s ograničenim ili neograničenim prometom

  - **Tag** – oznaka izvorišnog koda koja je otkrila promjenu

### <a name="officetelemetrysystemhealthmetadatanetworkcostchange"></a>Office.Telemetry.SystemHealthMetadataNetworkCostChange

Trošak mreže označava našu sposobnost dohvaćanja podataka.

Prikupljaju se sljedeća polja:

  - **NewNetworkCost** – novi trošak mreže s ograničenim ili neograničenim prometom

  - **OldNetworkCost** – prethodni trošak mreže s ograničenim ili neograničenim prometom

  - **Tag** – oznaka izvorišnog koda koja je otkrila promjenu

### <a name="officetelemetrytelemetryactivityaggregationwindowstatistics"></a>Office.Telemetry.TelemetryActivityAggregationWindowStatistics

Prijavljuje broj skupnih grupa aktivnosti i instanci u svakoj aktivnosti koja se prenosi.

Prikupljaju se sljedeća polja:

  - **GroupCount** – broj skupnih aktivnosti koje šalju podatke.

  - **InstancesToSend** – broj instanci skupnih aktivnosti koje šalju podatke.

### <a name="officetelemetrytelemetryulsqueueusage"></a>Office.Telemetry.TelemetryUlsQueueUsage

Prijavljivanje pogrešaka u stanju telemetrije. Obavezno za provjeru valjanosti ostalih podataka (uključujući NSD).

Prikupljaju se sljedeća polja:

  - **AverageEventCount** – prosječni broj događaja u redu čekanja

  - **AverageQueueCB** – prosječna veličina memorije reda čekanja

  - **PeakEventCount** – vršni broj događaja u redu čekanja

  - **PeakQueueCB** – vršna veličina memorije reda čekanja

  - **QueueDisableRuleLimit** – ograničenje pri kojem se telemetrijska pravila onemogućuju

### <a name="officetelemetryulsqueuetopthrottlingtags"></a>Office.Telemetry.UlsQueueTopThrottlingTags

Prijavljuje oznake koje su najviše pridonijele isključivanju reda čekanja ULS.

Prikupljaju se sljedeća polja:

  - **Tag0 –** oznaka koja je zauzela najviše mjesta u redu čekanja

  - **Tag0Percent –** postotak reda čekanja koji je zauzela oznaka tag0

  - **Tag1 –** druga po redu oznaka koja je zauzela najviše mjesta u redu čekanja

  - **Tag10 –** jedanaesta po redu oznaka koja je zauzela najviše mjesta u redu čekanja

  - **Tag10Percent –** postotak reda čekanja koji je zauzela oznaka tag10

  - **Tag11 –** dvanaesta po redu oznaka koja je zauzela najviše mjesta u redu čekanja

  - **Tag11Percent –** postotak reda čekanja koji je zauzela oznaka tag11

  - **Tag12 –** trinaesta po redu oznaka koja je zauzela najviše mjesta u redu čekanja

  - **Tag12Percent –** postotak reda čekanja koji je zauzela oznaka tag12

  - **Tag13 –** četrnaesta po redu oznaka koja je zauzela najviše mjesta u redu čekanja

  - **Tag13Percent –** postotak reda čekanja koji je zauzela oznaka tag13

  - **Tag14 –** petnaesta po redu oznaka koja je zauzela najviše mjesta u redu čekanja

  - **Tag14Percent –** postotak reda čekanja koji je zauzela oznaka tag14

  - **Tag1Percent –** postotak reda čekanja koji je zauzela oznaka tag1

  - **Tag2 –** treća po redu oznaka koja je zauzela najviše mjesta u redu čekanja

  - **Tag2Percent –** postotak reda čekanja koji je zauzela oznaka tag2

  - **Tag3 –** četvrta po redu oznaka koja je zauzela najviše mjesta u redu čekanja

  - **Tag3Percent –** postotak reda čekanja koji je zauzela oznaka tag3

  - **Tag4 –** peta po redu oznaka koja je zauzela najviše mjesta u redu čekanja

  - **Tag4Percent –** postotak reda čekanja koji je zauzela oznaka tag4

  - **Tag5 –** šesta po redu oznaka koja je zauzela najviše mjesta u redu čekanja

  - **Tag5Percent –** postotak reda čekanja koji je zauzela oznaka tag5

  - **Tag6 –** sedma po redu oznaka koja je zauzela najviše mjesta u redu čekanja

  - **Tag6Percent –** postotak reda čekanja koji je zauzela oznaka tag6

  - **Tag7 –** osma po redu oznaka koja je zauzela najviše mjesta u redu čekanja

  - **Tag7Percent –** postotak reda čekanja koji je zauzela oznaka tag7

  - **Tag8 –** deveta po redu oznaka koja je zauzela najviše mjesta u redu čekanja

  - **Tag8Percent –** postotak reda čekanja koji je zauzela oznaka tag8

  - **Tag9 –** deseta po redu oznaka koja je zauzela najviše mjesta u redu čekanja

  - **Tag9Percent –** postotak reda čekanja koji je zauzela oznaka tag9

### <a name="officetelemetryvolumetrackingdata"></a>Office.Telemetry.VolumeTrackingData

Metrika praćenja količine događaja za telemetrijske događaje

Prikupljaju se sljedeća polja:

  - **EventThreshold** – maksimalan broj instanci jednog događaja koji se može poslati u određenom vremenskom razdoblju.

  - **HighestEventCount** – najveći broj instanci jednog događaja poslanih u tom razdoblju.

  - **HighestEventName** – naziv događaja s najvećim brojem instanci u tom razdoblju.

  - **TimeWindowInSeconds** – trajanje razdoblja u sekundama.

  - **TotalEvents** – ukupan broj događaja poslanih u tom razdoblju.

  - **UniqueEvents** – broj jedinstvenih događaja poslanih tijekom nekog razdoblja.

### <a name="officetelemetrywritepayloadstodisk"></a>Office.Telemetry.WritePayloadsToDisk

Provjerava funkcioniraju li određeni dijelovi naslijeđenog kanala na platformama koje ga još koriste.

Prikupljaju se sljedeća polja:

  - **DetachedDuration** – odvojeno trajanje u mikrosekundama
