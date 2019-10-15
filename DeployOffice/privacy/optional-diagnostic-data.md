---
title: Neobavezni dijagnostički podaci za Office
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
description: Office administratorima sustava pruža informacije o neobaveznim dijagnostičkim podacima u sustavu Office, uključujući primjere događaja.
hideEdit: true
ms.openlocfilehash: d772a649a78a88112a270e839834cbe48141217f
ms.sourcegitcommit: 02c4120c0b10bfe378d21d60699ae49aaef97834
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/15/2019
ms.locfileid: "37510126"
---
# <a name="optional-diagnostic-data-for-office"></a>Neobavezni dijagnostički podaci za Office

> [!IMPORTANT]
> Informacije u ovom članku odnose se na verziju 1904 ili noviju verziju sljedećeg klijentskog softvera sustava Office instaliranog na računalu sa sustavom Windows:
> - Office 365 ProPlus i Office 365 Business
> - Office 365 Personal, Office 365 Home ili druge verzije sustava Office koje su dio pretplate na Office 365.
> - Project i Visio koji se isporučuju s nekim pretplatničkim tarifama, kao što su Project Online Professional ili Visio Online Plan 2.
>
> Informacije se odnose i na verziju 16.28 ili noviju verziju sljedećih aplikacija sustava Office za Mac: Excel, Outlook, OneNote, PowerPoint i Word.

Dijagnostički podaci koriste se da bi Office uvijek bio siguran i ažuran, kao i radi otkrivanja, dijagnosticiranja i rješavanja problema te poboljšavanja proizvoda. Ti podaci ne sadrže korisnikovo ime ili adresu e-pošte, sadržaj korisnikovih datoteka ni informacije o aplikacijama koje nisu povezane sa sustavom Office.

To su dijagnostički podaci o klijentskom softveru sustava Office koji se koristi na računalima sa sustavom Windows, a koji se prikupljaju i šalju tvrtki Microsoft. Neki su dijagnostički podaci obavezni, a neki nisu. Omogućujemo vam da odaberete hoćete li nam slati obavezne ili dijagnostičke podatke putem kontrola zaštite privatnosti, kao što su postavke pravila za tvrtke ili ustanove. Dijagnostičke podatke koji nam se šalju možete pogledati pomoću preglednika dijagnostičkih podataka.

***Neobavezni dijagnostički podaci***: dodatni podaci koji nam pomažu pri poboljšavanju proizvoda i pružaju poboljšane informacije koje nam pomažu pri otkrivanju, dijagnosticiranju i rješavanju problema.

Ako odaberete slanje neobaveznih dijagnostičkih podataka, uz njih se prikupljaju i obavezni dijagnostički podaci.

Primjeri neobaveznih dijagnostičkih podataka obuhvaćaju podatke koje prikupljamo o slikama koje korisnici umeću u dokumente programa Word da bismo mogli ponuditi bolje mogućnosti za slike te podatke koje prikupljamo o vremenu potrebnom da se slajd programa PowerPoint prikaže na zaslonu da bismo mogli poboljšati okruženje ako je presporo.

Dodatne informacije o dijagnostičkim podacima potražite u ovim člancima:

- [Obavezni dijagnostički podaci za Office](required-diagnostic-data.md)
- [Korištenje preglednika dijagnostičkih podataka sa sustavom Office](https://support.office.com/article/cf761ce9-d805-4c60-a339-4e07f3182855)

Ako ste administrator za tvrtku ili ustanovu, možda će vas zanimati i sljedeći članci:

- [Pregled kontrola za zaštitu privatnosti za Office 365 ProPlus](overview-privacy-controls.md)
- [Korištenje postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Office 365 ProPlus](manage-privacy-controls.md)
- [Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office za Mac](mac-privacy-preferences.md)
- [Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti na iOS uređajima](ios-privacy-preferences.md)

## <a name="categories-of-optional-diagnostic-data"></a>Kategorije neobaveznih dijagnostičkih podataka

Neobavezni dijagnostički podaci organizirani su u sljedeće kategorije:

- Instalacija softvera i instalirani softver
- Korištenje proizvoda i usluga
- Performanse proizvoda i usluga
- Povezivost i konfiguracija uređaja

Te se kategorije prikazuju u pregledniku dijagnostičkih podataka, a iste se kategorije koriste za obavezne dijagnostičke podatke.

Odjeljci u nastavku sadrže opis svake kategorije i primjere događaja za svaku kategoriju.

## <a name="software-setup-and-inventory-events"></a>Događaji koji se odnose na instalaciju softvera i instalirani softver

Ta kategorija obuhvaća događaje koji se mogu odnositi na sljedeća područja:

- Instalirani proizvod, njegovu verziju i njegov status instalacije
- Softverski dodaci i njihove postavke.
- Uvjeti za pogreške u dokumentima, značajkama i dodacima koji mogu ugroziti sigurnost, uključujući spremnost proizvoda za ažuriranje.

U tablici u nastavku navedeni su primjeri događaja u toj kategoriji i opis tih događaja.

| **Naziv događaja**   | **Opis događaja**  |
| ---- | ---- |
| Office.Extensibility.AppCommands.GetRibbonUpdatesForUserId | Taj događaj pokazuje ažurira li Word uspješno vrpcu u korisničkom sučelju programa Word kada korisnik promijeni identitet. Taj događaj koristimo za otkrivanje pogrešne instalacije i drugih problema koji mogu utjecati na korisničko sučelje sustava Office. |
| Office.Extensibility.AppCommands.AppCmdInstall   | Taj događaj nudi informacije o dodatku za Office koji je korisnik instalirao, uključujući ID aplikacije, međuverziju i verziju operacijskog sustava, uspješnost instalacije i trajanje instalacije.  |

## <a name="product-and-service-usage-events"></a>Događaji koji se odnose na korištenje proizvoda i usluga

Ta kategorija obuhvaća događaje koji se mogu odnositi na sljedeća područja:

- Uspješno funkcioniranje aplikacije. Ograničeno na otvaranje i zatvaranje aplikacije i dokumenata, uređivanje datoteka i zajedničko korištenje dokumenata (suradnju).
- Utvrđivanje je li došlo do određenih događaja povezanih sa značajkama, kao što je pokretanje ili zaustavljanje, te utvrđivanje je li značajka pokrenuta.
- Značajke pristupačnosti u sustavu Office

U tablici u nastavku navedeni su primjeri događaja u toj kategoriji i opis tih događaja.

| **Naziv događaja**   | **Opis događaja**  |
| ------ | ------- |
| Office.Word.Commanding.Highlight  | Taj događaj pokazuje da je Word izvršio naredbu za isticanje teksta. Taj događaj koristimo za otkrivanje pogrešaka u naredbi za označavanje teksta.  |
| Office.Translator.AddInLoaded   | Impulsni podaci koji pokazuju da je značajka prevoditelja uspješno učitana i prikazana.  |
| Office.Graphics.GVizInsertShape |Prati uspješnost ili neuspješnost značajke umetanja slike i prijavljuje pojedinosti o vrstama umetnutih slika i njihovu izvoru.| 
| Office.PowerPoint.PPT.Desktop.SummaryZoomInsertionRule   | Taj događaj utvrđuje ima li u dokumentu sekcija kada korisnik umeće skupni pregled te je li korisnik odabrao brisanje postojećih sekcija. |
| Office.Security.SecureReaderHost.ProtectedViewValidation | Prati kada je i zašto datoteka otvorena u zaštićenom prikazu. Koristi se za dijagnosticiranje stanja kada se zaštićeni prikaz nije mogao uspješno aktivirati da bi se provjerilo funkcionira li značajka ispravno. |

## <a name="product-and-service-performance-events"></a>Događaji koji se odnose na performanse proizvoda i usluga

Ta kategorija obuhvaća događaje koji se mogu odnositi na sljedeća područja:

- Neočekivana zatvaranja (rušenja) aplikacija i stanje aplikacije kada se to dogodi.
- Loše vrijeme odziva ili performanse u situacijama kao što su pokretanje aplikacije ili otvaranje datoteke.
- Pogreške u funkcioniranju značajke ili korisničkog okruženja.

U tablici u nastavku navedeni su primjeri događaja u toj kategoriji i opis tih događaja.

| **Naziv događaja**    | **Opis događaja**   |
| --------------- | -------------- |
| Office.Word.Word.CoreSaveTime100ns     | Taj događaj bilježi performanse aktivnosti spremanja dokumenta u programu Word. Taj događaj koristimo za otkrivanje pogrešaka i problema s performansama tijekom aktivnosti spremanja dokumenta u programu Word.|
| Office.Identity.SignInForWamAccountAad  | Taj se događaj šalje kada se korisnik prijavi na račun za Azure Active Directory pomoću biblioteke upravitelja web-računa (Web Account Manager, WAM). Taj događaj šalje metapodatke kao što su AppName, AppVersion i ErrorCode ako događaj ne uspije. |
| Office.PowerPoint.PPT.Desktop.FileOpen.FirstSlideMasterThumbnailRenderTime | Taj događaj prikuplja podatke o vremenu potrebnom za prikaz minijature prve matrice slajda u programu PowerPoint.  |
| Office.Extensibility.Diagnostics   | Taj događaj nudi općenite dijagnostičke podatke za dodatke sustava Office, kao što su izvješća o rušenju radi otklanjanja pogrešaka.|

## <a name="device-connectivity-and-configuration-events"></a>Događaji koji se odnose na povezivost i konfiguracija uređaja

Ta kategorija obuhvaća događaje koji se mogu odnositi na sljedeća područja:

- Stanje mrežne veze i postavke uređaja, kao što je memorija.

U tablici u nastavku navedeni su primjeri događaja u toj kategoriji i opis tih događaja.

| **Naziv događaja**                    | **Opis događaja**                                                                                                                                                     |
| ------ | ----- |
| Office.Graphics.ArtViewValidate | Taj događaj bilježi provjeru valjanosti rezultata prikaza grafike koji podržava grafičko korisničko sučelje. Taj događaj koristimo za prikupljanje podataka o korištenju i pogreškama o prikazu grafike. |
| Office.Graphics.ARCExceptionScope | Taj događaj prati pogreške u prikazu modula za prikaz. |
| Office.Extensibility.ODPLatency   | Taj događaj pruža informacije o korisnikovoj mrežnoj vezi i brzini.     |
