---
title: Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office za Mac
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
description: Administratorima sustava Office nudi informacije o načinu korištenja preferenci za upravljanje kontrolama za zaštitu privatnosti za Office za Mac.
hideEdit: true
ms.openlocfilehash: 01bb31f3b6c307ec1dc4762b54fea17185dcf27d
ms.sourcegitcommit: 0fd23324ba1364fa1f8dd1578adf25946adde90f
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/07/2019
ms.locfileid: "36246258"
---
# <a name="use-preferences-to-manage-privacy-controls-for-office-for-mac"></a>Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office za Mac

Počevši od verzije 16.28 sustava Office za Mac, postoje nove postavke preferenci koje omogućuju kontrolu nad postavkama vezanima uz sljedeće:

- ***Dijagnostičke podatke*** o klijentskom softveru sustava Office, koji se prikupljaju i šalju Microsoftu.

- ***Povezana iskustva*** koja koriste funkcije utemeljene na oblaku da bi vama i vašim korisnicima ponudila poboljšane značajke sustava Office.

Osim toga, tu je i nova postavka preferenci koja se odnosi na dijaloški okvir **potrebne podatkovne obavijesti** za Microsoft AutoUpdate (MAU).

Dodatne informacije o dijagnostičkim podacima i povezanim iskustvima potražite u članku Pregled kontrola zaštite privatnosti](overview-privacy-controls.md).

> [!NOTE]
> Dodatne informacije o sličnim postavkama za Office na računalima sa sustavom Windows potražite u članku [Korištenje postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Office 365 ProPlus](manage-privacy-controls.md).

## <a name="setting-preferences"></a>Postavke preferenci

Te su nove postavke značajke CFPreference API-ja kompatibilne i mogu se postaviti pomoću `defaults` naredbe u terminalu ili se primijeniti putem profila za konfiguraciju ili poslužitelja za upravljanje mobilnim uređajima (MDM). Prilikom provedbe preferenci korisnici ne mogu promijeniti vrijednosti, a sve će se kontrole u aplikaciji prikazati onemogućenima.

## <a name="preference-setting-for-diagnostic-data"></a>Postavka preferenci za dijagnostičke podatke

Dijagnostički podaci koriste se da bi Office uvijek bio siguran i ažuran, kao i radi otkrivanja, dijagnosticiranja i otklanjanja problema te poboljšavanja proizvoda. Za više informacija pogledajte [Dijagnostički podaci koje Office 365 ProPlus šalje Microsoftu](overview-privacy-controls.md#diagnostic-data-sent-from-office-365-proplus-to-microsoft).

|||
|:-----|:-----|
|**Preference Domain**  | `com.microsoft.office` |
|**Tipka**  | `DiagnosticDataTypePreference`  |
|**Vrsta podataka**  | Niz |
|**Moguće vrijednosti**  | `BasicDiagnosticData` *(time se razina postavlja na obveznu)* <br/> `FullDiagnosticData` *(time se razina postavlja na neobaveznu)* <br/> `ZeroDiagnosticData` *(time se ne postavlja razina)* |
|**Dostupnost** |16.28 i noviji |

> [!NOTE]
> Ako postavite tu preferencu, primjenjivat će se i na sljedeće proizvode:
> - Verzija 1.00.217856 i novija programa Teams za Mac
> - Verzija 16.28 i novija programa Skype za tvrtke za Mac

Ako ne postavite tu preferencu, Microsoftu se šalju neobavezni i obavezni dijagnostički podaci ako su korisnici s pretplatom na Office 365 prijavljeni pomoću računa tvrtke ili obrazovne ustanove ili ako korisnici imaju licencirane verzije sustava Office 2019 za Mac. Osim toga, ti korisnici ne mogu promijeniti razinu dijagnostičkih podataka bez obzira na to kako postavite tu preferencu.

Drugim korisnicima, kao privatnim korisnicima s pretplatom na Office 365, šalju se samo obavezni dijagnostički podaci, osim ako korisnik odabere da šalje i neobavezne dijagnostičke podatke odlaskom na **postavke** > **zaštite privatnosti**.

## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a>Postavka preferenci za povezana iskustva koja analiziraju vaš sadržaj

Povezana iskustva koja analiziraju vaš sadržaj iskustva su koja koriste vaš sadržaj iz sustava Office da bi vam ponudila preporuke dizajna, prijedloge za uređivanje, uvide u podatke i slične značajke. Na primjer, PowerPoint Designer ili Istraživač programu Word. Popis tih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).

|||
|:-----|:-----|
|**Preference Domain**  | `com.microsoft.office` |
|**Tipka**  | `OfficeExperiencesAnalyzingContentPreference`  |
|**Vrsta podataka**  | booleovski |
|**Moguće vrijednosti**  | `TRUE` *(omogućeno)* <br/> `FALSE` *(onemogućeno)*|
|**Dostupnost** |16.28 i noviji |

Ako ne postavite tu preferencu, povezana iskustva koja analiziraju sadržaj dostupna su korisnicima. 

Ako korisnik ima pretplatu na Office 365 te se prijavi pomoću računa tvrtke ili obrazovne ustanove ili ako ima licenciranu verziju sustava Office 2019 za Mac, ne može isključiti povezana iskustva koja analiziraju sadržaj.

Za druge korisnike, kao što su korisnici s pretplatom na Office 365, korisnik može odabrati isključiti povezana iskustva koja analiziraju sadržaj odlaskom na **postavke** > **zaštite privatnosti**.

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a>Postavka preferenci za povezana iskustva koja preuzimaju internetski sadržaj

Povezana iskustva koja preuzimaju internetski sadržaj iskustva su koja omogućuju pretraživanje i preuzimanje internetskih sadržaja – uključujući predloške, slike, 3D modele, videozapise i referentne materijale – radi poboljšavanja vaših dokumenata. Na primjer, predlošci sustava Office ili alat za brz početak rada s programom PowerPoint. Popis tih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).

|||
|:-----|:-----|
|**Preference Domain**  | `com.microsoft.office` |
|**Tipka**  | `OfficeExperiencesDownloadingContentPreference`  |
|**Vrsta podataka**  | booleovski |
|**Moguće vrijednosti**  | `TRUE` *(omogućeno)* <br/> `FALSE` *(onemogućeno)*|
|**Dostupnost** |16.28 i noviji |

Ako ne postavite tu preferencu, povezana iskustva koja preuzimaju internetski sadržaj dostupna su korisnicima.

Ako korisnik ima pretplatu na Office 365 te se prijavi pomoću računa tvrtke ili obrazovne ustanove ili ako ima licenciranu verziju sustava Office 2019 za Mac, ne može isključiti povezana iskustva koja preuzimaju internetski sadržaj.

Za druge korisnike, kao što su korisnici s pretplatom na Office 365, korisnik može odabrati isključiti povezana iskustva koja preuzimaju internetski sadržaj odlaskom na **postavke** > **zaštite privatnosti**.

## <a name="preference-setting-for-optional-connected-experiences"></a>Postavka preferenci za neobavezna povezana iskustva

Osim gore spomenutih povezanih iskustava postoje i neka neobavezna povezana iskustva za koja korisnicima možete omogućiti da im pristupaju korištenjem računa tvrtke ili ustanove, koji se ponekad naziva račun tvrtke ili račun obrazovne ustanove. Na primjer, značajke vezane uz LinkedIn u pomoćniku za životopis u programu Word ili Traka vremenske prognoze u programu Outlook, koja koristi servis MSN Vrijeme. Dodatne primjere potražite u članku [Pregled neobaveznih povezanih iskustava za Office](optional-connected-experiences.md).

|||
|:-----|:-----|
|**Preference Domain**  | `com.microsoft.office` |
|**Tipka**  | `OptionalConnectedExperiencesPreference`  |
|**Vrsta podataka**  | booleovski |
|**Moguće vrijednosti**  | `TRUE` *(omogućeno)* <br/> `FALSE` *(onemogućeno)*|
|**Dostupnost** |16.28 i noviji |

Ako ne postavite tu preferencu, neobavezna povezana iskustva dostupna su korisnicima s pretplatom na Office 365 na koji se prijavljuje pomoću računa tvrtke ili obrazovne ustanove ili korisnicima koji imaju licencirane verzije sustava Office 2019 za Mac. Osim ako niste postavili tu preferencu na , ti korisnici mogu odabrati isključiti neobavezno povezano iskustvo odlaskom na **Postavke** > **zaštite privatnosti**.

Za druge korisnike, kao što su privatni korisnici s pretplatom na Office 365, ne postoji opcija isključivanja neobaveznih povezanih iskustava.

## <a name="preference-setting-for-most-connected-experiences"></a>Postavka preferenci za većinu povezanih iskustava

Tu preferencu možete koristiti za kontrolu je li većina povezanih iskustva dostupna vašim korisnicima.

|||
|:-----|:-----|
|**Preference Domain**  | `com.microsoft.office` |
|**Tipka**  | `ConnectedOfficeExperiencesPreference`  |
|**Vrsta podataka**  | booleovski |
|**Moguće vrijednosti**  | `TRUE` *(omogućeno)* <br/> `FALSE` *(onemogućeno)*|
|**Dostupnost** |16.28 i noviji |

Ako ne postavite tu preferencu, sva su povezana iskustva dostupna vašim korisnicima, osim ako ste postavili neku od drugih preferenci za povezana iskustva koja su prethodno navedena, kao na primjer `OfficeExperiencesAnalyzingContentPreference`.

Na primjer, ako ovu preferencu postavite na `FALSE`, sljedeće vrste povezanih iskustava neće biti dostupne vašim korisnicima:
- iskustva koja analiziraju sadržaj
- iskustva koja preuzimaju internetski sadržaj
- neobavezna povezana iskustva

Uz to, ako podesite ovu preferencu na `FALSE`, isključuje se i većina drugih povezanih iskustava, kao što su suautorstvo i internetski prostor za pohranu datoteka. Popis tih drugih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).

No čak i ako podesite ovu preferencu na`FALSE`, ostat će dostupna ograničena funkcionalnost sustava Office, pa će tako sinkronizacija poštanskog sandučića u programu Outlook te Teams i Skype za tvrtke i dalje funkcionirati. [Ključni servisi](essential-services.md), poput servisa za licenciranje, koji potvrđuje da imate ispravnu licencu za korištenje sustava Office, također će ostati dostupni.

Ako korisnik ima pretplatu na Office 365 te se prijavi pomoću računa tvrtke ili obrazovne ustanove ili ako ima licenciranu verziju sustava Office 2019 za Mac, ne može isključiti većinu povezanih iskustava.

Za druge korisnike, kao što su privatni korisnici s pretplatom na Office 365, korisnik može odabrati isključiti većinu povezanih iskustva odlaskom na **postavke** > **zaštite privatnosti**.

## <a name="preference-setting-for-the-required-data-notice-dialog-for-microsoft-autoupdate"></a>Postavka preferenci u dijaloškom okviru potrebne podatkovne obavijesti za Microsoft AutoUpdate

Prvi put kada se pokrene verzija 4.12 ili novija programa Microsoft AutoUpdate (MAU), korisnici će vidjeti dijaloški okvir **potrebne podatkovne obavijesti** koji im omogućuje informacije o podacima iz MAU-a koji se šalju Microsoftu.

Ako ne želite da korisnici vide tu dijaloški okvir **potrebne podatkovne obavijesti** za Microsoft AutoUpdate, možete postaviti sljedeću preferencu. Bez obzira na to koju vrijednost postavite, dijaloški okvir neće se prikazati vašim korisnicima.

|||
|:-----|:-----|
|**Preference Domain**  | `com.microsoft.autoupdate2` |
|**Tipka**  | `AcknowledgedDataCollectionPolicy`  |
|**Vrsta podataka**  | Niz |
|**Moguće vrijednosti**  | `RequiredDataOnly` <br/> `RequiredAndOptionalData`|
|**Dostupnost** |4.12 i novija |

Ako vaši korisnici vide ovaj dijaloški okvir, kada korisnik odabere**U redu**, vrijednost`RequiredDataOnly` se zapisuje u `AcknowledgedDataCollectionPolicy` i dijaloški se okvir ne prikazuje ponovno korisniku.


## <a name="related-topics"></a>Povezane teme

- [Referenca za konfiguraciju profila (dokumentacija za Appleove inženjere)](https://go.microsoft.com/fwlink/p/?linkid=852998)
- [Implementacija preferenci za Office za Mac](../mac/deploy-preferences-for-office-for-mac.md)
- [Postavke zaštite privatnosti računa](https://support.office.com/article/3e7bc183-bf52-4fd0-8e6b-78978f7f121b#ID0EAADAAA=Mac)
