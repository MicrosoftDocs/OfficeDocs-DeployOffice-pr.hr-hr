---
title: Upotreba postavki za upravljanje kontrolama za zaštitu privatnosti za Office za Mac
ms.author: danbrown
author: pbowden-msft
manager: laurawi
audience: ITPro
ms.topic: article
ms.service: o365-proplus-itpro
localization_priority: Priority
ms.collection: Ent_O365
ms.custom:
- Ent_Office_ProPlus
- Ent_Office_Privacy
- Ent_Office_Mac
description: Administratorima sustava Office nudi informacije o načinu upotrebe preferenci za upravljanje kontrolama za zaštitu privatnosti za Office za Mac.
hideEdit: true
ms.openlocfilehash: d23d1288adf823888c900b44acd5bc905037cd94
ms.sourcegitcommit: 3890a23390edd0b5fdb2cf33613ec0778566cf97
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/01/2020
ms.locfileid: "43992865"
---
# <a name="use-preferences-to-manage-privacy-controls-for-office-for-mac"></a>Upotreba postavki za upravljanje kontrolama za zaštitu privatnosti za Office za Mac

Počevši od verzije 16.28 sustava Office za Mac, postoje nove postavke preferenci kojima se omogućuje kontrola nad postavkama povezanima sa sljedećim:

- ***Dijagnostički podaci*** koji se prikupljaju i šalju Microsoftu o klijentskom softveru sustava Office koji se upotrebljava.

- ***Povezana iskustva*** koja se koriste funkcijom utemeljenoj na oblaku da bi vama i vašim korisnicima ponudila poboljšane značajke sustava Office.

Osim toga, tu je i nova postavka preferenci koja se odnosi na dijalog **Potrebne podatkovne obavijesti** za Microsoft AutoUpdate (MAU).

Dodatne informacije o dijagnostičkim podacima i povezanim iskustvima potražite u članku [Pregled kontrola zaštite privatnosti](overview-privacy-controls.md).

> [!NOTE]
> - Informacije o sličnim postavkama za Office na računalima sa sustavom Windows potražite u članku [Upotreba postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Microsoft 365 Apps za velike tvrtke](manage-privacy-controls.md).
> - Informacije o sličnim postavkama za Office na iOS uređajima potražite u [Upotreba postavki za upravljanje kontrolama za zaštitu privatnosti za Office na iOS uređajima](ios-privacy-preferences.md).

## <a name="setting-preferences"></a>Postavke preferenci

Te su nove postavke značajke CFPreference API-ja kompatibilne i mogu se postaviti s pomoću `defaults` naredbe u terminalu ili se primijeniti s pomoću profila za konfiguraciju ili poslužitelja za upravljanje mobilnim uređajima (MDM). Prilikom provedbe preferenci korisnici ne mogu promijeniti vrijednosti, a sve će se kontrole u aplikaciji prikazati onemogućenima.

> [!NOTE]
> Možete koristiti i servis za pravilnike u oblaku sustava Office i sljedećih pet postavki pravilnika:
> - Konfiguriranje razine dijagnostičkih podataka o klijentskom softveru koje Office šalje Microsoftu
> - dopusti korištenje povezanih iskustava koja analiziraju sadržaj u sustavu Office 
> - dopusti korištenje povezanih iskustava koja preuzimaju internetski sadržaj u sustavu Office 
> - dopusti korištenje dodatnih neobaveznih povezanih iskustava u sustavu Office
> - Dopusti korištenje povezanih iskustava u sustavu Office
>
> Dodatne informacije o upotrebi servisa za pravilnike u oblaku sustava Office potražite u članku [Pregled servisa pravilnika u oblaku sustava Office](../overview-office-cloud-policy-service.md).


## <a name="preference-setting-for-diagnostic-data"></a>Postavka preferenci za dijagnostičke podatke

Dijagnostički podaci koriste se da bi Office uvijek bio siguran i ažuran, kao i radi otkrivanja, dijagnosticiranja i otklanjanja problema te poboljšavanja proizvoda. Dodatne informacije potražite u članku [Dijagnostički podaci koje Microsoft 365 Apps za velike tvrtke šalje Microsoftu](overview-privacy-controls.md#diagnostic-data-sent-from-microsoft-365-apps-for-enterprise-to-microsoft).

|||
|:-----|:-----|
|**Preference Domain**  | `com.microsoft.office` |
|**Tipka**  | `DiagnosticDataTypePreference`  |
|**Vrsta podataka**  | Niz |
|**Moguće vrijednosti**  | `BasicDiagnosticData` *(time se razina postavlja na Obvezno)* <br/> `FullDiagnosticData` *(time se razina postavlja na Neobvezno)* <br/> `ZeroDiagnosticData` *(time se razina postavlja na Nijedno)* |
|**Dostupnost** |16.28 i novija |

Počevši s novim instalacijama verzije 16.30, ako ne postavite tu preferencu, Microsoftu se šalju samo obavezni dijagnostički podaci ako su korisnici s pretplatom na Office 365 (ili Microsoft 365) prijavljeni pomoću računa tvrtke ili obrazovne ustanove ili ako korisnici imaju licencirane verzije sustava Office 2019 za Mac. Osim toga, ti korisnici ne mogu promijeniti razinu dijagnostičkih podataka bez obzira na to kako postavite tu preferencu.

> [!NOTE]
> - Ako instalirate verziju 16,28 ili 16,29 te ne postavljate tu preferencu, Microsoftu se šalju neobavezni i obavezni dijagnostički podaci. Ako ste zatim nadogradili na verziju 16.30 ili noviju, Microsoftu će se i dalje slati neobavezni i obavezni dijagnostički podaci, osim ako ne koristite tu preferencu da biste postavili neku drugu vrijednost.
> - Ako postavite tu preferencu, primjenjivat će se i na verzije 1.00.217856 i novije Teams za Mac,i na verziju 16.28 i novije verzije Skype za tvrtke za Mac.

Za druge korisnike, kao što su privatni korisnici s pretplatom na Office 365 (ili Microsoft 365), šalju se samo obavezni dijagnostički podaci, osim ako korisnik odabere i slanje neobaveznih dijagnostičkih podataka odlaskom na **Preference** > **Privatnost**.

## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a>Postavka preferenci za povezana iskustva kojima se analizira vaš sadržaj

Povezana iskustva koja analiziraju vaš sadržaj iskustva su koja koriste vaš sadržaj iz sustava Office da bi vam ponudila preporuke dizajna, prijedloge za uređivanje, uvide u podatke i slične značajke. Na primjer, PowerPoint Designer ili Istraživač u programu Word. Popis tih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).

|||
|:-----|:-----|
|**Preference Domain**  | `com.microsoft.office` |
|**Tipka**  | `OfficeExperiencesAnalyzingContentPreference`  |
|**Vrsta podataka**  | Booleov |
|**Moguće vrijednosti**  | `TRUE` *(omogućeno)* <br/> `FALSE` *(onemogućeno)*|
|**Dostupnost** |16.28 i novija |

Ako ne postavite tu preferencu, povezana iskustva kojima se analizira sadržaj dostupna su korisnicima. 

Ako korisnik ima pretplatu na Office 365 (ili Microsoft 365) te se prijavi pomoću računa poduzeća ili obrazovne ustanove ili ako ima licenciranu verziju sustava Office 2019 za Mac, ne može isključiti povezana iskustva koja analiziraju sadržaj.

Za druge korisnike, kao što su korisnici s pretplatom na Office 365 (ili Microsoft 365), korisnik može odabrati isključivanje povezanih iskustava kojima se analizira sadržaj odlaskom na **Preference** > **Privatnost**.

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a>Postavka preferenci za povezana iskustva kojima se preuzima internetski sadržaj

Povezana iskustva koja preuzimaju internetski sadržaj iskustva su koja omogućuju pretraživanje i preuzimanje internetskih sadržaja – uključujući predloške, slike, 3D modele, videozapise i referentne materijale – radi poboljšavanja vaših dokumenata. Na primjer, predlošci sustava Office ili alat za brz početak rada s programom PowerPoint. Popis tih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).

|||
|:-----|:-----|
|**Preference Domain**  | `com.microsoft.office` |
|**Tipka**  | `OfficeExperiencesDownloadingContentPreference`  |
|**Vrsta podataka**  | Booleov |
|**Moguće vrijednosti**  | `TRUE` *(omogućeno)* <br/> `FALSE` *(onemogućeno)*|
|**Dostupnost** |16.28 i novija |

Ako ne postavite tu preferencu, povezana iskustva kojima se preuzima internetski sadržaj dostupna su korisnicima.

Ako korisnik ima pretplatu na Office 365 (ili Microsoft 365) te se prijavi pomoću računa tvrtke ili obrazovne ustanove ili ako ima licenciranu verziju sustava Office 2019 za Mac, ne može isključiti povezana iskustva koja preuzimaju internetski sadržaj.

Za druge korisnike, kao što su privatni korisnici s pretplatom na Office 365 (ili Microsoft 365), korisnik može odabrati isključivanje povezanih iskustava koja preuzimaju internetski sadržaj odlaskom na **Preference** > **Privatnost**.

## <a name="preference-setting-for-optional-connected-experiences"></a>Postavka preferenci za neobavezna povezana iskustva

Osim prethodno spomenutih povezanih iskustava postoje i neka neobvezna povezana iskustva za koja korisnicima možete omogućiti da im pristupaju upotrebom računa poduzeća ili ustanove, koji se ponekad naziva račun poduzeća ili račun obrazovne ustanove. Na primjer, značajke povezane uz LinkedIn u pomoćniku za životopis u programu Word ili Traka vremenske prognoze u programu Outlook, koja se koristi servisom MSN Vrijeme. Dodatne primjere potražite u članku [Pregled neobveznih povezanih iskustava za Office](optional-connected-experiences.md).

|||
|:-----|:-----|
|**Preference Domain**  | `com.microsoft.office` |
|**Tipka**  | `OptionalConnectedExperiencesPreference`  |
|**Vrsta podataka**  | Booleov |
|**Moguće vrijednosti**  | `TRUE` *(omogućeno)* <br/> `FALSE` *(onemogućeno)*|
|**Dostupnost** |16.28 i novija |

Ako ne postavite tu preferencu, neobavezna povezana iskustva dostupna su korisnicima s pretplatom na Office 365 (ili Microsoft 365) prijavljenima pomoću računa tvrtke ili obrazovne ustanove ili korisnicima koji imaju licencirane verzije sustava Office 2019 za Mac. Ako niste postavili tu preferencu na `FALSE`, ti korisnici mogu odabrati isključivanje neobaveznih povezanih iskustava odlaskom na **Preference** > **Privatnost**.

Za druge korisnike, kao što su privatni korisnici s pretplatom na Office 365 (ili Microsoft 365), ne postoji opcija isključivanja neobaveznih povezanih iskustava.

## <a name="preference-setting-for-most-connected-experiences"></a>Postavka preferenci za većinu povezanih iskustava

Tu preferencu možete upotrijebiti kako biste kontrolirali je li većina povezanih iskustava dostupna vašim korisnicima.

|||
|:-----|:-----|
|**Preference Domain**  | `com.microsoft.office` |
|**Tipka**  | `ConnectedOfficeExperiencesPreference`  |
|**Vrsta podataka**  | Booleov |
|**Moguće vrijednosti**  | `TRUE` *(omogućeno)* <br/> `FALSE` *(onemogućeno)*|
|**Dostupnost** |16.28 i novija |

Ako ne postavite tu preferencu, sva su povezana iskustva dostupna vašim korisnicima, osim ako ste postavili neku od drugih preferenci za povezana iskustva koja su prethodno navedena, kao na primjer `OfficeExperiencesAnalyzingContentPreference`.

Na primjer, ako ovu preferencu postavite na `FALSE`, sljedeće vrste povezanih iskustava neće biti dostupne vašim korisnicima:
- iskustva koja analiziraju sadržaj
- iskustva koja preuzimaju internetski sadržaj
- neobavezna povezana iskustva

Usto, ako podesite ovu preferencu na `FALSE`, isključuje se i većina drugih povezanih iskustava, kao što su suautorstvo i internetski prostor za pohranu datoteka. Popis tih drugih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).

No čak i ako podesite ovu preferencu na`FALSE`, ostat će dostupna ograničena funkcionalnost sustava Office, kao što je sinkronizacija poštanskog sandučića u programu Outlook, pa će Teams i Skype za tvrtke i dalje funkcionirati. [Ključni servisi](essential-services.md), poput servisa za licenciranje, koji potvrđuje da imate ispravnu licencu za korištenje sustava Office, također će ostati dostupni.

Ako korisnik ima pretplatu na Office 365 (ili Microsoft 365) te se prijavi pomoću računa tvrtke ili obrazovne ustanove ili ako ima licenciranu verziju sustava Office 2019 za Mac, ne može isključiti većinu povezanih iskustava.

Za druge korisnike, kao što su privatni korisnici s pretplatom na Office 365 (ili Microsoft 365), korisnik može odabrati isključivanje većine povezanih iskustava odlaskom na **Preference** > **Privatnost**.

## <a name="preference-setting-for-the-required-data-notice-dialog-for-microsoft-autoupdate"></a>Postavka preferenci u dijalogu potrebne podatkovne obavijesti za Microsoft AutoUpdate

Prvi put kada se pokrene verzija 4.12 ili novija programa Microsoft AutoUpdate (MAU), korisnici će vidjeti dijalog **Potrebne podatkovne obavijesti** kojim im se omogućuju informacije o podacima iz MAU-a koji se šalju Microsoftu.

Ako ne želite da korisnici vide dijalog **Potrebne podatkovne obavijesti** za Microsoft AutoUpdate, možete postaviti sljedeću preferencu. Bez obzira na to koju vrijednost postavite, dijalog se neće prikazati vašim korisnicima.

|||
|:-----|:-----|
|**Preference Domain**  | `com.microsoft.autoupdate2` |
|**Tipka**  | `AcknowledgedDataCollectionPolicy`  |
|**Vrsta podataka**  | Niz |
|**Moguće vrijednosti**  | `RequiredDataOnly` <br/> `RequiredAndOptionalData`|
|**Dostupnost** |4.12 i novija |

Ako vašim korisnicima dopustite da vide ovaj dijalog, kada korisnik odabere**U redu**, vrijednost`RequiredDataOnly` zapisuje se u `AcknowledgedDataCollectionPolicy` i dijalog se više ne prikazuje korisniku.


## <a name="related-topics"></a>Povezane teme

- [Referenca za konfiguraciju profila (dokumentacija za Appleove inženjere) ](https://go.microsoft.com/fwlink/p/?linkid=852998)
- [Implementacija preferenci za Office za Mac](../mac/deploy-preferences-for-office-for-mac.md)
- [Postavke zaštite privatnosti računa](https://support.office.com/article/3e7bc183-bf52-4fd0-8e6b-78978f7f121b#ID0EAADAAA=Mac)
