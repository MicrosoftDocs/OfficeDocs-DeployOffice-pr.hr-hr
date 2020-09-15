---
title: Korištenje postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za aplikacije Office za web
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
audience: ITPro
ms.topic: article
ms.service: o365-proplus-itpro
localization_priority: Priority
ms.collection: Ent_O365
ms.custom:
- Ent_Office_ProPlus
- Ent_Office_Privacy
description: Administratorima sustava Office nudi informacije o upravljanju postavkama zaštite privatnosti za aplikacije Office za web.
hideEdit: true
ms.openlocfilehash: b5131d5ffc09b28a3b5731a417fcd6d383fb7d01
ms.sourcegitcommit: da41d41b443c8392c96e64a4d2fc674957abddf5
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/11/2020
ms.locfileid: "47431893"
---
# <a name="use-policy-settings-to-manage-privacy-controls-for-office-for-the-web-applications"></a>Korištenje postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za aplikacije Office za web

> [!NOTE]
> Popis proizvoda sustava Office obuhvaćenih ovim informacijama o zaštiti privatnosti potražite u članku [Kontrole za zaštitu privatnosti dostupne za proizvode Office](products-versions-privacy-controls.md).

Kao administrator u vašoj tvrtki ili ustanovi možete kontrolirati mogu li vaši korisnici koristiti neobavezna povezana iskustva prilikom korištenja aplikacija Office za web, kao što su Word za web ili PowerPoint za web. Ta je mogućnost dostupna vašim korisnicima samo ako su prijavljeni pomoću računa tvrtke ili obrazovne ustanove prilikom korištenja aplikacija Office za web. Da biste kontrolirali jesu li povezana iskustva te vrste dostupna vašim korisnicima, možete koristiti postavku pravilnika *Dopusti korištenje dodatnih neobaveznih povezanih iskustava u sustavu Office*.

## <a name="overview-of-optional-connected-experiences"></a>Pregled neobaveznih povezanih iskustava

Neobavezna povezana iskustva jesu servisi u oblaku koji su dostupni korisnicima prilikom korištenja sustava Office. Primjeri neobaveznih povezanih iskustva uključuju stvaranje grafikona s kartom u programu Excel ili umetanje mrežne slike u dokument programa Word, koje se oslanjaju na servise koje nudi Microsoft Bing. Upotreba servisa u oblaku nije obavezna. 

Neobavezna povezana iskustva nisu obuhvaćena komercijalnim ugovorom vaše tvrtke ili ustanove s Microsoftom. Umjesto toga, neobavezna povezana iskustva Microsoft izravno nudi vašim korisnicima te su ona regulirana [Microsoftovim ugovorom o pružanju usluga](https://www.microsoft.com/servicesagreement). U nekim se slučajevima putem tih neobaveznih povezanih iskustava nudi sadržaj ili funkcije trećih strana te se mogu primjenjivati i drugi uvjeti.

Neka neobavezna povezana iskustva možda nisu dostupna u aplikacijama Office za web, ali su dostupna prilikom korištenja drugih verzija sustava Office, kao što je verzija za stolna računala na uređaju sa sustavom Windows.

Dodatne informacije potražite u članku [Pregled neobaveznih povezanih iskustava za Office](optional-connected-experiences.md).

## <a name="configure-the-policy-setting-by-using-the-office-cloud-policy-service"></a>Konfiguriranje postavki pravilnika pomoću servisa za pravilnike u oblaku sustava Office

Da biste kontrolirali jesu li povezana iskustva te vrste dostupna vašim korisnicima, možete koristiti postavku pravilnika *Dopusti korištenje dodatnih neobaveznih povezanih iskustava u sustavu Office*. Da biste konfigurirali tu postavku pravilnika za aplikacije Office za web, morate koristiti [Servis za pravilnike u oblaku sustava Office](../overview-office-cloud-policy-service.md).  

Ako ne konfigurirate tu postavku pravilnika, vaši će korisnici moći odabrati hoće li koristiti neobavezna povezana iskustva. Ako onemogućite tu postavku pravilnika, vaši korisnici neće moći koristiti ni jedno od neobaveznih povezanih iskustava.

Postavka pravilnika za aplikacije Office za web odnosi se na to kada korisnici rade na dokumentima sustava Office spremljenim na web-prostor za pohranu tvrtke Microsoft, kao što su OneDrive za tvrtke ili SharePoint Online.

Budući da koristite servis za pravilnike u oblaku sustava Office, ta se postavka pravilnika odnosi i na to kada korisnici koriste Office na uređajima sa sustavom Windows, Mac, iOS ili Android. Tu postavku pravilnika nije moguće konfigurirati samo za one instance kada vaši korisnici koriste aplikacije Office za web. No možete stvoriti konfiguraciju pravilnika koja obuhvaća tu postavku pravilnika, a ta se konfiguracija pravilnika može primjenjivati samo na korisnike koji anonimno pristupaju dokumentima pomoću aplikacija Office za web.

Ako odaberete da korisnicima budu dostupna neobavezna povezana iskustva, vašim će se korisnicima prikazati obavijest o zaštiti privatnosti prilikom prvog korištenja aplikacije Office za web. Ta obavijest korisnicima omogućuje da znaju da ste im pružili mogućnost korištenja tih neobaveznih povezanih iskustava. Obavijest također obavještava korisnike da se neobavezna povezana iskustva pružaju na temelju Microsoftovog ugovora o pružanju usluga. Budući da je ta obavijest važna informacija za korisnike, ta se obavijest mora prikazati i ne može se isključiti, sakriti ni prihvatiti u ime korisnika.

## <a name="users-can-choose-to-turn-off-optional-connected-experiences"></a>Korisnici mogu odabrati isključiti neobavezna povezana iskustva

Ako odaberete da korisnicima budu dostupna neobavezna povezana iskustva, vaši korisnici mogu ići u [postavke zaštite privatnosti račun](https://support.microsoft.com/office/3e7bc183-bf52-4fd0-8e6b-78978f7f121b#ID0EAADAAA=Online) te isključiti pristup neobaveznim povezanim iskustvima. Taj je odabir dostupan u postavkama privatnosti računa samo ako su korisnici prijavljeni pomoću računa tvrtke ili obrazovne ustanove. Ne postoji način na koji vi, kao administrator, možete onemogućiti pojedinačnim korisnicima u vašoj tvrtki ili ustanovi da isključite pristup neobaveznim povezanim iskustvima u pripadajućim postavkama zaštite privatnosti računa ako ste korisnicima dodijelili mogućnost korištenja neobaveznih povezanih iskustava.

## <a name="related-articles"></a>Povezani članci

- [Pregled kontrola za zaštitu privatnosti za Microsoft 365 Apps za velike tvrtke](overview-privacy-controls.md)
- [Upotreba postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Microsoft 365 Apps za velike tvrtke](manage-privacy-controls.md)
- [Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office za Mac](mac-privacy-preferences.md)
- [Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office na iOS uređajima](ios-privacy-preferences.md)
- [Korištenje postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Office na Android uređajima](android-privacy-controls.md)