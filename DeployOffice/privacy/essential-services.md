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
ms.openlocfilehash: 81b5ff2e1451f910f2e9695dba488d39d27b7241
ms.sourcegitcommit: 3f5de6281b8e92c6c41a800f4374211188460320
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34701269"
---
# <a name="essential-services-for-office"></a>Ključni servisi za Office

> [!IMPORTANT]
> Informacije u ovom članku odnose se na verziju 1904 ili noviju verziju sljedećeg klijentskog softvera sustava Office instaliranog na računalu sa sustavom Windows:
> - Office 365 ProPlus i Office 365 Business
> - Office 365 Personal, Office 365 Home ili druge verzije sustava Office koje su dio pretplate na Office 365.
> - Project i Visio koji se isporučuju s nekim pretplatničkim tarifama, kao što su Project Online Professional ili Visio Online Plan 2.


Office se sastoji od klijentskih softverskih aplikacija i povezanih okruženja osmišljenih radi učinkovitijeg stvaranja, komunikacije i suradnje. Premda kao administrator tvrtke ili ustanove možete upravljati brojnim povezanim sučeljima koja su dostupna vama ili vašim korisnicima, neki su servisi ključni za funkcioniranje sustava Office, pa se ne mogu onemogućiti. To je, primjerice, servis za licenciranje, koji potvrđuje da imate odgovarajuću licencu za korištenje sustava Office. Obavezni servisni podaci o tim servisima prikupljaju se i šalju Microsoftu bez obzira na druge konfigurirane postavke zaštite privatnosti. Te podatke možete pogledati pomoću preglednika dijagnostičkih podataka.

Dodatne informacije potražite u sljedećim člancima:

- [Obavezni servisni podaci za Office](required-service-data.md)
- [Korištenje preglednika dijagnostičkih podataka sa sustavom Office](https://support.office.com/article/cf761ce9-d805-4c60-a339-4e07f3182855)
- [Povezana okruženja u sustavu Office](connected-experiences.md)

Ako ste administrator za tvrtku ili ustanovu, možda će vas zanimati i sljedeći članci:

- [Pregled kontrola za zaštitu privatnosti za Office 365 ProPlus](overview-privacy-controls.md)
- [Korištenje postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Office 365 ProPlus](manage-privacy-controls.md)

## <a name="list-of-essential-services-for-office"></a>Popis ključnih servisa za Office 

U tablici u nastavku naveden je popis ključnih servisa za Office i opis svakog servisa.

| **Servis**  | **Opis**  |
| ------ | ---- |
| [Provjera autentičnosti](#authentication-events) | Provjera autentičnosti servis je koji obuhvaća više platformi, a služi za provjeru valjanosti identiteta korisnika sustava Office.  Nužan je da biste se mogli prijaviti u Office, aktivirati licencu za Office, pristupiti datotekama pohranjenima u oblaku, a omogućuje i dosljedno sučelje u svim sesijama sustava Office na svim uređajima.    |
| [Klikom do cilja](#click-to-run-events) | "Klikom do cilja" tehnologija je za instalaciju koja se koristi za instaliranje i ažuriranje sustava Office u sustavu Windows. Tehnologija provjerava postoji li nova verzija sustava Office i kad postoji, preuzima je i instalira. Tehnologija "klikom do cilja" otkrit će jesu li vam potrebna ažuriranja sustava Office, uključujući sigurnosna ažuriranja, te će ih preuzeti i instalirati.     |
| [Servis za poboljšanu konfiguraciju (eng. Enhanced Configuration Service, ECS)](#experimentation-and-configuration-service-ecs-events) | ECS Microsoftu omogućuje da iznova konfigurira instalacije sustava Office bez potrebe za ponovnom implementacijom sustava. Služi za kontroliranje postupnog objavljivanja značajki ili ažuriranja, a učinak objavljivanja prati se na temelju prikupljenih dijagnostičkih podataka. Koristi se i za ublažavanje sigurnosnih problema i problema s performansama neke značajke ili ažuriranja. ECS podržava i promjene konfiguracije povezane s dijagnostičkim podacima da bi se prikupljali odgovarajući događaji. |
| [Licenciranje](#licensing-events)     | Licenciranje je servis u oblaku koji podržava aktivaciju novih instalacija sustava Office te održava licencu na uređajima nakon aktivacije sustava. Servis registrira svaki uređaj i aktivira Office, provjerava status pretplate na Office te upravlja ključevima proizvoda.    |
| [Konfiguracija servisa](#services-configuration-events)  | Konfiguracija servisa omogućuje ažuriranje postavki konfiguracije sustava Office radi omogućivanja odnosno onemogućivanja značajki klijenata. Aktivira se svaki put kad se pokrene neka aplikacija sustava Office te sadrži pojedinosti o drugim konfiguracijama i servisima sustava Office. Konfiguracija servisa ujedno kontrolira koji su servisi određeni kao ključni.  |
| [Telemetrija](#telemetry-events)  | Servis za telemetriju služi za prikupljanje dijagnostičkih podataka iz aplikacija sustava Office. Omogućuje prikupljanje obaveznih i neobaveznih dijagnostičkih podataka koje je generirao Office. Odgovoran je i za prikupljanje onog dijela obaveznih servisnih podataka za Office koji obuhvaća servisne dijagnostičke podatke.  |

## <a name="events-and-data-fields-for-essential-services-for-office"></a>Događaji i podatkovna polja za ključne servise za Office

U sljedećim odjeljcima navode se ove informacije:

- popis događaja za svaki ključni servis
- opis svakog događaja
- popis podatkovnih polja u svakom događaju
- opis svakog podatkovnog polja

Događaje možete pogledati pomoću preglednika dijagnostičkih podataka.



## <a name="authentication-events"></a>Događaji provjere autentičnosti

Ti se događaji dijagnostičkih podataka prikupljaju kada Office pokuša dohvatiti token za provjeru autentičnosti, bilo u pozadini ili putem upita korisniku.

### <a name="officeidentityfbapromptwin32"></a>Office.Identity.FbaPromptWin32

Prikuplja se kada Office korisniku prikaže upit za prijavu pomoću provjere autentičnosti na temelju obrazaca.

Upiti za provjeru autentičnosti zajedno s pozadinskim pribavljanjem tokena koriste se za utvrđivanje je li korisnik u neispravnom stanju provjere autentičnosti, koje se za korisnika očituje praktički izvanmrežnim stanjem klijenta. Neispravna provjera autentičnosti može i onemogućiti dohvaćanje licence, što uzrokuje potpunu nemogućnost korištenja klijenta.

Upiti za prijavu pomoću provjere autentičnosti na temelju obrazaca (FBA) koriste se u nekim scenarijima lokalne provjere autentičnosti i najčešće ne želimo da se to događa jer bi svi trebali koristiti modernu provjeru autentičnosti zbog sigurnosnih slabih točaka povezanih s provjerom autentičnosti na temelju obrazaca.

**Prikupljaju se sljedeća polja:**

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

Kad se zna da se korisnik odjavio, moguće je na očekivani način klasificirati druge događaje, kao što su upiti, da bi se točno izračunali u metrici pouzdanosti / spremnosti za isporuku te se izbjegavaju upozorenja ili vraćanje međuverzija na temelju pogrešne premise da se korisniku prikazuju neočekivani upiti za prijavu.

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

4\) signali služe kao podaci za razne nadzornike spremnosti za isporuku i stanja koji aktiviraju upozorenja da bi se naši inženjeri mogli brzo angažirati i skratiti vrijeme do otklanjanje kritičnih pogrešaka koje blokiraju rad korisnika

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

4\) signali služe kao podaci za razne nadzornike spremnosti za isporuku i stanja koji aktiviraju upozorenja da bi se naši inženjeri mogli brzo angažirati i skratiti vrijeme do otklanjanje kritičnih pogrešaka koje blokiraju rad korisnika

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

4\) signali služe kao podaci za razne nadzornike spremnosti za isporuku i stanja koji aktiviraju upozorenja da bi se naši inženjeri mogli brzo angažirati i skratiti vrijeme do otklanjanje kritičnih pogrešaka

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

  - **Microsoft\_ADAL\_http\_event\_coun**t – broj HTTP poziva koje je uputio ADAL.

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

  - **Microsoft\_ADAL\_x\_ms\_request\_id** – dodatni ID zahtjeva koji ADAL navodi u HTTP zaglavlju za servis.

  - **Platform** – Win32/WinRT/Android/iOS/Mac

  - **Scenarioid** – GUID. U jednom scenariju može biti veći broj događaja, npr. scenarijem se može dodavati novi račun, ali se u sklopu njega prikazuje više upita. Taj ID omogućuje korelaciju.

  - **Sessionid** – GUID koji određuje sesiju pokretanja

  - **Skdver** –verzija SDK-a MATS klijenta koja je korištena za stvaranje podataka

  - **StartTime** – vrijeme pozivanja MATS API-ja Start\*Action

  - **Tenantid** – GUID koji označava klijent kojem korisnik provjerene autentičnosti pripada (u slučajevima koji nisu ADAL).

  - **Uploadid** – jedinstveni GUID događaja, koristi se za poništavanje dupliciranja

  - **Wamapi** – određuje koji se WAM API poziva

  - **Wamtelemetrybatch** – trenutno se ne koristi. Ubuduće će komponenti WAM omogućiti slanje dodatnih informacija o događaju provjere autentičnosti.

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

  - **Data\_PrereqFailure\_Type** – neispunjeni preduvjet, npr. operacijski sustav nije podržan

  - **Data\_ProductReleaseId** – proizvod koji instaliramo, npr. Office 365 ProPlus

### <a name="officeclicktoruncorruptioncheck"></a>Office.ClickToRun.CorruptionCheck

Podaci o instalaciji i inventaru sustava Office prikupljeni kada klijent tehnologije "klikom do cilja" pokrene provjeru oštećenja radi potvrđivanja jesu li binarne datoteke sustava Office točne. Koristi se za mjerenje oštećenja binarnih datoteka sustava Office i utvrđivanje koje su binarne datoteke oštećene.

Prikupljaju se sljedeća polja:

  - **Data\_Active –** trenutni manifest strujanja koji provjeravamo na disku

  - **Data\_ActivePackages –** označava pakete koje manifest sadrži

  - **Data\_ActiveVersion –** verzija manifesta

  - **Data\_AddFileCount –** broj datoteka koje dodajemo

  - **Podataka\_AddFileFiles -** uzorak datoteka koje dodajemo

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

  - **Data\_Sku** – instalirani SKU, npr. Office 365 ProPlus.hr-hr

  - **Data\_SqmMachineID** – jedinstveni ID računala koji koristi identifikator ažuriranja sustava Office Windows SQM Data\_SusClientID- Machine

### <a name="officeclicktorunodt"></a>Office.ClickToRun.ODT

Podaci o instalaciji i inventaru sustava Office prikupljeni kada IT administrator pokrene setup.exe s tehnologijom "klikom do cilja" alata za implementaciju sustava Office radi izmjene proizvoda sustava Office koje su instalirali korisnici. Koristi se za mjerenje uspjeha/pogrešaka instalacija sustava Office koje je u potpunosti pokrenuo administrator, uključujući provjere preduvjeta.

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

  - **Data\_ProductReleaseId** – proizvod koji instaliramo, npr. Office 365 ProPlus

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

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala koji koristi Windows SQM 

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

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

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –**  jedinstveni ID računala koji koristi Windows SQM 

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

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

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala koji koristi Windows SQM 

  - **Data\_SusClientID –**  identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

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

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –**  jedinstveni ID računala koji koristi Windows SQM 

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

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

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –**  jedinstveni ID računala koji koristi Windows SQM 

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

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

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala koji koristi Windows SQM

  - **Data\_SusClientID –**  identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

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

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala koji koristi Windows SQM

  - **Data\_SusClientID –** identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

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

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala koji koristi Windows SQM

  - **Data\_SusClientID –**  identifikator ažuriranja sustava Office na računalu

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

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

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala koji koristi Windows SQM

  - **Data\_SusClientID –**  identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioinstalltaskremoveinstallation"></a>Office.ClickToRun.Scenario.InstallTaskRemoveinstallation

Podaci o instalaciji i inventaru sustava Office prikupljeni kada instalacijski program sustava Office uklanja dijelove sustava Office s uređaja. Koristi se za mjerenje uspjeha/pogrešaka instalacije sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –**  verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala koji koristi Windows SQM

  - **Data\_SusClientID –**  identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioinstalltaskstream"></a>Office.ClickToRun.Scenario.InstallTaskStream

Podaci o instalaciji i inventaru sustava Office prikupljeni kada instalacijski program sustava Office preuzima nove datoteke za Office. Koristi se za mjerenje uspjeha/pogrešaka instalacije sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –**  verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –**  jedinstveni ID računala koji koristi Windows SQM 

  - **Data\_SusClientID –**  identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioinstalltaskuninstallcentennial"></a>Office.ClickToRun.Scenario.InstallTaskUninstallcentennial

Podaci o instalaciji i inventaru sustava Office prikupljeni kada instalacijski program sustava Office deinstalira stariju verziju sustava Office koje je instalirana iz trgovine. Koristi se za mjerenje uspjeha/pogrešaka instalacije sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –** verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –**  jedinstveni ID računala koji koristi Windows SQM

  - **Data\_SusClientID –**  identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenariorepairtaskfinalintegrate"></a>Office.ClickToRun.Scenario.RepairTaskFinalintegrate

Podaci o instalaciji i inventaru sustava Office prikupljeni kada klijent za popravak sustava Office ponovno objavi .msi datoteke i datotečne nastavke sustava Office. Koristi se za mjerenje uspjeha/pogrešaka popravka sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –**  verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –**  jedinstveni ID računala koji koristi Windows SQM 

  - **Data\_SusClientID –**  identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

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

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –**  jedinstveni ID računala koji koristi Windows SQM 

  - **Data\_SusClientID –**  identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

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

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –**  jedinstveni ID računala koji koristi Windows SQM 

  - **Data\_SusClientID –**  identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

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

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –**  jedinstveni ID računala koji koristi Windows SQM 

  - **Data\_SusClientID –**  identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

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

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –**  jedinstveni ID računala koji koristi Windows SQM 

  - **Data\_SusClientID –**  identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

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

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –**  jedinstveni ID računala koji koristi Windows SQM 

  - **Data\_SusClientID –**  identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

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

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_PackageOperationSuccessful –** vrijednost true ako je zadatak na paketu sustava Office uspješno dovršen

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –**  jedinstveni ID računala koji koristi Windows SQM

  - **Data\_SusClientID –**  identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

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

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala koji koristi Windows SQM

  - **Data\_SusClientID –**  identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

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

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_PackageUpdateAvailable –** vrijednost je true ako je dostupna nova verzija sustava Office

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –**  jedinstveni ID računala koji koristi Windows SQM 

  - **Data\_SusClientID –**  identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioupdatetaskupdatedownload"></a>Office.ClickToRun.Scenario.UpdateTaskUpdatedownload

Podaci o instalaciji i inventaru sustava Office prikupljeni kada klijent tehnologije "klikom do cilja" preuzima novo ažuriranje. Koristi se za mjerenje uspjeha/pogrešaka ažuriranja sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –**  verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

  - **Data\_AddingProducts –** proizvodi koje trebamo dodati 

  - **Data\_AvailableVersion to –** verzija sustava Office na koju je moguće ažurirati sustav

  - **Data\_CompletedWithoutActionInfo –** razlog zbog kojeg scenarij nije dovršen, npr. aplikacije su bile otvorene

  - **Data\_CompletionState –** označava jesmo li dovršili zadatak

  - **Data\_CorruptionChecksOnly –-** označava radi li se samo o traženju oštećenja bez ažuriranja

  - **Data\_ErrorCode –** šifra pogreške zbog koje radnja nije uspjela 

  - **Data\_ErrorDetails –** dodatne pojedinosti o pogrešci 

  - **Data\_ErrorMessage –** poruka o pogrešci do koje je došlo 

  - **Data\_ErrorSource –** mjesto nastanka pogreške

  - **Data\_ExceptionType –** iznimka zbog koje radnja nije uspjela 

  - **Data\_FoundCorruptFiles –** vrijednost je true ako smo pronašli oštećene datoteke

  - **Data\_IsErrorCodeIgnorable –** označava može li se šifra pogreške zbog koje radnja nije uspjela zanemariti 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth –** određuje smatramo li da je šifru pogreške moguće zanemariti 

  - **Data\_NewestPackageVersion –** najnovija verzija sustava Office na računalu 

  - **Data\_OldestPackageVersion –** najstarija verzija sustava Office na računalu 

  - **Data\_PackageOperationSuccessful –** vrijednost true ako je zadatak na paketu sustava Office uspješno dovršen

  - **Data\_PipelineExitCode –** izlazna šifra koju je vratio kanal za datoteke

  - **Data\_ProductsToAdd –** proizvodi sustava Office koje dodajemo 

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –** jedinstveni ID računala koji koristi Windows SQM 

  - **Data\_SusClientID –**  identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktorunscenarioupdatetaskupdatefinalize"></a>Office.ClickToRun.Scenario.UpdateTaskUpdatefinalize

Podaci o instalaciji i inventaru sustava Office prikupljeni kada klijent tehnologije "klikom do cilja" čisti nakon ažuriranja i vraća prethodno otvorene aplikacije. Koristi se za mjerenje uspjeha ili pogrešaka ažuriranja sustava Office.

Prikupljaju se sljedeća polja:

  - **Data\_15\_SourceType –** mjesto na kojem se nalazi izvor za Office 15, npr. CDN ili lokalno 

  - **Data\_15\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 15 omogućena 

  - **Data\_15\_UpdateVersion –**  verzija sustava Office 15 na koju se sustav ažurira 

  - **Data\_15\_Version –** verzija sustava Office 15 

  - **Data\_16\_SourceType –** mjesto na kojem se nalazi izvor za Office 16, npr. CDN ili lokalno 

  - **Data\_16\_UpdatesEnabled –** označava jesu li ažuriranja sustava Office 16 omogućena 

  - **Data\_16\_UpdateVersion –** verzija sustava Office 16 na koju se sustav ažurira 

  - **Data\_16\_Version –** verzija sustava Office 16 

  - **Data\_AddingFixedProducts –** proizvod koji dodajemo 

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

  - **Data\_ProductsToRemove –**  proizvodi sustava Office koje uklanjamo 

  - **Data\_RemovingFixedProducts –** proizvodi koje uklanjamo 

  - **Data\_RemovingProducts –** proizvodi koje trebamo ukloniti 

  - **Data\_ScenarioInstanceID -** jedinstveni GUID za pokrenuti scenarij 

  - **Data\_ScenarioName –** scenarij koji je pokrenut. npr. instalacija 

  - **Data\_ScenarioSubType –** vrsta scenarija koji smo pokrenuli, npr. deinstalacija, ponovna instalacija 

  - **Data\_SourceType –** mjesto izvora, npr. CDN 

  - **Data\_SqmMachineID –**  jedinstveni ID računala koji koristi Windows SQM 

  - **Data\_SusClientID –**  identifikator ažuriranja sustava Office na računalu 

  - **Data\_TaskState –** stanje u kojem je zadatak, npr. pokrenut ili otkazan 

  - **Data\_TotalClientCabSize –** veličina klijentske cab datoteke 

  - **Data\_TriggeringUI –** određuje što je aktiviralo korisničko sučelje 

  - **Data\_UpdatesEnabled –** određuje jesu li ažuriranja sustava Office omogućena 

  - **Data\_Version –** verzija sustava Office 

### <a name="officeclicktoruntransportexperimentaltransportpipelinecreatetransport"></a>Office.ClickToRun.Transport.ExperimentalTransport.PipelineCreateTransport

Podaci o instalaciji i inventaru sustava Office prikupljeni kada klijent tehnologije "klikom do cilja" otvara kanal za prijenos putem kojeg će preuzimati datoteke sustava Office. Koristi se za utvrđivanje stanja raznih prijenosnih tehnologija prijenosa (npr. HTTP, BITS, DO) koje su ključne za pravilno preuzimanje sustava Office radi instalacije i ažuriranja.

Prikupljaju se sljedeća polja:

  - **Data\_IsForeGroundStreaming**  – označava prenosimo li podatke strujanjem u prvom planu ili u pozadini

  - **Data\_IsInstallMode** – ako instaliramo i preuzimamo datoteke, vrijednost je 1, a ako ne, vrijednost je 0

  - **Data\_SourceProtocol –** označava preuzimamo li iz mreže podataka sadržaja (CDN-a), s računala na koje instaliramo, iz lokalne mreže ili iz resursa u lokalnoj područnoj mjreži.

  - **Data\_Status**  – označava uspjeh ili neuspjeh 

### <a name="officeclicktorunupdatestatus"></a>Office.ClickToRun.UpdateStatus

Podaci o instalaciji i inventaru sustava Office prikupljeni kada klijent tehnologije "klikom do cilja" završava status ažuriranja

Prikupljaju se sljedeća polja:

  - **Data\_build** – trenutno instalirana verzija sustava Office

  - **Data\_channel** – kanal u kojem se korisnik nalazi

  - **Data\_errorCode** – cijeli broj koji određuje vrstu pogreške do koje je došlo ako pogreška postoji

  - **Data\_errorMessage** – niz koji sadrži opis pogreške do koje je došlo ako pogreška postoji

  - **Data\_status** – kratak status događaja tijekom ažuriranja, npr. uspješno ili preuzeto

  - **Data\_targetBuild -** – verzija sustava Office na koju pokušavamo ažurirati


## <a name="experimentation-and-configuration-service-ecs-events"></a>Događaji servisa za eksperimentiranje i konfiguraciju (ECS-a)

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


## <a name="licensing-events"></a>Događaji licenciranja

### <a name="officelicensingaccepteulaforcurrentlicense"></a>Office.Licensing.AcceptEulaForCurrentLicense 

To se prikuplja kad korisnik dobije licencu i prihvati EULA-u za trenutnu licencu

Koristi se radi otkrivanja je li korisnik u dobrom stanju, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **ACID** – GUID identifikator koji predstavlja proizvod sustava Office za koji korisnik ima licencu

  - **DwEulaId** – numerički identifikator vrste EULA-e koju je korisnik upravo prihvatio

### <a name="officelicensingactivation"></a>Office.Licensing.Activation 

Nakon postavljanja licence na računalu pokušavamo licencu aktivirati pozivanjem servisa AVS. Ovo prijavljuje rezultat poziva radi aktivacije

Ključno je za otkrivanje koliko bi korisnika moglo imati problema s aktivacijom. Za otkrivanje eventualnih regresija imamo otkrivanje anomalija. To je izuzetno važno jer ovisimo o vanjskom servisu AVS, pa nam ovaj signal pokazuje je li stanje naših vanjskih partnera dobro. Koristi se i u dijagnostičke svrhe te za utvrđivanje stanja sustava ako korisnik priajvi problem s uređajem

Prikupljaju se sljedeća polja:

  - **Acid** – GUID identifikator koji predstavlja proizvod sustava Office za koji korisnik ima licencu

  - **ReferralData** – identifikator OEM-a koji je instalirao Office na računalo

### <a name="officelicensingactivationwizard"></a>Office.Licensing.ActivationWizard 

Ako zbog nekog razloga ne možemo automatski aktivirati licencu, korisniku prikazujemo čarobnjak za aktivaciju. Ovo prijavljuje da je korisniku prikazan čarobnjak. Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Događaj ne prikuplja nijedno polje.

### <a name="officelicensingenforcesigninqualified"></a>Office.Licensing.EnforceSignInQualified 

Taj nam signal daje do znanja je li eksperiment koji smo pokrenuli radi prisilne prijave korisnika u sklopu licenciranja uspio. Ključan je za otkrivanje uspješnosti ili pogreške eksperimenta kojim se korisnika prisiljava na prijavu, a to je obavezan korak modernog stoga za licenciranje. Ako se korisnik ne prijavi, neće moći koristiti aplikaciju.

Prikupljaju se sljedeća polja:

  - **Qualified** – određuje je li korisnik kvalificiran za prisilnu prijavu

### <a name="officelicensingexpirationdialogshown"></a>Office.Licensing.ExpirationDialogShown

To se prikuplja kad korisniku prikažemo dijaloški okvir o isteku koji ga obavještava da je licenca istekla. Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **LicNotificationState** – identifikator koji nas obavještava o tome kakve se obavijesti prikazuju korisniku

### <a name="officelicensingfullvalidation"></a>Office.Licensing.FullValidation 

To se prikupljaju u svakoj sesiji koja prijavljuje stanje licenciranja računala te prijavljuje pogreške koje se korisniku prikazuju i zbog kojih ne može koristiti aplikaciju. Događaj označava je li korisnikovo računalo u dobrom stanju. Za taj smo događaj postavili otkrivanje anomalija da bismo prepoznali uzrokuje li regresija negativno ponašanje korisnika. Ključno je i za dijagnosticiranje korisničkih problema te za praćenje stanja sustava

Prikupljaju se sljedeća polja:

  - **Acid** – GUID identifikator koji predstavlja proizvod sustava Office za koji korisnik ima licencu 

  - **IsSessionLicensing** – određuje je li trenutno pokrenut način rada za aktivaciju zajedničkog računala 

  - **LicenseCategory** – kategorija licence za Office koju korisnik koristi 

  - **Licenses** – popis naziva svih licenci za Office koje postoje na računalu 

  - **LicenseStatuses** – status svih licenci za Office koje postoje na računalu 

### <a name="officelicensinggetentitlement"></a>Office.Licensing.GetEntitlement 

To prikupljamo kad korisnik postavlja uređaj te pozivamo servis za licenciranje da otkrije ima li prijavljeni korisnik prava na Office. Prijavljuje rezultat poziva Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Događaj ne prikuplja nijedno polje.

### <a name="officelicensingheartbeat"></a>Office.Licensing.Heartbeat 

Za svaku sesiju provjeravamo je li prošlo 72 sata od zadnje obnove licence te pokušavamo produljiti vrijeme do isteka trenutne licence. Događaj prijavljuje uspješnost ili pogrešku poziva koji upućujemo radi provjere možemo li produljiti vrijeme do isteka licence i zadržati funkcionalnost korisnikove instalacije sustava Office. Ključan je za dijagnosticiranje problema povezanih s pretplatom i problema sa servisom za korisnika te za otkrivanje regresija već aktiviranih korisnika pretplate.

Prikupljaju se sljedeća polja:

  - **Mode** – prikaz stoga licenciranja sustava Office koji se koristi na računalu kao identifikatora

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

U slučaju da naiđemo na probleme s tijekom rada za aktivaciju, aktiviramo čarobnjak za licenciranje te šaljemo signal koji to označava. Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

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

Ako zatvorimo/srušimo Office zbog problema s licenciranjem, šaljemo ovaj signal da bismo to naznačili. Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **ExitCode** – interni kod koji je uzrokovao zatvaranje aplikacije

### <a name="officelicensingloadidentityticket"></a>Office.Licensing.LoadIdentityTicket

Aplikacija tijekom pokušaja licenciranja uređaja pokušava učitati korisnikov identitet da bi provjerila ima li korisnik prava na Office. Ovaj događaj prijavljuje uspjeh ili pogrešku tog postupka te eventualnu šifru pogreške. Ključan je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **FederationProvider** – niz koji određuje davatelja usluga vanjskog pristupa trenutno prijavljenog korisnika

  - **IdentityProvider** – niz koji određuje davatelja usluga identiteta trenutno prijavljenog korisnika

### <a name="officelicensinglvuxeulaexplicitcrash"></a>Office.Licensing.LVUX.EULAExplicitCrash 

To se prikupljaju ako smo korisniku prikazali EULA-u, a korisnik je nije prihvatio, zbog čega rušimo/zatvaramo aplikaciju. Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **Acid** – GUID identifikator koji predstavlja proizvod sustava Office za koji korisnik ima licencu

  - **OptInShown** – označava je li dijaloški okvir za uključivanje koji se prikazuje prilikom prvog pokretanja aplikacije već prikazan

  - **Office.Licensing.NextUserLicensingEligible –** taj signal označava je li korisnik kvalificiran za premještanje na novi stog za licenciranje. Ključno je za kvantifikaciju učinka na postojeće korisnike tijekom uvođenja novog stoga za licenciranje te da korisnici ne bi izgubili funkcionalnost

Događaj ne prikuplja nijedno polje.

### <a name="officelicensingnulfetcherfetchmodelfromols"></a>Office.Licensing.Nul.Fetcher.FetchModelFromOls

Kada je uređaj na modernom stogu za licenciranje, licencnu datoteku pokušavamo dohvatiti izravno sa servisa. Događaj prijavljuje uspjeh ili pogrešku zajedno s eventualnom šifrom pogreške poziva servisu. Ključan je za otkrivanje je li korisnik u dobrom stanju na modernom stogu za licenciranje, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **MetadataValidationResult** – rezultat provjere valjanosti metapodataka o licenci da bi se potvrdilo da nije neovlašteno mijenjana

  - **SignatureValidationResult** – rezultat provjere valjanosti potpisa licence da bi se potvrdilo da nije neovlašteno mijenjana

### <a name="officelicensingnulvalidationfullvalidation"></a>Office.Licensing.Nul.Validation.FullValidation 

To se prikuplja tijekom svake sesije uređaja koji koristi moderni stog za licenciranje. Prijavljuje stanje licence računala i pogreške koje se korisniku prikazuju i zbog kojih ne može koristiti aplikaciju. Događaj naznačuje je li korisnikovo računalo u dobrom stanju na modernom stogu za licenciranje. Za taj smo događaj postavili otkrivanje anomalija da bismo prepoznali uzrokuje li regresija negativno ponašanje korisnika. Ključno je i za dijagnosticiranje korisničkih problema te za praćenje stanja sustava.

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

  - **Licensing ACID** – GUID identifikator koji predstavlja proizvod sustava Office za koji korisnik ima licencu 

  - **OlsLicenseId** – alfanumerički identifikator licence koja je izdana korisniku 

  - **SkuIdIsNull** – označava jesmo li naišli na pogrešku zbog koje ne znamo koji proizvod korisnik upotrebljava 

  - **SlapiIsNull** – označava jesmo li naišli na problem prilikom popunjavanja jednog od objekata licenciranja 

### <a name="officelicensingonlinerepair"></a>Office.Licensing.OnlineRepair 

Ako zbog nekog razloga ne možemo aktivirati korisnika i moramo mu prikazati dijaloški okvir u kojem se od njega traži da se povežu s internetom i pokušaju s koracima za popravak, aktivira se ovaj događaj. Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Događaj ne prikuplja nijedno polje.

### <a name="officelicensingpurchase"></a>Office.Licensing.Purchase 

Imamo eksperiment u kojem se korisniku nudi mogućnost da isproba i postavi automatsko plaćanje sustava Office izravno iz aplikacije, a da ni u jednom trenutku ne mora izaći iz aplikacije. Ovo prijavljuje uspjeh ili pogrešku tog eksperimenta te eventualnu šifru pogreške. Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **StorePurchaseStatus** – predstavlja šifru pogreške / šifru uspjeha poziva za kupnju obavljenog putem Windows trgovine

### <a name="officelicensingsearchforsessiontoken"></a>Office.Licensing.SearchForSessionToken

Ako je korisnik u načinu rada za aktivaciju na zajedničkom računalu, pokušavamo potražiti token sesije na računalu koji korisniku omogućuje upotrebu aplikacije. Ovaj događaj prijavljuje uspjeh ili pogrešku tog scenarija te eventualnu šifru pogreške. Ključan je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

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

  - **PendingAcid** – ID proizvoda za koji je na čekanju pretvorba SKU-a

  - **SourceSku** – naziv izvornog SKU-a instaliranog na računalu

  - **UninstallProduct** – označava hoće li se stari proizvod deinstalirati prilikom pretvorbe

### <a name="officelicensingusegracekey"></a>Office.Licensing.UseGraceKey

Ako zbog nekog razloga ne možemo licencirati korisnika, instaliramo privremeni ključ i šaljemo signal koji to označava. Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

Prikupljaju se sljedeća polja:

  - **OpportunisticTokenRenewalAttempted** – označava jesmo li pokušali oportunistički obnoviti korisnika u načinu rada za licenciranje zajedničkog računala

  - **ReArmResult** – označava rezultat ponovne aktivacije instalacijskog ključa koji može produljiti vrijeme do isteka trenutne licence

## <a name="services-configuration-events"></a>Događaji konfiguracije servisa

Konfiguracija servisa ne prikuplja događaje vezane uz obavezne servisne dijagnostičke podatke.

## <a name="telemetry-events"></a>Telemetrijski događaji

### <a name="officesystemidentitychanged"></a>Office.System.IdentityChanged

Podaci o identitetu korisnika koji su potrebni za ispunjavanje zahtjeva ispitanika.

Prikupljaju se sljedeća polja:

  - **IdentityChanged** – uvijek ima vrijednost true. Identitet je promijenjen.

  - **TimerDetectedChange** – označava je li redovno tempiran ping otkrio promjenu.

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

<!-- end list -->

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

  - **CollectibleClassifications –** klasifikacije podataka koje se mogu prikupljati u skladu s postavkama zaštite privatnosti u klijentu

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

Koristi se za snimanje metrike rušenja.

Prikupljaju se sljedeća polja:

  - **AffectedProcessAppBuild –** identifikator međuverzije zahvaćenog procesa.

  - **AffectedProcessAppBuildRevision –** identifikator revizije međuverzije zahvaćenog procesa.

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

  - **CrashedEcsETag –** identifikator eksperimenta za srušeni proces.

  - **CrashedImpressionId –** identifikator prikaza srušenog procesa.

  - **CrashedProcessSessionID –** jedinstveni identifikator srušenog procesa.

  - **CrashedProcessSessionInitTime –** vrijeme pokretanja zahvaćenog procesa.

  - **CrashType –** identifikator grupiranja za vrstu rušenja.

  - **DetectionTime –** vrijeme otkrivanja neočekivanog zatvaranja.

  - **ErrorString –** opis pogreške.

  - **ExceptionAddress –** adresa u programu na kojoj je došlo do pogreške.

  - **ExceptionCode –** identifikator grupiranja za iznimku.

  - **FaultAppName –** naziv aplikacije s pogreškom.

  - **InstallMethod** – određuje je li sustav nadograđen na trenutnu međuverziju sustava Office, vraćen na nju ili je u pitanju nova instalacija.

  - **InstallType –** identifikator metode kojom je Office instaliran.

  - **InstallTypeName –** identifikator metode kojom je Office instaliran.

  - **IsLabMachine –** određuje pokreće li se Office u Microsoftovu laboratoriju.

  - **IsMsftInternal –** označava je li korisnik sustava Windows koji pokreće Office Microsoftov zaposlenik.

  - **ModuleBaseAddress –** osnovna adresa neispravnog modula.

  - **ModuleBuildVersion –** broj međuverzije neispravnog modula.

  - **ModuleMajorVersion –** broj glavne verzije neispravnog modula.

  - **ModuleMinorVersion –** broj sporedne verzije neispravnog modula.

  - **ModuleName –** naziv neispravnog modula.

  - **ModuleOffset –** pomak u bajtovima od osnovne adrese na kojoj je došlo do pogreške.

  - **ModuleRevisionVersion –** broj revizije međuverzije neispravnog modula.

  - **ModuleSize –** veličina neispravnog modula u bajtovima.

  - **OSEnvironment –** identifikator okruženja u kojem je Office pokrenut.

  - **PreviousBuild** – prethodno instalirana međuverzija

  - **UAETypeName –** identifikator grupiranja načina na koji se aplikacija neočekivano zatvorila.

  - **VerifyElseCrashTag –** jedinstveni identifikator mjesta na kojem se aplikacija srušila.

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

Koristi se za snimanje metrike rušenja.

Prikupljaju se sljedeća polja:

  - **CrashedAppBuild –** identifikator međuverzije zahvaćenog procesa.

  - **CrashedAppMajor –** identifikator glavne verzije zahvaćenog procesa.

  - **CrashedAppMinor –** identifikator sporedne verzije zahvaćenog procesa.

  - **CrashedAppRevision –** identifikator međuverzije zahvaćenog procesa.

  - **CrashedConfigIds –** konfiguracija dodijeljena srušenom procesu.

  - **CrashedEcsETag –** identifikator eksperimenta za srušeni proces.

  - **CrashedImpressionId –** identifikator prikaza srušenog procesa.

  - **CrashedModuleName –** naziv neispravnog modula.

  - **CrashedSessionId –** jedinstveni identifikator srušenog procesa.

  - **CrashedSessionInitTime –** vrijeme pokretanja zahvaćenog procesa.

  - **CrashType –** identifikator grupiranja za vrstu rušenja.

  - **DetectionTime –** vrijeme otkrivanja neočekivanog zatvaranja.

  - **ExceptionAddress –** adresa u programu na kojoj je došlo do pogreške.

  - **ExceptionCode –** identifikator grupiranja za iznimku.

  - **HexExceptionAddress –** heksadecimalni oblik adrese u programu na kojoj je došlo do pogreške.

  - **HexExceptionCode –** heksadecimalni identifikator grupiranja za iznimku.

  - **HexModuleBaseAddress –** osnovna adresa neispravnog modula u heksadecimalnom obliku.

  - **HexModuleBaseAddress –** pomak u bajtovima (u heksadecimalnom obliku) od osnovne adrese na kojoj je došlo do pogreške.

  - **HexModuleSize –** veličina neispravnog modula u bajtovima u heksadecimalnom obliku.

  - **HexVerifyElseCrashTag –** jedinstveni identifikator mjesta na kojem se aplikacija srušila u heksadecimalnom obliku.

  - **InstallMethod** – određuje je li sustav nadograđen na trenutnu međuverziju sustava Office, vraćen na nju ili je u pitanju nova instalacija.

  - **IsLabMachine –** određuje pokreće li se Office u Microsoftovu laboratoriju.

  - **ModuleBaseAddress –** osnovna adresa neispravnog modula.

  - **ModuleOffset –** pomak u bajtovima od osnovne adrese na kojoj je došlo do pogreške.

  - **ModuleSize –** veličina neispravnog modula u bajtovima.

  - **PreviousBuild** – prethodno instalirana međuverzija

  - **UAEOSEnvironment –** identifikator okruženja operacijskog sustava.

  - **VerifyElseCrashTag –** jedinstveni identifikator mjesta na kojem se aplikacija srušila.

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

  - **RejectedConfigsList** – popis odbijenih konfiguracija na kojem su vrijednosti razdvojene zarezom.

### <a name="officetelemetrydynamicconfigparsejsonconfig"></a>Office.Telemetry.DynamicConfig.ParseJsonConfig

Podaci potrebni za mjerenje stanja servisa za konfiguraciju telemetrije

Prikupljaju se sljedeća polja:

  - **ErrorMessage** – poruka o pogrešci s raščlanjivanjem

  - **NodeName** – čvor koji se nije uspio raščlaniti

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

<!-- end list -->

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
