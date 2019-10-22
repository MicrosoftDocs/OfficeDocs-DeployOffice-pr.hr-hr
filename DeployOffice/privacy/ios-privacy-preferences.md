---
title: Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office na iOS uređajima
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
description: Administratorima sustava Office nudi informacije o upravljanju postavkama zaštite privatnosti na uređajima sa sustavom iOS.
hideEdit: true
ms.openlocfilehash: d1a14d2e1bfe45710255467fcbce9ac4af2c9cb7
ms.sourcegitcommit: 903d6bac7d8b7d8003863ac778c0b5bbdfa7a62a
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/21/2019
ms.locfileid: "37604275"
---
# <a name="use-preferences-to-manage-privacy-controls-for-office-on-ios-devices"></a>Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office na iOS uređajima

Postoje nove postavke preferenci kojima se omogućuje kontrola nad postavkama povezanima sa sljedećim:

- ***Dijagnostički podaci*** koji se prikupljaju i šalju Microsoftu o klijentskom softveru sustava Office koji se upotrebljava.

- ***Povezana iskustva*** koja se koriste funkcijom utemeljenoj na oblaku da bi vama i vašim korisnicima ponudila poboljšane značajke sustava Office.

Dodatne informacije o dijagnostičkim podacima i povezanim iskustvima potražite u članku [Pregled kontrola zaštite privatnosti](overview-privacy-controls.md).

Te preference postavki odnose se na sljedeće aplikacije:
- Verzija 2.30 i novije aplikacije Word za iOS, Excel za iOS i PowerPoint za iOS.
- Verzija 16.30 i novije aplikacije OneNote za iOS.
- Verzija 1.17 i novije programa Visio Viewer za iOS.

> [!NOTE]
> Informacije o sličnim postavkama za Office na računalima sa sustavom macOS potražite u odjeljku [Upotreba postavki za upravljanje kontrolama za zaštitu privatnosti za Office za Mac](mac-privacy-preferences.md)


## <a name="setting-device-preferences"></a>Postavljanje preferenci uređaja
Ove nove preference postavki također se mogu postaviti na razini uređaja putem poslužitelja za upravljanje mobilnim uređajima (MDM) kada je instaliran program Office. Mnogi MDM poslužitelji omogućuju IT administratorima da dodaju neobavezni konfiguracijski rječnik kada poslužitelj pošalje `InstallApplication` MDM naredbu na iOS uređaj. Pojedinosti potražite u dokumentaciji vašeg MDM poslužitelja.

Rječnik je predstavljen kao skup parova ključeva/vrijednosti u XML obliku. Na primjer:

```xml
<dict>
    <key>DiagnosticDataTypePreference</key>
    <string>BasicDiagnosticData</string>
</dict>
```

Nakon slanja na uređaj, konfiguracijski rječnik nalazit će se pod `com.apple.managed.configuration` ključem, gdje će se čitati kada se pokrene aplikacija Office.

## <a name="preference-setting-for-diagnostic-data"></a>Postavka preferenci za dijagnostičke podatke

Dijagnostički se podaci upotrebljavaju da bi Office uvijek bio siguran i ažuran, kao i radi otkrivanja, dijagnosticiranja i otklanjanja problema te poboljšavanja proizvoda. Za više informacija pogledajte [Dijagnostički podaci koje Office 365 ProPlus šalje Microsoftu](overview-privacy-controls.md#diagnostic-data-sent-from-office-365-proplus-to-microsoft).

|||
|:-----|:-----|
|**Ključ**  | `DiagnosticDataTypePreference`  |
|**Vrsta podataka**  | Niz |
|**Moguće vrijednosti**  | `BasicDiagnosticData` *(time se razina postavlja na Obvezno)* <br/> `FullDiagnosticData` *(time se razina postavlja na Neobvezno)* <br/> `ZeroDiagnosticData` *(time se razina postavlja na Nijedno)* |

Ako ne postavite tu preferencu, Microsoftu se šalju samo obvezni dijagnostički podaci ako su korisnici s pretplatom na Office 365 prijavljeni pomoću računa poduzeća ili obrazovne ustanove. Osim toga, ti korisnici ne mogu promijeniti razinu dijagnostičkih podataka bez obzira na to kako postavite tu preferencu.

Drugim korisnicima, kao što su privatni korisnici s pretplatom na Office 365, šalju se samo obavezni dijagnostički podaci, osim ako korisnik odabere da šalje i neobavezne dijagnostičke podatke odlaskom na **Postavke** > **Postavke privatnosti**.


## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a>Postavka preferenci za povezana iskustva kojima se analizira vaš sadržaj

Povezana iskustva koja analiziraju vaš sadržaj iskustva su koja koriste vaš sadržaj iz sustava Office da bi vam ponudila preporuke dizajna, prijedloge za uređivanje, uvide u podatke i slične značajke. Na primjer, Ideje za dizajn u programu PowerPoint. Popis tih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).

|||
|:-----|:-----|
|**Ključ**  | `OfficeExperiencesAnalyzingContentPreference`  |
|**Vrsta podataka**  | Booleov |
|**Moguće vrijednosti**  | `TRUE` *(omogućeno)* <br/> `FALSE` *(onemogućeno)*|


Ako ne postavite tu preferencu, povezana iskustva kojima se analizira sadržaj dostupna su korisnicima.

Ako korisnik ima pretplatu na Office 365 te se prijavi s pomoću računa poduzeća ili obrazovne ustanove, ne može isključiti povezana iskustva kojima se analizira sadržaj.

Za druge korisnike, kao što su korisnici s pretplatom na Office 365, korisnik može odabrati da isključi povezana iskustva kojima se analizira sadržaj odlaskom na **Postavke** > **Postavke privatnosti**.

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a>Postavka preferenci za povezana iskustva kojima se preuzima internetski sadržaj

Povezana iskustva koja preuzimaju internetski sadržaj iskustva su koja omogućuju pretraživanje i preuzimanje internetskih sadržaja – uključujući predloške, slike, videozapise i referentne materijale – radi poboljšavanja vaših dokumenata. Na primjer, predlošci sustava Office ili umetanje mrežne ikone. Popis tih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).

|||
|:-----|:-----|
|**Ključ**  | `OfficeExperiencesDownloadingContentPreference`  |
|**Vrsta podataka**  | Booleov |
|**Moguće vrijednosti**  | `TRUE` *(omogućeno)* <br/> `FALSE` *(onemogućeno)*|


Ako ne postavite tu preferencu, povezana iskustva kojima se preuzima internetski sadržaj dostupna su korisnicima.

Ako korisnik ima pretplatu na Office 365 te se prijavi s pomoću računa poduzeća ili obrazovne ustanove, ne može isključiti povezana iskustva kojima se preuzima internetski sadržaj.

Za druge korisnike, kao što su korisnici s pretplatom na Office 365, korisnik može odabrati da isključi povezana iskustva kojima se preuzima internetski sadržaj odlaskom na **Postavke** > **Postavke privatnosti**.

## <a name="preference-setting-for-optional-connected-experiences"></a>Postavka preferenci za neobavezna povezana iskustva

Osim prethodno spomenutih povezanih iskustava postoje i neka neobavezna povezana iskustva za koja korisnicima možete omogućiti da im pristupaju upotrebom računa poduzeća ili ustanove, koji se ponekad naziva račun poduzeća ili račun obrazovne ustanove. Na primjer, dodaci sustava Office koji se preuzimaju putem trgovine sustava Office na vaš uređaj. Dodatne primjere potražite u članku [Pregled neobaveznih povezanih iskustava za Office](optional-connected-experiences.md).

|||
|:-----|:-----|
|**Ključ**  | `OptionalConnectedExperiencesPreference`  |
|**Vrsta podataka**  | Booleov |
|**Moguće vrijednosti**  | `TRUE` *(omogućeno)* <br/> `FALSE` *(onemogućeno)*|


Ako ne postavite tu preferencu, neobavezna povezana iskustva dostupna su korisnicima s pretplatom na Office 365 na koji se prijavljuje s pomoću računa poduzeća ili obrazovne ustanove. Osim ako niste postavili tu preferencu na FALSE, ti korisnici mogu odabrati da isključe neobavezno povezano iskustvo odlaskom na **Postavke** > **Postavke privatnosti**.

Za druge korisnike, kao što su privatni korisnici s pretplatom na Office 365, ne postoji opcija isključivanja neobaveznih povezanih iskustava.