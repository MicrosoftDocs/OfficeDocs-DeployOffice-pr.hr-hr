---
title: Upotreba postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Office na uređajima sa sustavom Android
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
description: Administratorima sustava Office nudi informacije o upravljanju postavkama zaštite privatnosti za Office na uređajima sa sustavom Android.
hideEdit: true
ms.openlocfilehash: 6086ecd1b2cd55bbf6cb4577879714f1d20a2f93
ms.sourcegitcommit: 81295dff0f2fa474f0db39fd40560e3a23fff32a
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45092110"
---
# <a name="use-policy-settings-to-manage-privacy-controls-for-office-on-android-devices"></a>Upotreba postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Office na uređajima sa sustavom Android

Postoje postavke pravila za Office na uređajima sa sustavom Android kojima se omogućuje kontrola nad postavkama povezanima sa sljedećim:

- ***Dijagnostički podaci*** koji se prikupljaju i šalju Microsoftu o klijentskom softveru sustava Office koji se upotrebljava.

- ***Povezana iskustva*** koja se koriste funkcijom utemeljenoj na oblaku da bi vama i vašim korisnicima ponudila poboljšane značajke sustava Office.

Dodatne informacije o dijagnostičkim podacima i povezanim iskustvima potražite u članku [Pregled kontrola zaštite privatnosti](overview-privacy-controls.md).

Te se postavke pravilnika odnose na sljedeće aplikacije:
- Verziju 16.0.12228.20260 i novije aplikacije Word za Android, Excel za Android i PowerPoint za Android.
- Verziju 4.1.71 i noviju aplikacije Outlook za Android.
- Verziju 16.0.12228.20004 i noviju aplikacije OneNote za Android.
- Verziju 5.47 i noviju aplikacije OneDrive za Android.
- Verziju 16.0.12430.20254 i noviju aplikacije Office za Android.

## <a name="policy-settings-available-for-office-on-android-devices"></a>Postavke pravilnika dostupne za Office na uređajima sa sustavom Android

U tablici u nastavku navedene su postavke pravilnika za Office na uređajima sa sustavom Android i veza na dodatne informacije o svakoj postavci pravilnika.

> [!NOTE]
>- Dodatne dostupne informacije pokrivaju postavke pravilnika za Office na uređajima sa sustavom Windows. Ali te se informacije odnose na Office na uređajima sa sustavom Android jer imaju iste postavke pravilnika.
>- Postavka pravilnika *Dopuštanje upotrebe povezanih iskustava u sustavu Office* koja je dostupna za Office na uređajima sa sustavom Windows ne odnosi se na Office na uređajima sa sustavom Android. 


|Naziv postavke pravilnika  |Dodatne informacije |
|---------|---------|
|Konfiguriranje razine dijagnostičkih podataka o klijentskom softveru koje Office šalje Microsoftu|[Postavka pravilnika za dijagnostičke podatke](manage-privacy-controls.md#policy-setting-for-diagnostic-data)         |
|Dopusti upotrebu povezanih iskustava koja analiziraju sadržaj u sustavu Office| [Postavka pravilnika za povezana iskustva koja analiziraju vaš sadržaj](manage-privacy-controls.md#policy-setting-for-connected-experiences-that-analyze-your-content)        |
|Dopusti upotrebu povezanih iskustava koja preuzimaju internetski sadržaj u sustavu Office |[Postavka pravilnika za povezana iskustva koja preuzimaju internetski sadržaj](manage-privacy-controls.md#policy-setting-for-connected-experiences-that-download-online-content)         |
|Dopusti upotrebu dodatnih neobaveznih povezanih iskustava u sustavu Office |[Postavka pravilnika za neobavezna povezana iskustva](manage-privacy-controls.md#policy-setting-for-optional-connected-experiences)|



## <a name="use-office-cloud-policy-service-to-apply-policy-settings"></a>Upotreba servisa pravilnika u oblaku sustava Office radi primjene postavki pravilnika

Da biste primijenili bilo koju od te 4 postavke pravilnika za Office na uređajima sa sustavom Android, morate upotrijebiti servis pravilnika u oblaku sustava Office. Dodatne informacije o upotrebi servisa pravilnika u oblaku sustava Office potražite u članku [Pregled servisa pravilnika u oblaku sustava Office](../overview-office-cloud-policy-service.md).

> [!NOTE]
> Ako ste prethodno upotrijebili servis pravilnika u oblaku sustava Office da biste konfigurirali te postavke pravilnika za Office na uređajima sa sustavom Windows, te će se postavke primjenjivati u sustavu Office na uređajima sa sustavom Android. Da biste to učinili, samo se morate prijaviti na servis pravilnika u oblaku sustava Office i servis će automatski primijeniti postavke na Office na uređajima sa sustavom Android.
