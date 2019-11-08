---
title: Obavezni servisni podaci za Office
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
description: Administratorima sustava Office pruža pregled obaveznih servisnih podataka koji se prikupljaju o povezanim iskustvima u sustavu Office.
hideEdit: true
ms.openlocfilehash: b4cc25ae1c2a34082bff623ad630db664050effb
ms.sourcegitcommit: acb22296532bbfdfcad4dc1e7162f812997fbdd1
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/08/2019
ms.locfileid: "38067148"
---
# <a name="required-service-data-for-office"></a>Obavezni servisni podaci za Office 

> [!IMPORTANT]
> Informacije u ovom članku odnose se na verziju 1904 ili noviju verziju sljedećeg klijentskog softvera sustava Office instaliranog na računalu sa sustavom Windows:
> - Office 365 ProPlus i Office 365 Business
> - Office 365 Personal, Office 365 Home ili druge verzije sustava Office koje su dio pretplate na Office 365.
> - Project i Visio koji se isporučuju s nekim pretplatničkim tarifama, kao što su Project Online Professional ili Visio Online Plan 2.
>
> Informacije se odnose i na verziju 16.28 ili noviju verziju sljedećih aplikacija sustava Office za Mac: Excel, Outlook, OneNote, PowerPoint i Word.

Office se sastoji od klijentskih softverskih aplikacija i povezanih okruženja osmišljenih radi učinkovitijeg stvaranja, komunikacije i suradnje. Suradnja s drugim korisnicima na dokumentu pohranjenom na servisu OneDrive za tvrtke ili prevođenje sadržaja dokumenta programa Word na neki drugi jezik primjeri su povezanih iskustava.

Obavezni servisni podaci ključni su jer nam omogućuju primjenu povezanih iskustava utemeljenih na oblaku te pospješuju sigurnost i funkcioniranje tih iskustava na očekivan način za naše korisnike. Obavezne servisne podatke čine tri vrste informacija.

- **Korisnički sadržaj**, tj. sadržaj koji stvarate koristeći Office, kao što je tekst upisan u dokument programa Word, koji se koristi zajedno s povezanim iskustvom.
- **Funkcionalni podaci**, koji obuhvaćaju informacije koje su povezanom iskustvu potrebne za izvođenje njegovih zadataka, poput konfiguracijskih informacija o aplikaciji.
- **Servisni dijagnostički podaci**, tj. podaci nužni za zaštitu, ažurnost i funkcioniranje servisa na očekivan način. Budući da su ti podaci strogo vezani uz povezano iskustvo, odvojeni su od razina obaveznih ili neobaveznih dijagnostičkih podataka.

## <a name="example-of-required-service-data-for-a-connected-experience"></a>Primjer obaveznih servisnih podataka za povezano iskustvo

Da biste bolje razumjeli obavezne servisne podatke, u nastavku je naveden primjer scenarija upotrebe značajke PowerPoint Designer, povezanog iskustva koje možete koristiti prilikom stvaranja slajdova prezentacije. PowerPoint Designer potpomaže poboljšavanje slajdova automatskim generiranjem dizajnerskih ideja između kojih možete birati. Dok stavljate sadržaj na slajd, Designer u pozadini radi na podudaranju tog sadržaja s profesionalno dizajniranim izgledima.

Obavezni servisni podaci koji se šalju Microsoftu da bi vam se omogućilo to povezano iskustvo mogu obuhvaćati sljedeće:

- *Korisnički sadržaj*, poput teksta ili slika koje ste dodali na slajd.
- *Funkcionalne podatke*, poput slajda na kojem radite i njegovog izgleda.
- *Servisne dijagnostičke podatke*, poput događaja koji nam govore je li se dizajnerska ideja pravilno primijenila na vaš slajd i jesu li servisni pozivi pravilno funkcionirali.

## <a name="view-and-manage-required-service-data"></a>Prikaz obaveznih servisnih podataka i upravljanje njima

Servisne dijagnostičke podatke možete pogledati pomoću preglednika dijagnostičkih podataka. Dodatne informacije potražite u članku [Primjeri događaja za servisne dijagnostičke podatke](#examples-of-events-for-service-diagnostic-data).

Omogućujemo vam da odaberete koje vrste povezanih iskustava želite koristiti u sustavu Office, što pak određuje koji se obavezni servisni podaci šalju nama. PowerPoint Designer, primjerice, jedno je od nekoliko povezanih iskustava koje analizira vaš sadržaj. Ako odlučite isključiti povezano iskustvo koje analizira sadržaj, ne šalju nam se obavezni servisni podaci o programu PowerPoint Designer jer PowerPoint Designer neće biti dostupan za korištenje.

Obavezni servisni podaci prikupljaju se i šalju Microsoftu i za ključne servise sustava Office, kao što je servis za licenciranje, koji provjerava jeste li pravilno licencirani za korištenje sustava Office. Ti podaci za ključne servise šalju se neovisno o postavkama povezanima s privatnošću koje ste konfigurirali.

Dodatne informacije potražite u sljedećim člancima:

- [Povezana iskustva u sustavu Office](connected-experiences.md)
- [Ključni servisi za Office](essential-services.md)
- [Korištenje preglednika dijagnostičkih podataka sa sustavom Office](https://support.office.com/article/cf761ce9-d805-4c60-a339-4e07f3182855)

Ako ste administrator za tvrtku ili ustanovu, možda će vas zanimati i sljedeći članci:

- [Pregled kontrola za zaštitu privatnosti za Office 365 ProPlus](overview-privacy-controls.md)
- [Korištenje postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Office 365 ProPlus](manage-privacy-controls.md)
- [Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office za Mac](mac-privacy-preferences.md)
- [Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office na iOS uređajima](ios-privacy-preferences.md)
- [Korištenje postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Office na Android uređajima](android-privacy-controls.md)

## <a name="examples-of-events-for-service-diagnostic-data"></a>Primjeri događaja za servisne dijagnostičke podatke

Servisni dijagnostički podaci prikazuju se u pregledniku dijagnostičkih podataka i organizirani su u iste kategorije koje koriste obavezni i neobavezni dijagnostički podaci. Na primjer, *Korištenje proizvoda i usluga* ili *Performanse proizvoda i usluga.*

Događaji sa servisne dijagnostičke podatke daju nam nužne informacije o tome jesu li performanse povezanog iskustva onakve kakve korisnik očekuje. Na primjer, je li servis koji povezano iskustvo koristi uspješno pokrenut i je li bio dostupan kada je bio potreban, je li bilo pogrešaka ili drugih neočekivanih problema (rušenja) prilikom interakcije sa servisom te kakve su brzina odziva i performanse sustava.

U tablici u nastavku navedeno je nekoliko primjera događaja za servisne dijagnostičke podatke.

| **Naziv**      | **Opis**    |
| ---------- | --------------------- |
| Office.Excel.Coauth.SaveXrr     | Događaj koji se aktivira u programu Excel prilikom korištenja servisa za suradnju koji prijavljuje pojedinosti o pojedinačnim revizijama koje se zapisuju u zapisnik revizija. Omogućuje nadzor latencije i upućuje na pogreške u programu Excel povezane sa suradnjom  |
| Office.Excel.Coauth.CloseWorkbook  | Događaj koji se aktivira u programu Excel prilikom korištenja servisa za suradnju koji prijavljuje kada se zatvori radna knjiga. Potreban je za utvrđivanje pogrešaka povezanih s ponovnim učitavanjem i automatskim osvježavanjem. Omogućuje mjerenje uspješnosti za aktivnosti servisa za suradnju.   |
| Office.Security.OCX.NonTrustedEncounter    | Događaj koji se aktivira u aplikacijama sustava Office (uključujući Word, Excel, Outlook, PowerPoint i Visio) kada korisnik otvori nepouzdani dokument s ActiveX kontrolom. Koristi se za općenitu procjenu korištenja ActiveX kontrola ugrađenih u dokumente sustava Office radi ublažavanja posljedica sigurnosnih incidenata.  |
| Office.Security.UrlReputation.GetUrlReputation | Događaj koji se aktivira u aplikacijama sustava Office (uključujući Word, Excel, PowerPoint, Visio i Publisher) i koji prati uspješnost ili neuspješnost poziva sigurnosnih veza. Koristi se za provjeru funkcionira li servis sigurnih veza ispravno i za dijagnosticiranje problema.  |
| Office.Voice.VoiceManager.StreamingAudio   | Događaj koji se aktivira u aplikacijama sustava Office (uključujući Word, Outlook i PowerPoint) i koji pruža informacije o stanju prijenosa audiodatoteka strujanjem na servis za govor. Sadrži informacije o veličini audiodatoteke koja se prenosi i pogreškama do kojih je došlo. Taj se podatak koristi za nadzor stanja servisa i za dijagnosticiranje problema koje s prijavili korisnici. |
