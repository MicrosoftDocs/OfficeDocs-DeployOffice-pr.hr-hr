---
title: Korištenje postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Office 365 ProPlus
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
audience: ITPro
ms.topic: article
ms.service: o365-proplus-itpro
localization_priority: Priority
ms.collection:
- Ent_O365
- M365-modern-desktop
ms.custom:
- Ent_Office_ProPlus
- Ent_Office_Privacy
description: Administratorima sustava Office nudi informacije o upravljanju kontrolama za zaštitu privatnosti u sustavu Office 365 ProPlus pomoću postavki pravilnika.
hideEdit: true
ms.openlocfilehash: 5f3b63c65d43827befe58ba600c7957410f2d3c0
ms.sourcegitcommit: 02c4120c0b10bfe378d21d60699ae49aaef97834
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/15/2019
ms.locfileid: "37510252"
---
# <a name="use-policy-settings-to-manage-privacy-controls-for-office-365-proplus"></a>Korištenje postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Office 365 ProPlus

Microsoft predano radi na tome da vam pruži informacije i kontrole potrebne da biste mogli odabrati načine prikupljanja i korištenja podataka o vama prilikom korištenja sustava Office 365 ProPlus.

Počevši od verzije 1904 sustava Office 365 ProPlus, postoje nove postavke pravilnika koje omogućuju kontrolu nad postavkama vezanima uz sljedeće:

- ***Dijagnostičke podatke*** o klijentskom softveru sustava Office, koji se prikupljaju i šalju Microsoftu.

- ***Povezana iskustva*** koja koriste funkcije utemeljene na oblaku da bi vama i vašim korisnicima ponudila poboljšane značajke sustava Office.

Ovo je pet novih postavki pravilnika:

- konfiguriranje razine dijagnostičkih podataka o klijentskom softveru koje Office šalje Microsoftu
- dopusti korištenje povezanih iskustava koja analiziraju sadržaj u sustavu Office 
- dopusti korištenje povezanih iskustava koja preuzimaju internetski sadržaj u sustavu Office 
- dopusti korištenje dodatnih neobaveznih povezanih iskustava u sustavu Office
- dopusti korištenje povezanih iskustava u sustavu Office

Postavke pravilnika mogu se implementirati putem pravilnika grupe ili [servisa pravilnika u oblaku za Office](https://docs.microsoft.com/DeployOffice/overview-office-client-policy-service). Ako koristite pravilnik grupe, morat ćete preuzeti najnoviju verziju datoteka administrativnih predložaka (ADMX/ADML) iz [Microsoftovog centra za preuzimanje](https://www.microsoft.com/download/details.aspx?id=49030).

> [!NOTE]
> - Informacije o načinu upravljanja kontrolama zaštite privatnosti za Office za Mac potražite u članku [Korištenje preferenci za upravljanje kontrolama zaštite privatnosti za Office za Mac](mac-privacy-preferences.md).
> - Informacije o sličnim postavkama za Office na iOS uređajima potražite [Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office na iOS uređajima](ios-privacy-preferences.md).


Ako koristite alat za upravljanje pravilnikom grupe, sve postavke pravilnika nalaze se u odjeljku Konfiguracija korisnika\\Pravilnici\\Administrativni predlošci\\Microsoft Office 2016\\Zaštita privatnosti\\Centar za pouzdanost.

Nove postavke pravilnika primjenjuju se i na verzije programa Project i Visio za računala koje se isporučuju s nekim pretplatničkim tarifama, kao što su Project Online Professional ili Visio Online Plan 2. Primjenjuju se i na Office 365 Business.

Ima i postojećih postavki pravilnika koje se više neće primjenjivati na Office 365 ProPlus, kao i nekih promjena korisničkog sučelja (UI) nastalih zbog postavki zaštite privatnosti, kojih biste trebali biti svjesni jer će ih korisnici možda opaziti te postavljati pitanja u vezi s njima.

Kao što je slučaj sa svim novim postavkama pravilnika, prije nego što šire implementirate postavke pravilnika u svojoj tvrtki ili ustanovi, morate ih pažljivo testirati u ograničenom i kontroliranom okruženju da biste osigurali da postavke koje ste konfigurirali imaju željeni učinak.

## <a name="policy-setting-for-diagnostic-data"></a>Postavka pravilnika za dijagnostičke podatke

Dijagnostički podaci koriste se da bi Office uvijek bio siguran i ažuran, kao i radi otkrivanja, dijagnosticiranja i otklanjanja problema te poboljšavanja proizvoda.

Možete koristiti postavku pravilnika *Konfiguriranje razine dijagnostičkih podataka o klijentskom softveru koje Office šalje Microsoftu* da biste odabrali koja se razina dijagnostičkih podataka šalje Microsoftu.

Ako omogućite tu postavku pravilnika, morate odabrati razinu dijagnostičkih podataka koji se šalju Microsoftu. Dostupni su izbori Obavezno, Neobavezno i Nijedno.

- Ako odaberete ***Obavezno***, Microsoftu se šalju minimalni podaci nužni da bi Office bio siguran i ažuran te da bi na uređaju na kojem je instaliran funkcionirao na očekivan način.

- Ako odaberete ***Neobavezno***, Microsoftu se šalju dodatni podaci koji pomažu pri poboljšavanju proizvoda i pružaju poboljšane informacije za pomoć pri otkrivanju, dijagnosticiranju i otklanjanju problema. Ako odaberete slanje neobaveznih dijagnostičkih podataka, uz njih se prikupljaju i obavezni dijagnostički podaci.

- Ako odaberete ***Nijedno***, Microsoftu se ne šalju nikakvi dijagnostički podaci o klijentskom softveru sustava Office na korisnikovu uređaju. Ta mogućnost, međutim, znatno ograničava Microsoftove mogućnosti vezane uz otkrivanje, dijagnosticiranje i otklanjanje problema na koje vaši korisnici mogu naići prilikom korištenja sustava Office.

Ako onemogućite ili ne konfigurirate tu postavku pravilnika, Microsoftu se šalju i neobavezni i obavezni dijagnostički podaci.

Dodatne informacije o dijagnostičkim podacima potražite u ovim člancima:

- [Pregled kontrola za zaštitu privatnosti za Office 365 ProPlus](overview-privacy-controls.md)
- [Obavezni dijagnostički podaci za Office](required-diagnostic-data.md)
- [Neobavezni dijagnostički podaci za Office](optional-diagnostic-data.md)
- [Korištenje preglednika dijagnostičkih podataka sa sustavom Office](https://support.office.com/article/cf761ce9-d805-4c60-a339-4e07f3182855)

## <a name="policy-settings-for-connected-experiences"></a>Postavke pravilnika za povezana iskustva

Office 365 ProPlus sastoji se od klijentskih softverskih aplikacija i povezanih iskustava osmišljenih radi učinkovitijeg stvaranja, komunikacije i suradnje. Suradnja s drugim korisnicima na dokumentu pohranjenom na servisu OneDrive za tvrtke ili prevođenje sadržaja dokumenta programa Word na neki drugi jezik primjeri su povezanih iskustava.

Razumijemo da možda želite odabrati koje će vrste povezanih iskustava biti dostupne vašim korisnicima prilikom rada u aplikacijama sustava Office. Stoga smo za vas pripremili četiri nove postavke pravilnika:

- dopusti korištenje povezanih iskustava koja analiziraju sadržaj u sustavu Office 
- dopusti korištenje povezanih iskustava koja preuzimaju internetski sadržaj u sustavu Office 
- dopusti korištenje dodatnih neobaveznih povezanih iskustava u sustavu Office
- dopusti korištenje povezanih iskustava u sustavu Office

Ako ne konfigurirate te postavke pravilnika, bit će dostupna sva povezana iskustva. To vašim korisnicima nudi sve značajke i funkcije dostupne putem sustava Office 365 ProPlus. Znamo, međutim, da ćete možda morati isključiti neka ili sva povezana iskustva da biste udovoljili određenim zahtjevima svoje tvrtke ili ustanove.

> [!IMPORTANT]
> Problem povezan s onemogućivanjem te četiri postavke pravilnika nedavno je riješen objavljivanjem novih datoteka administrativnog predloška (ADMX/ADML) u utorak 28. svibnja 2019. Obavezno preuzmite i instalirajte ažurirane datoteke grupnog pravilnika putem [Microsoftova centra za preuzimanje](https://www.microsoft.com/en-us/download/details.aspx?id=49030).

Ako odlučite korisnicima uskratiti određene vrste povezanih iskustava, naredbe tih povezanih iskustava na vrpci ili izborniku bit će zasivljene ili će korisnici dobiti poruku o pogrešci kada pokušaju koristiti ta povezana iskustva. U tom se slučaju Microsoftu ne šalju nikakvi [obavezni servisni podaci](required-service-data.md) za ta povezana iskustva.

Vaši korisnici neće moći odabrati žele li uključiti ili isključiti ta povezana iskustva obuhvaćena sustavom Office 365 ProPlus ako su se prijavili u Office pomoću vjerodajnica svoje tvrtke ili ustanove, koje se ponekad nazivaju računom tvrtke ili obrazovne ustanove.

### <a name="policy-setting-for-connected-experiences-that-analyze-your-content"></a>Postavka pravilnika za povezana iskustva koja analiziraju vaš sadržaj

To su iskustva koja koriste vaš sadržaj iz sustava Office da bi vam ponudila preporuke dizajna, prijedloge za uređivanje, uvid u podatke i slične značajke. Na primjer, PowerPoint Designer ili Redaktor u programu Word. Popis tih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).

Možete koristiti postavku pravilnika *Dopusti korištenje povezanih iskustava koja analiziraju sadržaj u sustavu Office* da biste kontrolirali jesu li povezana iskustva te vrste dostupna vašim korisnicima. Ako ne konfigurirate tu postavku pravilnika, ta će povezana iskustva biti dostupna vašim korisnicima.

Imajte na umu da ako onemogućite postavku pravilnika *Dopusti korištenje povezanih iskustava u sustavu Office*, povezana iskustva koja analiziraju sadržaj neće biti dostupna vašim korisnicima.

### <a name="policy-setting-for-connected-experiences-that-download-online-content"></a>Postavka pravilnika za povezana iskustva koja preuzimaju internetski sadržaj

To su iskustva koja omogućuju pretraživanje i preuzimanje internetskih sadržaja, uključujući predloške, slike, 3D modele, videozapise i referentni materijal, radi poboljšavanja dokumenata. Na primjer, predlošci sustava Office ili alat za brz početak rada s programom PowerPoint. Popis tih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).

Možete koristiti postavku pravilnika *Dopusti korištenje povezanih iskustava koja preuzimaju internetski sadržaj u sustavu Office* da biste kontrolirali jesu li povezana iskustva te vrste dostupna vašim korisnicima. Ako ne konfigurirate tu postavku pravilnika, ta će povezana iskustva biti dostupna vašim korisnicima.

Imajte na umu da ako onemogućite postavku pravilnika *Dopusti korištenje povezanih iskustava u sustavu Office*, povezana iskustva koja preuzimaju internetski sadržaj neće biti dostupna vašim korisnicima.

### <a name="policy-setting-for-optional-connected-experiences"></a>Postavka pravilnika za neobavezna povezana iskustva

Osim gore spomenutih povezanih iskustava obuhvaćenih sustavom Office 365 ProPlus, postoje i neka neobavezna povezana iskustva za koja korisnicima možete omogućiti da im pristupaju korištenjem računa tvrtke ili ustanove. Na primjer, značajke vezane uz LinkedIn u pomoćniku za životopis u programu Word ili značajka 3D karte u programu Excel, koja koristi Bing. Dodatne primjere potražite u članku [Pregled neobaveznih povezanih iskustava za Office](optional-connected-experiences.md).

Ta se povezana iskustva razlikuju po tome što nisu obuhvaćena komercijalnim ugovorom vaše tvrtke ili ustanove s Microsoftom. Neobavezna povezana iskustva Microsoft izravno nudi vašim korisnicima te su ona regulirana [Microsoftovim ugovorom o pružanju usluga](https://www.microsoft.com/servicesagreement), a ne [Uvjetima korištenja internetskih servisa](https://www.microsoft.com/licensing/product-licensing/products). U nekim se slučajevima putem tih neobaveznih povezanih iskustava nudi sadržaj ili funkcije trećih strana te se mogu primjenjivati i drugi uvjeti. Dodatne informacije potražite u članku [Pregled neobaveznih povezanih iskustava za Office](optional-connected-experiences.md).

Možete koristiti postavku pravilnika *Dopusti korištenje dodatnih neobaveznih povezanih iskustava u sustavu Office* da biste kontrolirali jesu li povezana iskustva te vrste dostupna vašim korisnicima. Ako ne konfigurirate tu postavku pravilnika, ta će neobavezna povezana iskustva biti dostupna vašim korisnicima.

> [!NOTE]
> Postavka pravilnika *Dopusti korištenje dodatnih neobaveznih povezanih iskustava u sustavu Office* se može konfigurirati i tako da primjenjuje sljedeće aplikacije za Office for web:
> - Excel za web
> - OneNote za web
> - PowerPoint za web
> - Visio za web
> - Word za web
>
> Te aplikacije Office za web moraju početi koristiti novu kontrolu zaštite privatnosti za neobvezna povezana iskustva u sredinom listopada 2019, ali sada možete konfigurirati postavku pravilnika. Da biste konfigurirali tu postavku pravilnika za te aplikacije za Office za web, morate koristiti uslugu [Office pravilnik o oblaku](../overview-office-cloud-policy-service.md).

Čak i ako odlučite neobavezna povezana iskustva staviti na raspolaganje korisnicima, oni će imati mogućnost isključiti ih kao grupu putem[dijaloškog okvira postavki postavke privatnosti](https://support.office.com/article/3e7bc183-bf52-4fd0-8e6b-78978f7f121b). Korisnicima će se taj izbor pružati samo ako su se prijavili u Office s vjerodajnicama tvrtke ili ustanove (koje se ponekad nazivaju računom tvrtke ili obrazovne ustanove), a ne i ako su se prijavili s osobnom adresom e-pošte.

Uz to, neka od tih neobaveznih povezanih iskustava također se smatraju povezanim iskustvima koja analiziraju sadržaj ili preuzimaju internetski sadržaj. Na primjer, umetanje internetskih slika neobavezno je povezano iskustvo koje omogućuje Microsoft Bing, ali se ujedno smatra i povezanim iskustvom koje preuzima internetski sadržaj. Stoga ako onemogućite postavku pravilnika *Dopusti korištenje povezanih iskustava koja preuzimaju internetski sadržaj u sustavu Office*, umetanje internetskih slika neće biti dostupno vašim korisnicima. Ono im neće biti dostupno čak ni ako ste omogućili postavku pravilnika *Dopusti korištenje dodatnih neobaveznih povezanih iskustava u sustavu Office*. Dodatne informacije o tome koja povezana iskustva analiziraju sadržaj ili preuzimaju internetski sadržaj potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).

Postoji i jedna iznimka na koju treba obratiti pozornost. Postavka pravilnika *Dopusti korištenje dodatnih neobaveznih povezanih iskustava u sustavu Office* ne kontrolira iskustva koja od vas traže povezivanje računa za LinkedIn s Microsoftovim računom tvrtke ili obrazovne ustanove. Informacije o kontroli iskustava te vrste, kao što su informacije sa servisa LinkedIn na [kartici profila](https://support.office.com/article/365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) u programu Outlook, potražite u člancima [Povezivanje računa za LinkedIn i Microsoftovog računa](https://support.office.com/article/dc81cc70-4d64-4755-9f1c-b9536e34d381) i [Pristanak na veze iz računa za LinkedIn u tvrtki ili ustanovi koja koristi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/linkedin-integration).

### <a name="policy-setting-for-most-connected-experiences"></a>Postavka pravilnika za većinu povezanih iskustava

Možete koristiti postavku pravilnika *Dopusti korištenje povezanih iskustava u sustavu Office* da biste kontrolirali je li većina povezanih iskustava kojima se pristupa putem sustava Office 365 ProPlus dostupna vašim korisnicima. Ako onemogućite tu postavku pravilnika, ove vrste povezanih iskustava neće biti dostupne vašim korisnicima:

- iskustva koja analiziraju sadržaj
- iskustva koja preuzimaju internetski sadržaj
- neobavezna povezana iskustva

Uz to, ako onemogućite tu postavku pravilnika, isključuje se i većina drugih povezanih iskustava, kao što su suautorstvo i internetski prostor za pohranu datoteka. Popis tih drugih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).

No čak i ako odlučite onemogućiti tu postavku pravilnika, ostat će dostupna ograničena funkcionalnost sustava Office, pa će tako sinkronizacija poštanskog sandučića u programu Outlook te Teams i Skype za tvrtke i dalje funkcionirati. [Ključni servisi](essential-services.md), poput servisa za licenciranje, koji potvrđuje da imate ispravnu licencu za korištenje sustava Office, također će ostati dostupni.

## <a name="existing-policy-settings-that-are-replaced-by-new-policy-settings"></a>Postojeće postavke pravilnika koje se mijenjaju novim postavkama pravilnika

Dvije se postojeće postavke pravilnika od verzije 1904 više ne primjenjuju na Office 365 ProPlus. Te su postavke pravilnika sljedeće:

- **Slanje osobnih podataka** u odjeljku Konfiguracija korisnika\\Pravilnici\\Administrativni predlošci\\Microsoft Office 2016\\Zaštita privatnosti\\Centar za pouzdanost.

- **Mogućnosti internetskog sadržaja** u odjeljku Konfiguracija korisnika\\Pravilnici\\Administrativni predlošci\\Microsoft Office 2016\\Alati | Mogućnosti | Općenito | Mogućnosti servisa...\\Internetski sadržaj.

Počevši od verzije 1904, konfiguriranje tih dviju postojećih postavki pravilnika neće utjecati na Office 365 ProPlus. One više nisu primjenjive jer je njihova funkcionalnost zamijenjena ovim novim postavkama pravilnika:

- dopusti korištenje povezanih iskustava koja analiziraju sadržaj u sustavu Office 
- dopusti korištenje povezanih iskustava koja preuzimaju internetski sadržaj u sustavu Office 
- dopusti korištenje dodatnih neobaveznih povezanih iskustava u sustavu Office
- dopusti korištenje povezanih iskustava u sustavu Office

Te nove postavke pravilnika nude finiju razinu kontrole od dviju postojećih postavki pravilnika. Primjerice, ako ste ranije koristili postavku pravilnika *Slanje osobnih podataka*, time biste isključili i alat za brz početak rada s programom PowerPoint i pametno traženje. No ako sada, uz nove postavke pravilnika, koristite postavku pravilnika *Dopusti korištenje povezanih iskustava koja analiziraju sadržaj u sustavu Office* da biste isključili tu vrstu povezanih iskustava, time ćete isključiti samo pametno traženje. Brz početak rada s programom PowerPoint i dalje će biti dostupan vašim korisnicima.

Postavke pravilnika još uvijek se prikazuju u alatu za upravljanje pravilnikom grupe jer još uvijek vrijede za količinski licencirane verzije sustava Office 2016 i Office 2019, kao što je Office Professional Plus 2019.

## <a name="what-about-existing-policy-settings-that-control-connected-experiences"></a>Što je s postojećim postavkama pravilnika koje kontroliraju povezana iskustva?

Kao što vjerojatno već znate, neke od postojećih postavki pravilnika omogućuju kontrolu nad povezanim iskustvima. Evo nekoliko primjera postojećih postavki pravilnika:

- *Mogućnosti značajke PowerPoint Designer* u odjeljku Konfiguracija korisnika\\Pravilnici\\Administrativni predlošci\\Microsoft Office 2016\\Alati | Mogućnosti | Općenito | Mogućnosti servisa...\\PowerPoint Designer.

- *Isključivanje alata za brz početak rada* u odjeljku Konfiguracija korisnika\\Pravilnici\\Administrativni predlošci\\Microsoft PowerPoint 2016\\Mogućnosti programa PowerPoint\\Općenito

- *Dopusti značajku LinkedIn pomoćnika za životopis* u odjeljku Konfiguracija korisnika\\Pravilnici\\Administrativni predlošci\\Microsoft Word 2016\\Mogućnosti programa Word\\Općenito

 I dalje možete koristiti te postojeće postavke pravilnika ako želite isključiti pojedinačna povezana iskustva. Ipak, imajte na umu da ako koristite neku od novih postavki pravilnika, ta nova postavka pravilnika može isključiti povezano iskustvo koje ste uključili korištenjem neke druge postavke pravilnika. Na primjer, ako omogućite postavku pravilnika *Dopusti značajku LinkedIn pomoćnika za životopis*, a onemogućite postavku pravilnika *Dopusti korištenje povezanih iskustava u sustavu Office*, LinkedIn pomoćnik za životopis neće biti dostupan vašim korisnicima.

Općenito govoreći, ako je jedna postavka pravilnika konfigurirana tako da uključuje određeno povezano iskustvo, dok je istodobno druga postavka pravilnika konfigurirana tako da isključuje tu vrstu povezanih iskustava, to će konkretno povezano iskustvo vašim korisnicima biti isključeno.

## <a name="privacy-related-changes-to-the-office-ui"></a>Promjene u korisničkom sučelju sustava Office vezane uz zaštitu privatnosti

Postoje promjene u korisničkom sučelju (UI) sustava Office 365 ProPlus vezane uz zaštitu privatnosti koje će vaši korisnici možda opaziti te postavljati pitanja u vezi s njima. Te su promjene izravan rezultat novih kontrola za zaštitu privatnosti i postavki pravilnika dostupnih počevši od verzije 1904.

### <a name="dialog-about-optional-connected-experiences"></a>Dijaloški okvir za neobavezna povezana iskustva

Ako ste odabrali korisnicima ponuditi [neobavezna povezana iskustva](optional-connected-experiences.md), kada vaši korisnici prvi put otvore aplikaciju sustava Office nakon ažuriranja na verziju 1904 ili noviju, pojavit će se informativni dijaloški okvir. Taj dijaloški okvir obavještava korisnike da ste im omogućili izbor žele li koristiti ta neobavezna povezana iskustva te im daje do znanja da mogu otići u odjeljak **Datoteka** > **Račun** > **Zaštita privatnosti računa** da bi promijenili tu postavku.

### <a name="privacy-settings-removed-from-the-office-ui"></a>Postavke zaštite privatnosti uklonjene iz korisničkog sučelja sustava Office

Ove su postavke uklonjene iz odjeljka **Datoteka** > **Mogućnosti** > **Centar za pouzdanost** > **Postavke centra za pouzdanost...** > **Mogućnosti zaštite privatnosti**:

- Dohvatite dizajn, informacije, preporuke i servise dopuštajući sustavu Office pristup poboljšanjima proizvoda i njihovu primjenu na temelju sadržaja sustava Office na mom uređaju.

- Dopusti povezivanje sustava Office s Microsoftovim internetskim servisima radi omogućivanja funkcija relevantnih za vaše korištenje i preferencije.

Osim toga, u odjeljku **Datoteka** > **Mogućnosti** > **Općenito** uklonjen je odabir za omogućivanje inteligentnih servisa sustava Office.

Kao administrator za svoju tvrtku ili ustanovu sada možete kontrolirati ekvivalentne postavke putem prethodno opisanih novih postavki pravilnika.

### <a name="privacy-settings-added-to-the-office-ui"></a>Postavke zaštite privatnosti dodane u korisničko sučelje sustava Office

Ovo su novi elementi dodani u korisničko sučelje sustava Office:

- U odjeljku **Datoteka** > **Račun** korisnici će vidjeti novu mogućnost u odjeljku **Zaštita privatnosti računa** > **Upravljanje postavkama**. U odjeljku **Upravljanje postavkama** korisnici mogu isključiti neobavezna povezana iskustva ako ste im dali tu mogućnost.

- U odjeljku **Datoteka** > **Mogućnosti** > **Centar za pouzdanost** > **Postavke centra za pouzdanost...** > **Mogućnosti zaštite praivatnosti** nalazi se mogućnost kojom se omogućuje korištenje [Preglednika dijagnostičkih podataka](https://support.office.com/article/cf761ce9-d805-4c60-a339-4e07f3182855) na tom uređaju.

 
## <a name="control-privacy-settings-by-editing-the-registry"></a>Kontrolirajte postavke zaštite privatnosti uređivanjem registra

Pojedini administratori radije mijenjaju postavke izravno u registru, primjerice pomoću skripte, umjesto pomoću Pravilnika grupe ili servisa pravilnika u oblaku za Office. Pomoću sljedećih informacija možete konfigurirati postavke zaštite privatnosti izravno u registru.


|**Postavka pravilnika** |**Postavka registra**  |**Vrijednosti**  |
|---------|---------|---------|---------|
|Konfiguriranje razine dijagnostičkih podataka o klijentskom softveru koje Office šalje Microsoftu  | SendTelemetry |1 = obavezno <br/> 2 = neobavezno <br/> 3 = nijedno|
|Dopusti korištenje povezanih iskustava koja analiziraju sadržaj u sustavu Office  | UserContentDisabled | 1 = omogućeno <br/> 2 = onemogućeno|
|Dopusti korištenje povezanih iskustava koja preuzimaju internetski sadržaj u sustavu Office  | DownloadContentDisabled | 1 = omogućeno <br/> 2 = onemogućeno|
|Dopusti korištenje dodatnih neobaveznih povezanih iskustava u sustavu Office   | ControllerConnectedServicesEnabled  |1 = omogućeno <br/> 2 = onemogućeno|
|Dopusti korištenje povezanih iskustava u sustavu Office | DisconnectedState  | 1 = omogućeno <br/> 2 = onemogućeno|

Da biste stvorili datoteku .reg za postavke zaštite privatnosti, otvorite Blok za pisanje i kopirajte u sljedeće retke. Prilagodite vrijednosti u skladu sa svojim potrebama, a zatim spremite datoteku. Provjerite ima li naziv datoteke proširenje .reg

```
Windows Registry Editor Version 5.00

[HKEY_CURRENT_USER\Software\Policies\Microsoft\office\16.0\common\privacy]
"disconnectedstate"=dword:00000001
"usercontentdisabled"=dword:00000001
"downloadcontentdisabled"=dword:00000001
"controllerconnectedservicesenabled"=dword:00000001

[HKEY_CURRENT_USER\Software\Policies\Microsoft\office\common\clienttelemetry]
"sendtelemetry"=dword:00000002
```

Na primjer, da biste konfigurirali postavke zaštite privatnosti za korisnika, ovu datoteku .reg možete koristiti s naredbom regedit.exe u skripti.