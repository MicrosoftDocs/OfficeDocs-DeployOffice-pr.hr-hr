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
ms.openlocfilehash: 74d827255ddbedb42cbe242229140d2c8eafea66
ms.sourcegitcommit: f8201a088d2b160b6fcec2342e11be0e9ba3d189
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/09/2020
ms.locfileid: "44663165"
---
# <a name="essential-services-for-office"></a>Ključni servisi za Office

> [!IMPORTANT]
> Informacije u ovom članku odnose se na verziju 1904 ili noviju verziju sljedećeg klijentskog softvera sustava Office instaliranog na računalu sa sustavom Windows:
> - Microsoft 365 Apps za velike tvrtke (prethodni naziv: Office 365 ProPlus)
> - Microsoft 365 Apps za male tvrtke (prethodni naziv: Office 365 Business)
> - Microsoft 365 Personal, Microsoft 365 Family i druge verzije sustava Office koje su obuhvaćene pretplatom na Microsoft 365.
> - Računalne aplikacije za Project i Visio koje su obuhvaćene nekim planovima pretplate, kao što su Project tarifa 5 ili Visio tarifa 2.
>
> Informacije se odnose i na verziju 16.28 ili noviju verziju sljedećih aplikacija sustava Office za Mac: Excel, Outlook, OneNote, PowerPoint i Word.

Office se sastoji od klijentskih softverskih aplikacija i povezanih okruženja osmišljenih radi učinkovitijeg stvaranja, komunikacije i suradnje. Premda kao administrator tvrtke ili ustanove možete upravljati brojnim povezanim sučeljima koja su dostupna vama ili vašim korisnicima, neki su servisi ključni za funkcioniranje sustava Office, pa se ne mogu onemogućiti. To je, primjerice, servis za licenciranje, koji potvrđuje da imate odgovarajuću licencu za korištenje sustava Office. Obavezni servisni podaci o tim servisima prikupljaju se i šalju Microsoftu bez obzira na druge konfigurirane postavke zaštite privatnosti. Te podatke možete pogledati pomoću preglednika dijagnostičkih podataka.

Dodatne informacije potražite u sljedećim člancima:

- [Obavezni servisni podaci za Office](required-service-data.md)
- [Korištenje preglednika dijagnostičkih podataka sa sustavom Office](https://support.office.com/article/cf761ce9-d805-4c60-a339-4e07f3182855)
- [Povezana okruženja u sustavu Office](connected-experiences.md)

Ako ste administrator za tvrtku ili ustanovu, možda će vas zanimati i sljedeći članci:

- [Pregled kontrola za zaštitu privatnosti za Microsoft 365 Apps za velike tvrtke](overview-privacy-controls.md)
- [Upotreba postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Microsoft 365 Apps za velike tvrtke](manage-privacy-controls.md)
- [Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office za Mac](mac-privacy-preferences.md)
- [Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office na iOS uređajima](ios-privacy-preferences.md)
- [Korištenje postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Office na Android uređajima](android-privacy-controls.md)

## <a name="list-of-essential-services-for-office"></a>Popis ključnih servisa za Office 

U tablici u nastavku naveden je popis ključnih servisa za Office i opis svakog servisa.

| **Servis**  | **Opis**  |
| ------ | ---- |
| [Provjera autentičnosti](#authentication-events) | Provjera autentičnosti servis je koji obuhvaća više platformi, a služi za provjeru valjanosti identiteta korisnika sustava Office.  Nužan je da biste se mogli prijaviti u Office, aktivirati licencu za Office, pristupiti datotekama pohranjenima u oblaku, a omogućuje i dosljedno sučelje u svim sesijama sustava Office na svim uređajima.    |
| [Klikom do cilja](#click-to-run-events) | "Klikom do cilja" tehnologija je za instalaciju koja se koristi za instaliranje i ažuriranje sustava Office u sustavu Windows. Tehnologija provjerava postoji li nova verzija sustava Office i kad postoji, preuzima je i instalira. Tehnologija "klikom do cilja" otkrit će jesu li vam potrebna ažuriranja sustava Office, uključujući sigurnosna ažuriranja, te će ih preuzeti i instalirati.     |
| [Servis za poboljšanu konfiguraciju (eng. Enhanced Configuration Service, ECS)](#enhanced-configuration-service-ecs-events) | ECS Microsoftu omogućuje da iznova konfigurira instalacije sustava Office bez potrebe za ponovnom implementacijom sustava. Služi za kontroliranje postupnog objavljivanja značajki ili ažuriranja, a učinak objavljivanja prati se na temelju prikupljenih dijagnostičkih podataka. Koristi se i za ublažavanje sigurnosnih problema i problema s performansama neke značajke ili ažuriranja. ECS podržava i promjene konfiguracije povezane s dijagnostičkim podacima da bi se prikupljali odgovarajući događaji. |
| [Licenciranje](#licensing-events)     | Licenciranje je servis u oblaku koji podržava aktivaciju novih instalacija sustava Office te održava licencu na uređajima nakon aktivacije sustava. Servis registrira svaki uređaj i aktivira Office, provjerava status pretplate na Office te upravlja ključevima proizvoda.    |
|[Microsoftovo automatsko ažuriranje (MAU)](#microsoft-autoupdate-mau-events)|Microsoftovo automatsko ažuriranje (MAU) je tehnologija koja se koristi za ažuriranje Microsoftovih aplikacija proizvedenih za macOS, kao što je Office. MAU će otkriti jesu li vam potrebna ažuriranja aplikacije, uključujući sigurnosna ažuriranja, te će ih preuzeti i instalirati.|
|[Sinkronizacija programa OneNote](#onenote-sync-events)|OneNote za Mac podržava samo bilježnice pohranjene na internetu na servisu OneDrive ili u sustavu SharePoint Online. OneNote za Mac kontinuirano sinkronizira sve bilješke korisnika sa servisom OneDrive ili sustavom SharePoint Online. To korisnicima omogućuje otvaranje, pregled i uređivanje bilježnica na svim svojim uređajima tako da su njihove bilježnice uvijek ažurne.
 [Konfiguracija servisa](#services-configuration-events)  | Konfiguracija servisa omogućuje ažuriranje postavki konfiguracije sustava Office radi omogućivanja odnosno onemogućivanja značajki klijenata. Aktivira se svaki put kad se pokrene neka aplikacija sustava Office te sadrži pojedinosti o drugim konfiguracijama i servisima sustava Office. Konfiguracija servisa ujedno kontrolira koji su servisi određeni kao ključni.  |
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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_CorruptionChecksOnly –** označava radi li se samo o traženju oštećenja bez ažuriranja

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_TaskState –** stanje u kojem je zadatak, primjerice pokrenut ili otkazan 

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

  - **Data\_IsForeGroundStreaming**  – označava prenosimo li podatke strujanjem u prvom planu ili u pozadini

  - **Data\_IsInstallMode** – ako instaliramo i preuzimamo datoteke, vrijednost je 1, a ako ne, vrijednost je 0

  - **Data\_SourceProtocol –** označava preuzimamo li iz mreže podataka sadržaja (CDN-a), s računala na koje instaliramo, iz lokalne mreže ili iz resursa u lokalnoj područnoj mreži.

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


### <a name="officeclicktorununiversalbootstrapperapplication"></a>Office.ClickToRun.UniversalBootstrapper.Application

Prijavljuje rezultat sveobuhvatnih pokušaja instalacije

 - **ErrorCode –**    vrijednost cijelog broja povezana je s neobrađenom iznimkom

 - **ErrorDetails –**    Niz koji opisuje mjesto na kojem se desila neobrađena iznimka (funkcija, datoteka, broj retka, dodatni parametri koje je postavio bacač)

 - **ErrorMessage –**    Niz definiran na mjestu izbacivanja neobrađene iznimke, opisujući prirodu neuspjeha

 - **ErrorType –**    niz koji opisuje kategoriju neobrađene iznimke

 - **ExitCode –**    vrijednost cijelog broja povezana s rezultatom pokretanja automatskog pokretanja, ukazuje na uspjeh nasuprot određenim vrstama neuspjeha

### <a name="officeclicktorununiversalbootstrappercalculateparameters"></a>Office.ClickToRun.UniversalBootstrapper.CalculateParameters

Izvješćuje o radnji koja je razlog unosa prikupljenog pomoću CollectParameters

- **BitField –**    Vrijednost cijelog broja argumenta BitField koji nam  govori je li zatražena eksplicitna instalacija/nadogradnja kanala. Na primjer, beta kanal, trenutačni kanal (pretpregled), trenutačni kanal, mjesečni kanal za velike tvrtke, polugodišnji kanal za velike tvrtke (pretpregled) ili polugodišnji kanal za velike tvrtke.

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
 
- **ErrorCode –**    cijeli broj povezan je s neobrađenom iznimkom

- **ErrorDetails –**    Niz koji opisuje mjesto na kojem se desila neobrađena iznimka (funkcija, datoteka, broj retka, dodatni parametri koje je postavio bacač)

- **ErrorMessage –**    Niz definiran na mjestu izbacivanja neobrađene iznimke, opisujući prirodu neuspjeha

- **ErrorType –**    niz koji opisuje kategoriju neobrađene iznimke

### <a name="officeclicktorununiversalbootstrappercollectparameters"></a>Office.ClickToRun.UniversalBootstrapper.CollectParameters

Izvješćuje o parametrima koji se koriste za instalaciju sustava Office

- **BitField –**    Vrijednost cijelog broja argumenta BitField koji nam  govori je li zatražena eksplicitna instalacija/nadogradnja kanala. Na primjer, beta kanal, trenutačni kanal (pretpregled), trenutačni kanal, mjesečni kanal za velike tvrtke, polugodišnji kanal za velike tvrtke (pretpregled) ili polugodišnji kanal za velike tvrtke.

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

- **DeliveryMechanism –**   „FFNRoot” guid izdvojen iz verzije Deskriptora XML (koju je izdao RDX), koji nam govori iz koje publike/kanala potječe izvor za izgradnju

- **DownloadC2RClientAction –**    „true” ako se planira pokretanje zadatka DownloadC2RClientAction tijekom ove instalacije

- **ErrorCode –**    vrijednost cijelog broja povezana je s neobrađenom iznimkom

- **ErrorDetails –**    Niz koji opisuje mjesto na kojem se desila neobrađena iznimka (funkcija, datoteka, broj retka, dodatni parametri koje je postavio bacač)

- **ErrorMessage –**    Niz definiran na mjestu izbacivanja neobrađene iznimke, opisujući prirodu neuspjeha

- **ErrorType –**    niz koji opisuje kategoriju neobrađene iznimke

- **ExitCode –**   Vrijednost cijelog broja  povezana s rezultatom pokretanja automatskog pokretanja, ukazuje na uspjeh nasuprot određenim vrstama neuspjeha

- **LaunchAction –**    "true" ako se planira pokretanje zadatka LaunchAction tijekom instalacije

- **LaunchUpdateAction –**    „true” ako se planira pokretanje zadatka LaunchUpdateAction tijekom instalacije

- **PreReqResult –**    Vrijednost cijelog broja identifikatora rezultata kada su izvedene provjere bez preduvjeta (prolaz/pad/ponovno pokretanje)

- **UnexpectedAction –**    "true" ako se planira pokretanje zadatka (slučaja pogreške) UnexpectedAction tijekom instalacije

- **VersionToInstall –**   Vrijednost niza verzije sustava Office "16.0.xxxxx.yyyyy" koja se instalira

### <a name="officeserviceabilitymanagerinventoryaddonheartbeat"></a>Office.ServiceabilityManager.InventoryAddon.Heartbeat

*[Ovaj je događaj uklonjen iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

Taj se događaj koristi za pribavljanje standardnih meta-podataka pri svakom pokretanju dodatka Inventar, koji je dio Upravitelja za Office servisiranje i koristi se za informacije o Office inventaru na onim strojevima koje je IT administrator uključio. Meta-podatak od posebnog zanimanja u ovom slučaju je ID sesije, a koristi se za povezivanje s drugim podacima pohranjenima unutar usluge na oblaku po klijentu.

Ovaj događaj nema dodatnih polja jer su relevantni samo meta-podaci.

### <a name="officeserviceabilitymanagerinventoryaddonresults"></a>Office.ServiceabilityManager.InventoryAddon.Results

Taj se događaj bilježi kada se poziv na web-servis u sklopu dodatka "klikom do cilja" za inventar upravitelja za servis dovrši, neovisno o tome uspijeva li ili ne uspijeva. To je u suštini posljednja operacija unutar dodatka za praćenje ukupnog stanja rada.

Prikupljaju se sljedeća polja:

-  **WebCallSource** – vrijednost za numeriranje (koja se određuje kao cijeli broj) koja označava dodatak upravitelja servisa koji je bio izvor poziva:
   - Zalihe: 0
   - Konfiguriranje zaliha: 1
   - Pravilnik o zalihama: 2
   - Stanje mreže zaliha: 3

- **Rezultat** - brojčana oznaka pogreške koju vraćaju API-jevi poziva web-servisa sustava Office.

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
 
- **ConfigParam** – konfiguracija za koju se pristupa vrijednostima za

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

Ako zatvorimo/srušimo Office zbog problema s licenciranjem, šaljemo ovaj signal da bismo to naznačili.  Ključno je radi otkrivanja je li korisnik u dobrom stanju te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom

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

### <a name="officelicensingnextuserlicensingeligible"></a>Office.Licensing.NextUserLicensingEligible 

Taj signal označava je li korisnik kvalificiran za premještanje na novi stog za licenciranje. To je ključno za kvantifikaciju učinka na postojeće korisnike tijekom uvođenja novog stoga za licenciranje i da korisnici ne bi izgubili funkcionalnost.

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

Ako je korisnik u načinu rada za aktivaciju na zajedničkom računalu, pokušavamo potražiti token sesije na računalu koji korisniku omogućuje upotrebu aplikacije. Ovaj događaj prijavljuje uspjeh ili pogrešku tog scenarija, te šifru pogreške. Ključan je za otkrivanje je li korisnik u dobrom stanju, te da mu ne nedostaje neka funkcija, koristi se u svrhe određivanja stanja sustava i za dijagnostiku ako korisnik prijavi problem s računalom.

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

OEM-ovi prodaju strojeve koji isporučuju sa sustavom Office (jednogodišnja ili neprekidna pretplata).  Ti se proizvodi sustava Office plaćaju kada kupac kupi uređaj. Strojevi koje se podešava pomoću određenog regkey-a (OOBEMode: OBIS) možda imaju povezane obveze sustava Office.  Prilikom dizanja sustava Office na takvim strojevima obavljamo servisne provjere da bismo saznali je li pronađena obveza sustava Office koja odgovara stroju.

Ta telemetrijska aktivnost prati točke uspjeha i neuspjeha u traženju povezivanja da bismo mogli osigurati da ih strojevi koji imaju obveze mogu uspješno dohvatiti i da su naši servisi zdravi.  Ta aktivnost ne prati strojeve bez obveza koji nisu povezani s njima kada provjerimo naše servise.

Prikupljaju se sljedeća polja:

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

- **ActionCreateAccount**- korisnik je odabrao da stvori račun.

- **ActionSignIn**- korisnik je odabrao prijavu.

- **DialogRedemption**-prikazuje dijaloški okvir za AFO otkup.

- **DialogSignIn**- prikazuje dijaloški okvir za prijavu u AFO.

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

- **InAppTrialPurchase** – upućuje na to je li za pokretanje SDK za kupnju u trgovini omogućeno snimanje PI-a i kupnja iz probne aplikacije

- **IsRS1OrGreater** – upućuje na to je li verzija sustava veća od RS1 ili ne, jer se SDK za kupnju u trgovini može koristiti samo ako je verzija OS-a veća od RS1

- **NotInitializedBeforeWhileAdding** – to je samo informativno i govori da je događaj dodan u mapu telemetrijskog upravitelja bez eksplicitnog registriranja za nju

- **OEMSendToWebForTrial** – upućuje na to je li omogućen let za slanje korisnika na web radi iskorištavanja probne verzije

- **StoreErrorConditions** – upućuje na različite uvjete u kojima je SDK za kupnju u trgovini možda neuspio

- **StoreErrorHResult**- upućuje na kôd pogreške vraćen iz SDK za kupnju u trgovini

- **StorePurchaseStatusResult** – daje rezultat poziva SDK za kupnju u trgovini i je li korisnik obavio kupnju ili nije, što će pomoći odrediti hoće li korisnik imati licencu za korištenje sustava Office

- **Tag** – koristi se za određivanje mjesta u kodu s kojeg je poslan događaj

- **UserSignedInExplicitly** – govori je li se korisnik potpisao eksplicitno, jer ćemo u tom slučaj, ponovno usmjeriti korisnike na web za probnu verziju

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

### <a name="appdelegate_launch"></a>appdelegate_launch

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


### <a name="appdelegate_terminate"></a>appdelegate_terminate

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


### <a name="appinstall_connecttoxpc"></a>appinstall_connecttoxpc

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


### <a name="appregistry_info"></a>appregistry_info

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


### <a name="appregistry_remove"></a>appregistry_remove

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


### <a name="catalog_errorsignature"></a>catalog_errorsignature

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


### <a name="cloningtask_helpertoolconnection"></a>cloningtask_helpertoolconnection

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


### <a name="configuration_channel"></a>configuration_channel

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


### <a name="configuration_metadata"></a>configuration_metadata

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


### <a name="controller_alertmanager_reinstallresponse"></a>controller_alertmanager_reinstallresponse

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

    
### <a name="controller_alertmanager_tmpdiskfull"></a>controller_alertmanager_tmpdiskfull

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


### <a name="controller_alertmanager_tmpdiskfullretry"></a>controller_alertmanager_tmpdiskfullretry

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
    

### <a name="controller_alertmanager_tmpdiskfullretrycancel"></a>controller_alertmanager_tmpdiskfullretrycancel

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

    
### <a name="controller_checkwindow_noupdatefoundok"></a>controller_checkwindow_noupdatefoundok

Ovaj događaj označava da je provjera ažuriranja rezultirala time da nije pronađeno nijedno ažuriranje. Koristimo ovaj događaj za osiguravanje ispravne ponude ažuriranja, optimiziranje opterećenja usluge i definiranje koliko učestale bi trebale biti provjere ažuriranja. Također želimo optimizirati naš ritam izdanja na temelju očekivanja korisnika o ažuriranjima.

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

    

### <a name="controller_checkwindow_updatecheck"></a>controller_checkwindow_updatecheck

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


### <a name="controller_checkwindow_updatecheckcancel"></a>controller_checkwindow_updatecheckcancel

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

    
### <a name="controller_checkwindow_updatecheckcanceluser"></a>controller_checkwindow_updatecheckcanceluser

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

    
### <a name="controller_checkwindow_updatesfound"></a>controller_checkwindow_updatesfound

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

    
### <a name="controller_checkwindow_uptodate"></a>controller_checkwindow_uptodate

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


### <a name="controller_downloadwindow_applaunchwithpendingupdate"></a>controller_downloadwindow_applaunchwithpendingupdate

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

    
### <a name="controller_downloadwindow_closeapplicationdialog"></a>controller_downloadwindow_closeapplicationdialog

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

    
### <a name="controller_downloadwindow_curtasknull"></a>controller_downloadwindow_curtasknull

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

    
### <a name="controller_downloadwindow_downloadcancel"></a>controller_downloadwindow_downloadcancel

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

    
### <a name="controller_downloadwindow_downloadfailed"></a>controller_downloadwindow_downloadfailed

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

    
### <a name="controller_downloadwindow_downloadfailedok"></a>controller_downloadwindow_downloadfailedok

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


### <a name="controller_downloadwindow_downloadpathmissing"></a>controller_downloadwindow_downloadpathmissing

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


### <a name="controller_downloadwindow_downloadtasknull"></a>controller_downloadwindow_downloadtasknull

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


### <a name="controller_downloadwindow_filesignaturenotverified"></a>controller_downloadwindow_filesignaturenotverified

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


### <a name="controller_downloadwindow_installcomplete"></a>controller_downloadwindow_installcomplete

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


### <a name="controller_downloadwindow_networkunavailablealert"></a>controller_downloadwindow_networkunavailablealert

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

    
### <a name="controller_downloadwindow_networkunavailablealertok"></a>controller_downloadwindow_networkunavailablealertok

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

    
### <a name="controller_downloadwindow_noconnectionok"></a>controller_downloadwindow_noconnectionok

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


### <a name="controller_downloadwindow_repairrequired"></a>controller_downloadwindow_repairrequired

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

### <a name="controller_downloadwindow_updateaborted"></a>controller_downloadwindow_updateaborted

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


### <a name="controller_downloadwindow_updatefailed"></a>controller_downloadwindow_updatefailed

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


### <a name="controller_downloadwindow_updatesuccessful"></a>controller_downloadwindow_updatesuccessful

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


### <a name="controller_downloadwindow_userpaused"></a>controller_downloadwindow_userpaused

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


### <a name="controller_downloadwindow_userresumed"></a>controller_downloadwindow_userresumed

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


### <a name="controller_mainwindow_setautomaticdownloadinstall"></a>controller_mainwindow_setautomaticdownloadinstall

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

    
### <a name="controller_mainwindow_setmanualchecking"></a>controller_mainwindow_setmanualchecking

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

    
### <a name="controller_templateawindow_cancel"></a>controller_templateawindow_cancel

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

    
### <a name="controller_templateawindow_enroll"></a>controller_templateawindow_enroll

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



### <a name="controller_templateawindow_install"></a>controller_templateawindow_install

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


### <a name="controller_updatewindow_begindownloadingapps"></a>controller_updatewindow_begindownloadingapps

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

    
### <a name="controller_updatewindow_networkretry"></a>controller_updatewindow_networkretry

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

    
### <a name="controller_updatewindow_networkretrycancel"></a>controller_updatewindow_networkretrycancel

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


### <a name="controller_updatewindow_networkunavailable"></a>controller_updatewindow_networkunavailable

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


### <a name="controller_updatewindow_noupdateavailable"></a>controller_updatewindow_noupdateavailable

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


### <a name="controller_updatewindow_noupdatestoselect"></a>controller_updatewindow_noupdatestoselect

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


### <a name="controller_updatewindow_updateavailable"></a>Controller_UpdateWindow_UpdateAvailable

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

    
### <a name="controller_updatewindow_updateavailablecancel"></a>controller_updatewindow_updateavailablecancel

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


### <a name="downloadactor_pause"></a>downloadactor_pause

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


### <a name="downloadactor_redirect"></a>downloadactor_redirect

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

    
### <a name="downloadactor_resume"></a>downloadactor_resume

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


### <a name="downloadactor_resumeerror"></a>downloadactor_resumeerror

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

    
### <a name="downloadactor_status"></a>downloadactor_status

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


### <a name="downloadmanifest_downloadcatalogfail"></a>downloadmanifest_downloadcatalogfail

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

    
### <a name="downloadmanifest_downloadcatalogsuccess"></a>downloadmanifest_downloadcatalogsuccess

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


### <a name="downloadmanifest_downloadfail"></a>downloadmanifest_downloadfail

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


### <a name="downloadmanifest_downloadfromurl"></a>downloadmanifest_downloadfromurl

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


### <a name="downloadmanifest_downloading"></a>downloadmanifest_downloading

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


### <a name="downloadmanifest_downloadsuccess"></a>downloadmanifest_downloadsuccess

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

    
### <a name="downloadmanifest_downloadurl"></a>downloadmanifest_downloadurl

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


### <a name="downloadmanifest_filenameerror"></a>downloadmanifest_filenameerror

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


### <a name="downloadmanifest_invalidhash"></a>downloadmanifest_invalidhash

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


### <a name="downloadmanifest_missingdaemon"></a>downloadmanifest_missingdaemon

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


### <a name="downloadmanifest_signatureerror"></a>downloadmanifest_signatureerror

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


### <a name="downloadmanifest_status"></a>downloadmanifest_status

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


### <a name="downloadmgr_downloadend"></a>downloadmgr_downloadend

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


### <a name="downloadmgr_downloadstart"></a>downloadmgr_downloadstart

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


### <a name="downloadtask_downloadfailure"></a>downloadtask_downloadfailure

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


### <a name="downloadtask_downloadsuccess"></a>downloadtask_downloadsuccess

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


### <a name="fba_checkforupdate"></a>fba_checkforupdate

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


### <a name="fba_checkforupdateskip"></a>fba_checkforupdateskip

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


### <a name="fba_launchstatus"></a>fba_launchstatus

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

### <a name="fba_silentupdateoptin"></a>fba_silentupdateoptin

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


### <a name="fba_skipforcedupdate"></a>fba_skipforcedupdate

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


### <a name="fba_startforcedupdate"></a>fba_startforcedupdate

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


### <a name="fba_terminate"></a>fba_terminate

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


### <a name="fba_updatefound"></a>fba_updatefound

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

    
### <a name="fba_updatetimer"></a>fba_updatetimer

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


### <a name="fbasilentupdate_allappsclosed"></a>fbasilentupdate_allappsclosed

Ovaj događaj evidentira ako su sve aplikacije bile zatvorene prije instalacije. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
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


### <a name="fbasilentupdate_applaunchafterupdate"></a>fbasilentupdate_applaunchafterupdate

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


### <a name="fbasilentupdate_applaunchwileinstalling"></a>fbasilentupdate_applaunchwileinstalling

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


### <a name="fbasilentupdate_appneedtoclose"></a>fbasilentupdate_appneedtoclose

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


### <a name="fbasilentupdate_appterminationeventreceived"></a>fbasilentupdate_appterminationeventreceived

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


### <a name="fbasilentupdate_codesignfailure"></a>fbasilentupdate_codesignfailure

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


### <a name="fbasilentupdate_download"></a>fbasilentupdate_download

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

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdate_downloadfailed"></a>fbasilentupdate_downloadfailed

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


### <a name="fbasilentupdate_downloadinbackground"></a>fbasilentupdate_downloadinbackground

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


### <a name="fbasilentupdate_downloadingrepairupdate"></a>fbasilentupdate_downloadingrepairupdate

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

- **SessionId** – Identifikator sesije


### <a name="fbasilentupdate_duplicatedownloadattempted"></a>fbasilentupdate_duplicatedownloadattempted

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


### <a name="fbasilentupdate_installattemptfailed"></a>fbasilentupdate_installattemptfailed

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


### <a name="fbasilentupdate_installcomplete"></a>fbasilentupdate_installcomplete

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


### <a name="fbasilentupdate_installed"></a>fbasilentupdate_installed

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

    
### <a name="fbasilentupdate_installing"></a>fbasilentupdate_installing

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


### <a name="fbasilentupdate_notificationremoved"></a>fbasilentupdate_notificationremoved

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


### <a name="fbasilentupdate_queueinstall"></a>fbasilentupdate_queueinstall

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


### <a name="fbasilentupdate_requiredappsclosed"></a>fbasilentupdate_requiredappsclosed

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


### <a name="fbasilentupdate_updateavailablenotification"></a>fbasilentupdate_updateavailablenotification

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


### <a name="fbasilentupdate_userclicknotification"></a>fbasilentupdate_userclicknotification

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


### <a name="fbasilentupdate_userselectinstalllater"></a>fbasilentupdate_userselectinstalllater

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


### <a name="fbasilentupdate_userselectinstallnow"></a>fbasilentupdate_userselectinstallnow

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


### <a name="installdata_checkrunning"></a>installdata_checkrunning

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

    
### <a name="installdata_cleanup"></a>installdata_cleanup

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


### <a name="installedapp_invalidbundle"></a>installedapp_invalidbundle

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

    
### <a name="installedapp_invalidpreference"></a>installedapp_invalidpreference

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

    
### <a name="installedapp_nilbundleid"></a>installedapp_nilbundleid

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


### <a name="installedapp_nilbundlename"></a>installedapp_nilbundlename

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

    
### <a name="installstatus_codesign"></a>installstatus_codesign

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


### <a name="installstatus_daemon"></a>installstatus_daemon

Ovaj događaj evidentira stanje statusa daemona Microsoftova automatskog ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
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


### <a name="installstatus_helper"></a>installstatus_helper

Ovaj događaj evidentira stanje statusa pomoćnog alata Microsoftova automatskog ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
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

    
### <a name="installupdatestask_applaunched"></a>installupdatestask_applaunched

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

    
### <a name="installupdatestask_applaunchwithpendingupdate"></a>installupdatestask_applaunchwithpendingupdate

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

    
### <a name="installupdatestask_codesignverificationfail"></a>installupdatestask_codesignverificationfail

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


### <a name="installupdatestask_codesignverificationstart"></a>installupdatestask_codesignverificationstart

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


### <a name="installupdatestask_codesignverificationsuccess"></a>installupdatestask_codesignverificationsuccess

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


### <a name="installupdatestask_failsilentinstall"></a>installupdatestask_failsilentinstall

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

    
### <a name="installupdatestask_multiplerelocatablepackage"></a>installupdatestask_multiplerelocatablepackage

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

    
### <a name="installupdatestask_removeclone"></a>installupdatestask_removeclone

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


### <a name="installupdatestask_retryfail"></a>installupdatestask_retryfail

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


### <a name="installupdatestask_retryproxyerror"></a>installupdatestask_retryproxyerror

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

    
### <a name="installupdatestask_retryproxyerror"></a>installupdatestask_retryproxyerror

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

    

### <a name="installupdatestask_retryresponse"></a>installupdatestask_retryresponse

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


### <a name="installupdatestask_retrysuccess"></a>installupdatestask_retrysuccess

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


### <a name="installupdatestask_setreopengui"></a>installupdatestask_setreopengui

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


### <a name="msupdate_cli_eventhandler_applyupdates_appids"></a>msupdate_cli_eventhandler_applyupdates_appids

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


### <a name="msupdate_cli_eventhandler_config"></a>msupdate_cli_eventhandler_config

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


### <a name="msupdate_cli_eventhandler_updates"></a>msupdate_cli_eventhandler_updates

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

    
### <a name="msupdate_monitor_progress_downloaded"></a>msupdate_monitor_progress_downloaded

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


### <a name="msupdate_monitor_progress_failure"></a>msupdate_monitor_progress_failure

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

    
### <a name="msupdate_monitor_progress_finished"></a>msupdate_monitor_progress_finished

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


### <a name="msupdate_monitor_progress_queued"></a>msupdate_monitor_progress_queued

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


### <a name="updatecore_appregistration"></a>updatecore_appregistration

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


### <a name="updatecore_loadinglaunchagent"></a>updatecore_loadinglaunchagent

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


### <a name="updatecore_server_connectionfail"></a>updatecore_server_connectionfail

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


### <a name="updatefilterhelper_cannotretrievebuilddate"></a>updatefilterhelper_cannotretrievebuilddate

Možemo filtrirati ažuriranja putem usluge MAU samo ako ažuriranje koje se nudi nije starije od određenog broja dana. Ovdje evidentiramo kako nismo mogli dohvatiti datum iz metapodataka aplikacije. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
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


### <a name="updatefilterhelper_invalidresponsefromupdatefiltering"></a>updatefilterhelper_invalidresponsefromupdatefiltering

Možemo filtrirati ažuriranja putem usluge MAU samo ako ažuriranje koje se nudi nije starije od određenog broja dana. Ovdje evidentiramo da iz metapodataka aplikacije nedostaje datum. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
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


### <a name="updatefilterhelper_missingbuilddate"></a>updatefilterhelper_missingbuilddate

Možemo filtrirati ažuriranja putem usluge MAU samo ako ažuriranje koje se nudi nije starije od određenog broja dana. Ovdje evidentiramo da iz metapodataka aplikacije nedostaje datum. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
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


### <a name="updatefilterhelper_updatebypassedoldage"></a>updatefilterhelper_updatebypassedoldage

Možemo filtrirati ažuriranja putem usluge MAU samo ako ažuriranje koje se nudi nije starije od određenog broja dana. Ovdje evidentiramo da je usluga zaobiđena zbog starog datuma ažuriranja. Ovaj događaj koristimo za osiguravanje da postupak ažuriranja funkcionira kako se očekuje i da pomogne u rješavanju pogrešaka.
 
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


### <a name="updatefinder_check_start"></a>updatefinder_check_start

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


### <a name="updatefinder_check_status"></a>updatefinder_check_status

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


### <a name="updatefinder_check_updatefound"></a>updatefinder_check_updatefound

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


### <a name="updatefinder_check_updatenotfound"></a>updatefinder_check_updatenotfound

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


### <a name="updatefinder_check_uptodate"></a>updatefinder_check_uptodate

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


### <a name="updatefinder_offerupdates_minoscheckfail"></a>updatefinder_offerupdates_minoscheckfail

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


### <a name="updatefinder_offerupdates_nullbundleforappid"></a>updatefinder_offerupdates_nullbundleforappid

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


### <a name="updatefinder_offerupdates_updaterulematched"></a>updatefinder_offerupdates_updaterulematched

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

    
### <a name="updatefinder_registeredapps"></a>updatefinder_registeredapps

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

    
### <a name="updatefinder_suite_missingcollateral"></a>updatefinder_suite_missingcollateral

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


### <a name="updatefinder_suite_staleversion"></a>updatefinder_suite_staleversion

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


### <a name="updatefinder_suite_updateapplicable"></a>updatefinder_suite_updateapplicable

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


### <a name="updatefinder_suite_updatenotapplicabledefaultpath"></a>updatefinder_suite_updatenotapplicabledefaultpath

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

    
### <a name="updatefinder_suite_updatenotapplicableversion"></a>updatefinder_suite_updatenotapplicableversion

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


### <a name="updatefinder_suite_updatenotoffered"></a>updatefinder_suite_updatenotoffered

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


### <a name="updatefinder_suite_updateoffered"></a>updatefinder_suite_updateoffered

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


### <a name="updatemanager_checkupdate"></a>updatemanager_checkupdate

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

    
### <a name="updatemanager_updatespending"></a>updatemanager_updatespending

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

    
### <a name="webservices_checkforsilentupdates"></a>webservices_checkforsilentupdates

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


### <a name="webservices_deltaupdater"></a>webservices_deltaupdater

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


### <a name="webservices_serviceaction"></a>webservices_serviceaction

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


### <a name="webservices_serviceaction"></a>webservices_serviceaction

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


### <a name="webservices_serviceresponse"></a>webservices_serviceresponse

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

    
### <a name="webservices_silentupdate"></a>webservices_silentupdate

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



### <a name="webservices_webcontent"></a>webservices_webcontent

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

Konfiguracija servisa ne prikuplja događaje vezane uz obavezne servisne dijagnostičke podatke.

## <a name="telemetry-events"></a>Telemetrijski događaji

### <a name="office_firstrun_apple_telemetryoptin"></a>Office_FirstRun_Apple_TelemetryOptIn

Ovaj se događaj prikuplja za aplikacije sustava Office koje rade na Apple platformama. Događaj se koristi za nadziranje stanja telemetrijske funkcije uključivanja u iskustvo prvog pokretanja. Prikupljamo kôd koji označava vrstu mogućnosti za prikupljanje dijagnostičkih podataka koju je korisnik odabrao.

Prikupljaju se sljedeća polja:

 - **Data_EventId** – Kôd koji pokazuje preferenciju prikupljanja podataka koju je odabrao korisnik.


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

Događaj aktivira nenormalno ukidanje aplikacije (npr. zaustavljanje u upravitelju zadataka, prekid aplikacije, itd.) za klijentske aplikacije sustava Office, kao što su, no ne ograničavajući se na, Word, Excel, PowerPoint i Outlook. Parametre neočekivanog zatvaranja aplikacije koristimo za mjerenje stanja proizvoda klijenata sustava Office. To je signal ključan za poslovanje koji inženjeri sustava Office koriste za postizanje stabilnosti proizvoda.

Prikupljaju se sljedeća polja:

  - **AddinExecution –** Zastavica koja obavještava je li izvršavanje dodatka prekinuto prilikom neočekivanog izlaska iz aplikacije.

  - **BootCompleted –** je li dovršeno pokretanje sustava Office u trenutku rušenja.

  - **CrashedAppBuild –** identifikator međuverzije zahvaćenog procesa.

  - **CrashedAppMajor –** identifikator glavne verzije zahvaćenog procesa.

  - **CrashedAppMinor –** identifikator sporedne verzije zahvaćenog procesa.

  - **CrashedAppRevision –** identifikator međuverzije zahvaćenog procesa.

  - **CrashedEcsETag –** identifikator eksperimenta za srušeni proces.

  - **CrashedModuleName –** naziv neispravnog modula.

  - **CrashedSessionId –** jedinstveni identifikator srušenog procesa.

  - **CrashedSessionInitTime –** vrijeme pokretanja zahvaćenog procesa.

  - **CrashTime –** vrijeme koje ukazuje da je klijent neočekivano prekinut.

  - **CrashType –** identifikator grupiranja za vrstu rušenja.

  - **DetectionTime –** vrijeme otkrivanja neočekivanog zatvaranja.

  - **ExceptionAddress –** adresa u programu na kojoj je došlo do pogreške.

  - **ExceptionCode –** identifikator grupiranja za iznimku.

  - **HandOff –** je li korisnik stvorio i predao Officeov postupak novoj sesiji.

  - **HasEdit –** je li korisnik uređivao dokument u srušenom klijentu.

  - **HasOpen –** je li dokument bio otvoren u srušenom klijentu.

  - **HexCrashTag –**  Jedinstveni identifikator kôda rušenja.

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

  - **OfficeArchitectureText –** Arhitektura proizvoda sustava Office predstavljena kao niz (npr. x86, arm).

  - **OfficeUILang –** jezik korisničkog sučelja u međuverziji sustava Office.

  - **PreviousBuild** – prethodno instalirana međuverzija

  - **SafeMode –** je li sesija bila pokrenuta u sigurnom načinu rada.

  - **UAEOSEnvironment –** identifikator okruženja operacijskog sustava.

  - **UninitLibletId –** Jedinstveni identifikator za neispravnu komponentu rušenja.

  - **VerifyElseCrashTag –** jedinstveni identifikator mjesta na kojem se aplikacija srušila. *[Ovo je polje uklonjeno iz trenutačnih međuverzija sustava Office, ali se i dalje može pojavljivati u starijim međuverzijama.]*

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
