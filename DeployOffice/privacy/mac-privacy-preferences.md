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
ms.openlocfilehash: 01bb31f3b6c307ec1dc4762b54fea17185dcf27d
ms.sourcegitcommit: 0fd23324ba1364fa1f8dd1578adf25946adde90f
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/07/2019
ms.locfileid: "36246258"
---
# <a name="use-preferences-to-manage-privacy-controls-for-office-for-mac"></a><span data-ttu-id="07482-103">Upotreba postavki za upravljanje kontrolama za zaštitu privatnosti za Office za Mac</span><span class="sxs-lookup"><span data-stu-id="07482-103">Use preferences to manage privacy controls for Office for Mac</span></span>

<span data-ttu-id="07482-104">Počevši od verzije 16.28 sustava Office za Mac, postoje nove postavke preferenci kojima se omogućuje kontrola nad postavkama povezanima sa sljedećim:</span><span class="sxs-lookup"><span data-stu-id="07482-104">Starting with Version 1904 of Office 365 ProPlus, there are new policy settings that will allow you to control settings related to the following:</span></span>

- <span data-ttu-id="07482-105">***Dijagnostički podaci*** koji se prikupljaju i šalju Microsoftu o klijentskom softveru sustava Office koji se upotrebljava.</span><span class="sxs-lookup"><span data-stu-id="07482-105">***Diagnostic data*** that is collected and sent to Microsoft about Office client software being used</span></span>

- <span data-ttu-id="07482-106">***Povezana iskustva*** koja se koriste funkcijom utemeljenoj na oblaku da bi vama i vašim korisnicima ponudila poboljšane značajke sustava Office.</span><span class="sxs-lookup"><span data-stu-id="07482-106">***Connected experiences*** that use cloud-based functionality to provide enhanced Office features to you and your users.</span></span>

<span data-ttu-id="07482-107">Osim toga, tu je i nova postavka preferenci koja se odnosi na dijalog **Potrebne podatkovne obavijesti** za Microsoft AutoUpdate (MAU).</span><span class="sxs-lookup"><span data-stu-id="07482-107">In addition, there is a new preference setting related to a **Required Data Notice** dialog for Microsoft AutoUpdate (MAU).</span></span>

<span data-ttu-id="07482-108">Dodatne informacije o dijagnostičkim podacima i povezanim iskustvima potražite u članku Pregled kontrola zaštite privatnosti](overview-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="07482-108">For more information about diagnostic data and connected experiences, see [Overview of privacy controls](overview-privacy-controls.md).</span></span>

> [!NOTE]
> <span data-ttu-id="07482-109">Dodatne informacije o sličnim postavkama za Office na računalima sa sustavom Windows potražite u članku [Upotreba postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Office 365 ProPlus](manage-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="07482-109">For information about similar settings for Office on computers running Windows, see [Use policy settings to manage privacy controls for Office 365 ProPlus](manage-privacy-controls.md)</span></span>

## <a name="setting-preferences"></a><span data-ttu-id="07482-110">Postavke preferenci</span><span class="sxs-lookup"><span data-stu-id="07482-110">Setting preferences</span></span>

<span data-ttu-id="07482-111">Te su nove postavke značajke CFPreference API-ja kompatibilne i mogu se postaviti s pomoću `defaults` naredbe u terminalu ili se primijeniti s pomoću profila za konfiguraciju ili poslužitelja za upravljanje mobilnim uređajima (MDM).</span><span class="sxs-lookup"><span data-stu-id="07482-111">These new preference settings are CFPreferences API compatible and can be set using the `defaults` command in Terminal, or enforced through a Configuration Profile or Mobile Device Management (MDM) server.</span></span> <span data-ttu-id="07482-112">Prilikom provedbe preferenci korisnici ne mogu promijeniti vrijednosti, a sve će se kontrole u aplikaciji prikazati onemogućenima.</span><span class="sxs-lookup"><span data-stu-id="07482-112">When the preferences are enforced, the user cannot change the values, and any in-app controls will appear disabled.</span></span>

## <a name="preference-setting-for-diagnostic-data"></a><span data-ttu-id="07482-113">Postavka preferenci za dijagnostičke podatke</span><span class="sxs-lookup"><span data-stu-id="07482-113">Policy setting for diagnostic data</span></span>

<span data-ttu-id="07482-114">Dijagnostički se podaci upotrebljavaju da bi Office uvijek bio siguran i ažuran, kao i radi otkrivanja, dijagnosticiranja i otklanjanja problema te poboljšavanja proizvoda.</span><span class="sxs-lookup"><span data-stu-id="07482-114">Diagnostic data is used to keep Office secure and up-to-date, detect, diagnose and remediate problems, and also make product improvements.</span></span> <span data-ttu-id="07482-115">Za više informacija pogledajte [Dijagnostički podaci koje Office 365 ProPlus šalje Microsoftu](overview-privacy-controls.md#diagnostic-data-sent-from-office-365-proplus-to-microsoft).</span><span class="sxs-lookup"><span data-stu-id="07482-115">Diagnostic data sent from Office 365 ProPlus to Microsoft</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07482-116">**Preference Domain**</span><span class="sxs-lookup"><span data-stu-id="07482-116">**Preference Domain**</span></span>  | `com.microsoft.office` |
|<span data-ttu-id="07482-117">**Tipka**</span><span class="sxs-lookup"><span data-stu-id="07482-117">**Key**</span></span>  | `DiagnosticDataTypePreference`  |
|<span data-ttu-id="07482-118">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="07482-118">**Data Type**</span></span>  | <span data-ttu-id="07482-119">Niz</span><span class="sxs-lookup"><span data-stu-id="07482-119">String</span></span> |
|<span data-ttu-id="07482-120">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="07482-120">**Possible values**</span></span>  | <span data-ttu-id="07482-121">`BasicDiagnosticData` *(time se razina postavlja na Obvezno)*</span><span class="sxs-lookup"><span data-stu-id="07482-121">`BasicDiagnosticData` *(this sets the level to Required)*</span></span> <br/> <span data-ttu-id="07482-122">`FullDiagnosticData` *(time se razina postavlja na Neobvezno)*</span><span class="sxs-lookup"><span data-stu-id="07482-122">`FullDiagnosticData` *(this sets the level to Optional)*</span></span> <br/> <span data-ttu-id="07482-123">`ZeroDiagnosticData` *(time se razina postavlja na Nijedno)*</span><span class="sxs-lookup"><span data-stu-id="07482-123">`ZeroDiagnosticData` *(this sets the level to Neither)*</span></span> |
|<span data-ttu-id="07482-124">**Dostupnost**</span><span class="sxs-lookup"><span data-stu-id="07482-124">**Availability**</span></span> |<span data-ttu-id="07482-125">16.28 i novija</span><span class="sxs-lookup"><span data-stu-id="07482-125">16.28 and later</span></span> |

> [!NOTE]
> <span data-ttu-id="07482-126">Ako postavite tu preferencu, primjenjivat će se i na sljedeće proizvode:</span><span class="sxs-lookup"><span data-stu-id="07482-126">If you set this preference, it also will apply to the following products:</span></span>
> - <span data-ttu-id="07482-127">Verzija 1.00.217856 i novija programa Teams za Mac</span><span class="sxs-lookup"><span data-stu-id="07482-127">Version 1.00.217856 and later of Teams for Mac</span></span>
> - <span data-ttu-id="07482-128">Verzija 16.28 i novija programa Skype za tvrtke za Mac</span><span class="sxs-lookup"><span data-stu-id="07482-128">Version 16.28 and later of Skype for Business for Mac</span></span>

<span data-ttu-id="07482-129">Ako ne postavite tu preferencu, Microsoftu se šalju neobavzni i obvezni dijagnostički podaci ako su korisnici s pretplatom na Office 365 prijavljeni s pomoću računa poduzeća ili obrazovne ustanove ili ako korisnici imaju licencirane verzije sustava Office 2019 za Mac.</span><span class="sxs-lookup"><span data-stu-id="07482-129">If you don't set this preference, both optional and required diagnostic data is sent to Microsoft if users with an Office 365 subscription are signed in with a work or school account or if users have a volume licensed version of Office 2019 for Mac.</span></span> <span data-ttu-id="07482-130">Osim toga, ti korisnici ne mogu promijeniti razinu dijagnostičkih podataka bez obzira na to kako postavite tu preferencu.</span><span class="sxs-lookup"><span data-stu-id="07482-130">Also, these users can't change the level of diagnostic data regardless of how you set this preference.</span></span>

<span data-ttu-id="07482-131">Drugim korisnicima, kao što su privatni korisnici s pretplatom na Office 365, šalju se samo obvezni dijagnostički podaci, osim ako korisnik odabere da šalje i neobvezne dijagnostičke podatke odlaskom na **Preference** > **Privatnost**.</span><span class="sxs-lookup"><span data-stu-id="07482-131">For other users, such as home users with an Office 365 subscription, only required diagnostic data is sent, unless the user chooses to also send optional diagnostic data by going to **Preferences** > **Privacy**.</span></span>

## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a><span data-ttu-id="07482-132">Postavka preferenci za povezana iskustva kojima se analizira vaš sadržaj</span><span class="sxs-lookup"><span data-stu-id="07482-132">Policy setting for connected experiences that analyze your content</span></span>

<span data-ttu-id="07482-133">Povezana iskustva koja analiziraju vaš sadržaj iskustva su koja koriste vaš sadržaj iz sustava Office da bi vam ponudila preporuke dizajna, prijedloge za uređivanje, uvide u podatke i slične značajke.</span><span class="sxs-lookup"><span data-stu-id="07482-133">Connected experiences that analyze your content are experiences that use your Office content to provide you with design recommendations, editing suggestions, data insights, and similar features.</span></span> <span data-ttu-id="07482-134">Na primjer, PowerPoint Designer ili Istraživač u programu Word.</span><span class="sxs-lookup"><span data-stu-id="07482-134">For example, PowerPoint Designer or Editor in Word.</span></span> <span data-ttu-id="07482-135">Popis tih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="07482-135">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07482-136">**Preference Domain**</span><span class="sxs-lookup"><span data-stu-id="07482-136">**Preference Domain**</span></span>  | `com.microsoft.office` |
|<span data-ttu-id="07482-137">**Tipka**</span><span class="sxs-lookup"><span data-stu-id="07482-137">**Key**</span></span>  | `OfficeExperiencesAnalyzingContentPreference`  |
|<span data-ttu-id="07482-138">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="07482-138">**Data Type**</span></span>  | <span data-ttu-id="07482-139">Booleov</span><span class="sxs-lookup"><span data-stu-id="07482-139">Boolean</span></span> |
|<span data-ttu-id="07482-140">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="07482-140">**Possible values**</span></span>  | <span data-ttu-id="07482-141">`TRUE` *(omogućeno)*</span><span class="sxs-lookup"><span data-stu-id="07482-141">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="07482-142">`FALSE` *(onemogućeno)*</span><span class="sxs-lookup"><span data-stu-id="07482-142">`FALSE` *(disabled)*</span></span>|
|<span data-ttu-id="07482-143">**Dostupnost**</span><span class="sxs-lookup"><span data-stu-id="07482-143">**Availability**</span></span> |<span data-ttu-id="07482-144">16.28 i novija</span><span class="sxs-lookup"><span data-stu-id="07482-144">16.28 and later</span></span> |

<span data-ttu-id="07482-145">Ako ne postavite tu preferencu, povezana iskustva kojima se analizira sadržaj dostupna su korisnicima.</span><span class="sxs-lookup"><span data-stu-id="07482-145">If you don't set this preference, connected experiences that analyze content are available to users.</span></span> 

<span data-ttu-id="07482-146">Ako korisnik ima pretplatu na Office 365 te se prijavi s pomoću računa poduzeća ili obrazovne ustanove ili ako ima licenciranu verziju sustava Office 2019 za Mac, ne može isključiti povezana iskustva kojima se analizira sadržaj.</span><span class="sxs-lookup"><span data-stu-id="07482-146">If the user has an Office 365 subscription and is signed in with a work or school account or if the user has a volume licensed version of Office 2019 for Mac, then the user can't turn off connected experiences that analyze content.</span></span>

<span data-ttu-id="07482-147">Za druge korisnike, kao što su korisnici s pretplatom na Office 365, korisnik može odabrati da isključi povezana iskustva kojima se analizira sadržaj odlaskom na **Preference** > **Privatnost**.</span><span class="sxs-lookup"><span data-stu-id="07482-147">For other users, such as home users with an Office 365 subscription, the user can choose to turn off connected experiences that analyze content by going to **Preferences** > **Privacy**.</span></span>

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a><span data-ttu-id="07482-148">Postavka preferenci za povezana iskustva kojima se preuzima internetski sadržaj</span><span class="sxs-lookup"><span data-stu-id="07482-148">Policy setting for connected experiences that download online content</span></span>

<span data-ttu-id="07482-149">Povezana iskustva koja preuzimaju internetski sadržaj iskustva su koja omogućuju pretraživanje i preuzimanje internetskih sadržaja – uključujući predloške, slike, 3D modele, videozapise i referentne materijale – radi poboljšavanja vaših dokumenata.</span><span class="sxs-lookup"><span data-stu-id="07482-149">Connected experiences that download online content are experiences that allow you to search and download online content including templates, images, 3D models, videos, and reference materials to enhance your documents.</span></span> <span data-ttu-id="07482-150">Na primjer, predlošci sustava Office ili alat za brz početak rada s programom PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="07482-150">For example, Office templates or PowerPoint QuickStarter.</span></span> <span data-ttu-id="07482-151">Popis tih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="07482-151">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07482-152">**Preference Domain**</span><span class="sxs-lookup"><span data-stu-id="07482-152">**Preference Domain**</span></span>  | `com.microsoft.office` |
|<span data-ttu-id="07482-153">**Tipka**</span><span class="sxs-lookup"><span data-stu-id="07482-153">**Key**</span></span>  | `OfficeExperiencesDownloadingContentPreference`  |
|<span data-ttu-id="07482-154">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="07482-154">**Data Type**</span></span>  | <span data-ttu-id="07482-155">Booleov</span><span class="sxs-lookup"><span data-stu-id="07482-155">Boolean</span></span> |
|<span data-ttu-id="07482-156">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="07482-156">**Possible values**</span></span>  | <span data-ttu-id="07482-157">`TRUE` *(omogućeno)*</span><span class="sxs-lookup"><span data-stu-id="07482-157">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="07482-158">`FALSE` *(onemogućeno)*</span><span class="sxs-lookup"><span data-stu-id="07482-158">`FALSE` *(disabled)*</span></span>|
|<span data-ttu-id="07482-159">**Dostupnost**</span><span class="sxs-lookup"><span data-stu-id="07482-159">**Availability**</span></span> |<span data-ttu-id="07482-160">16.28 i novija</span><span class="sxs-lookup"><span data-stu-id="07482-160">16.28 and later</span></span> |

<span data-ttu-id="07482-161">Ako ne postavite tu preferencu, povezana iskustva kojima se preuzima internetski sadržaj dostupna su korisnicima.</span><span class="sxs-lookup"><span data-stu-id="07482-161">If you don't set this preference, connected experiences that download online content are available to users.</span></span>

<span data-ttu-id="07482-162">Ako korisnik ima pretplatu na Office 365 te se prijavi s pomoću računa poduzeća ili obrazovne ustanove ili ako ima licenciranu verziju sustava Office 2019 za Mac, ne može isključiti povezana iskustva kojima se preuzima internetski sadržaj.</span><span class="sxs-lookup"><span data-stu-id="07482-162">If the user has an Office 365 subscription and is signed in with a work or school account or if the user has a volume licensed version of Office 2019 for Mac, then the user can't turn off connected experiences that download online content.</span></span>

<span data-ttu-id="07482-163">Za druge korisnike, kao što su korisnici s pretplatom na Office 365, korisnik može odabrati da isključi povezana iskustva kojima se preuzima internetski sadržaj odlaskom na **Preference** > **Privatnost**.</span><span class="sxs-lookup"><span data-stu-id="07482-163">For other users, such as home users with an Office 365 subscription, a user can choose to turn off connected experiences that download online content by going to **Preferences** > **Privacy**.</span></span>

## <a name="preference-setting-for-optional-connected-experiences"></a><span data-ttu-id="07482-164">Postavka preferenci za neobvezna povezana iskustva</span><span class="sxs-lookup"><span data-stu-id="07482-164">Policy setting for optional connected experiences</span></span>

<span data-ttu-id="07482-165">Osim prethodno spomenutih povezanih iskustava postoje i neka neobvezna povezana iskustva za koja korisnicima možete omogućiti da im pristupaju upotrebom računa poduzeća ili ustanove, koji se ponekad naziva račun poduzeća ili račun obrazovne ustanove.</span><span class="sxs-lookup"><span data-stu-id="07482-165">In addition to the connected experiences mentioned above, there are some optional connected experiences that you may choose to allow your users to access with their organization account, which is sometimes referred to as a work or school account.</span></span> <span data-ttu-id="07482-166">Na primjer, značajke povezane uz LinkedIn u pomoćniku za životopis u programu Word ili Traka vremenske prognoze u programu Outlook, koja se koristi servisom MSN Vrijeme.</span><span class="sxs-lookup"><span data-stu-id="07482-166">For example, the LinkedIn features of the Resume Assistant in Word or the 3D Maps feature in Excel, which uses Bing.</span></span> <span data-ttu-id="07482-167">Dodatne primjere potražite u članku [Pregled neobveznih povezanih iskustava za Office](optional-connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="07482-167">For more examples, see [Overview of optional connected experiences in Office](optional-connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07482-168">**Preference Domain**</span><span class="sxs-lookup"><span data-stu-id="07482-168">**Preference Domain**</span></span>  | `com.microsoft.office` |
|<span data-ttu-id="07482-169">**Tipka**</span><span class="sxs-lookup"><span data-stu-id="07482-169">**Key**</span></span>  | `OptionalConnectedExperiencesPreference`  |
|<span data-ttu-id="07482-170">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="07482-170">**Data Type**</span></span>  | <span data-ttu-id="07482-171">Booleov</span><span class="sxs-lookup"><span data-stu-id="07482-171">Boolean</span></span> |
|<span data-ttu-id="07482-172">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="07482-172">**Possible values**</span></span>  | <span data-ttu-id="07482-173">`TRUE` *(omogućeno)*</span><span class="sxs-lookup"><span data-stu-id="07482-173">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="07482-174">`FALSE` *(onemogućeno)*</span><span class="sxs-lookup"><span data-stu-id="07482-174">`FALSE` *(disabled)*</span></span>|
|<span data-ttu-id="07482-175">**Dostupnost**</span><span class="sxs-lookup"><span data-stu-id="07482-175">**Availability**</span></span> |<span data-ttu-id="07482-176">16.28 i novija</span><span class="sxs-lookup"><span data-stu-id="07482-176">16.28 and later</span></span> |

<span data-ttu-id="07482-177">Ako ne postavite tu preferencu, neobvezna povezana iskustva dostupna su korisnicima s pretplatom na Office 365 na koji se prijavljuje s pomoću računa poduzeća ili obrazovne ustanove ili korisnicima koji imaju licencirane verzije sustava Office 2019 za Mac.</span><span class="sxs-lookup"><span data-stu-id="07482-177">If you don't set this preference, optional connected experiences are available to users with an Office 365 subscription that are signed in with a work or school account or users who have a volume licensed version of Office 2019 for Mac.</span></span> <span data-ttu-id="07482-178">Osim ako niste postavili tu preferencu na `FALSE`, ti korisnici mogu odabrati da isključe neobvezno povezano iskustvo odlaskom na **Preference** > **Privatnost**.</span><span class="sxs-lookup"><span data-stu-id="07482-178">Unless you have set this preference to `FALSE`, these users can choose to turn off optional connected experiences by going to **Preferences** > **Privacy**.</span></span>

<span data-ttu-id="07482-179">Za druge korisnike, kao što su privatni korisnici s pretplatom na Office 365, ne postoji opcija isključivanja neobveznih povezanih iskustava.</span><span class="sxs-lookup"><span data-stu-id="07482-179">For other users, such as home users with an Office 365 subscription, there isn't an option to turn off optional connected experiences.</span></span>

## <a name="preference-setting-for-most-connected-experiences"></a><span data-ttu-id="07482-180">Postavka preferenci za većinu povezanih iskustava</span><span class="sxs-lookup"><span data-stu-id="07482-180">Policy setting for most connected experiences</span></span>

<span data-ttu-id="07482-181">Tu preferencu možete upotrijebiti kako biste kontrolirali je li većina povezanih iskustava dostupna vašim korisnicima.</span><span class="sxs-lookup"><span data-stu-id="07482-181">You can use this preference to control whether most connected experiences are available to your users.</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07482-182">**Preference Domain**</span><span class="sxs-lookup"><span data-stu-id="07482-182">**Preference Domain**</span></span>  | `com.microsoft.office` |
|<span data-ttu-id="07482-183">**Tipka**</span><span class="sxs-lookup"><span data-stu-id="07482-183">**Key**</span></span>  | `ConnectedOfficeExperiencesPreference`  |
|<span data-ttu-id="07482-184">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="07482-184">**Data Type**</span></span>  | <span data-ttu-id="07482-185">Booleov</span><span class="sxs-lookup"><span data-stu-id="07482-185">Boolean</span></span> |
|<span data-ttu-id="07482-186">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="07482-186">**Possible values**</span></span>  | <span data-ttu-id="07482-187">`TRUE` *(omogućeno)*</span><span class="sxs-lookup"><span data-stu-id="07482-187">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="07482-188">`FALSE` *(onemogućeno)*</span><span class="sxs-lookup"><span data-stu-id="07482-188">`FALSE` *(disabled)*</span></span>|
|<span data-ttu-id="07482-189">**Dostupnost**</span><span class="sxs-lookup"><span data-stu-id="07482-189">**Availability**</span></span> |<span data-ttu-id="07482-190">16.28 i novija</span><span class="sxs-lookup"><span data-stu-id="07482-190">16.28 and later</span></span> |

<span data-ttu-id="07482-191">Ako ne postavite tu preferencu, sva su povezana iskustva dostupna vašim korisnicima, osim ako ste postavili neku od drugih preferenci za povezana iskustva koja su prethodno navedena, kao na primjer `OfficeExperiencesAnalyzingContentPreference`.</span><span class="sxs-lookup"><span data-stu-id="07482-191">If you don't set this preference, all connected experiences are available to your users, unless you have set one of the other preferences for connected experiences previously mentioned, such as `OfficeExperiencesAnalyzingContentPreference`.</span></span>

<span data-ttu-id="07482-192">Na primjer, ako ovu preferencu postavite na `FALSE`, sljedeće vrste povezanih iskustava neće biti dostupne vašim korisnicima:</span><span class="sxs-lookup"><span data-stu-id="07482-192">For example, if you set this preference to `FALSE`, the following types of connected experiences won't be available to your users:</span></span>
- <span data-ttu-id="07482-193">iskustva koja analiziraju sadržaj</span><span class="sxs-lookup"><span data-stu-id="07482-193">Experiences that analyze your content</span></span>
- <span data-ttu-id="07482-194">iskustva koja preuzimaju internetski sadržaj</span><span class="sxs-lookup"><span data-stu-id="07482-194">Experiences that download online content</span></span>
- <span data-ttu-id="07482-195">neobavezna povezana iskustva</span><span class="sxs-lookup"><span data-stu-id="07482-195">Optional connected experiences</span></span>

<span data-ttu-id="07482-196">Usto, ako podesite ovu preferencu na `FALSE`, isključuje se i većina drugih povezanih iskustava, kao što su suautorstvo i internetski prostor za pohranu datoteka.</span><span class="sxs-lookup"><span data-stu-id="07482-196">In addition, if you disable this policy setting, most other connected experiences are also turned off, such as co-authoring and online file storage.</span></span> <span data-ttu-id="07482-197">Popis tih drugih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="07482-197">For a list of these other connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

<span data-ttu-id="07482-198">No čak i ako podesite ovu preferencu na`FALSE`, ostat će dostupna ograničena funkcionalnost sustava Office, kao što je sinkronizacija poštanskog sandučića u programu Outlook, pa će Teams i Skype za tvrtke i dalje funkcionirati.</span><span class="sxs-lookup"><span data-stu-id="07482-198">But even if you disable this policy setting, limited Office functionality will remain available, such as synching a mailbox in Outlook, and Teams and Skype for Business will continue to work.</span></span> <span data-ttu-id="07482-199">[Ključni servisi](essential-services.md), poput servisa za licenciranje, kojima se potvrđuje da imate ispravnu licenciju za upotrebu sustava Office, također će ostati dostupni.</span><span class="sxs-lookup"><span data-stu-id="07482-199">[Essential services](essential-services.md), such as the licensing service that confirms that you’re properly licensed to use Office, will also remain available.</span></span>

<span data-ttu-id="07482-200">Ako korisnik ima pretplatu na Office 365 te se prijavi s pomoću računa poduzeća ili obrazovne ustanove ili ako ima licenciranu verziju sustava Office 2019 za Mac, ne može isključiti većinu povezanih iskustava.</span><span class="sxs-lookup"><span data-stu-id="07482-200">If the user has an Office 365 subscription and is signed in with a work or school account or if the user has a volume licensed version of Office 2019 for Mac, then the user can't turn off most connected experiences.</span></span>

<span data-ttu-id="07482-201">Za druge korisnike, kao što su privatni korisnici s pretplatom na Office 365, korisnik može odabrati da isključi većinu povezanih iskustava odlaskom na **Preference** > **Privatnost**.</span><span class="sxs-lookup"><span data-stu-id="07482-201">For other users, such as home users with an Office 365 subscription, a user can choose to turn off most connected experiences by going to **Preferences** > **Privacy**.</span></span>

## <a name="preference-setting-for-the-required-data-notice-dialog-for-microsoft-autoupdate"></a><span data-ttu-id="07482-202">Postavka preferenci u dijalogu potrebne podatkovne obavijesti za Microsoft AutoUpdate</span><span class="sxs-lookup"><span data-stu-id="07482-202">Preference setting for the Required Data Notice dialog for Microsoft AutoUpdate</span></span>

<span data-ttu-id="07482-203">Prvi put kada se pokrene verzija 4.12 ili novija programa Microsoft AutoUpdate (MAU), korisnici će vidjeti dijalog **Potrebne podatkovne obavijesti** kojim im se omogućuju informacije o podacima iz MAU-a koji se šalju Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="07482-203">The first time Version 4.12 or later of Microsoft AutoUpdate (MAU) is launched, users will see a **Required Data Notice** dialog which provides them with information about what data from MAU is sent to Microsoft.</span></span>

<span data-ttu-id="07482-204">Ako ne želite da korisnici vide dijalog **Potrebne podatkovne obavijesti** za Microsoft AutoUpdate, možete postaviti sljedeću preferencu.</span><span class="sxs-lookup"><span data-stu-id="07482-204">If you don't want your users to see this **Required Data Notice** dialog for Microsoft AutoUpdate, you can set the following preference.</span></span> <span data-ttu-id="07482-205">Bez obzira na to koju vrijednost postavite, dijalog se neće prikazati vašim korisnicima.</span><span class="sxs-lookup"><span data-stu-id="07482-205">Regardless of which value you set, the dialog won't be shown to your users.</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07482-206">**Preference Domain**</span><span class="sxs-lookup"><span data-stu-id="07482-206">**Preference Domain**</span></span>  | `com.microsoft.autoupdate2` |
|<span data-ttu-id="07482-207">**Tipka**</span><span class="sxs-lookup"><span data-stu-id="07482-207">**Key**</span></span>  | `AcknowledgedDataCollectionPolicy`  |
|<span data-ttu-id="07482-208">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="07482-208">**Data Type**</span></span>  | <span data-ttu-id="07482-209">Niz</span><span class="sxs-lookup"><span data-stu-id="07482-209">String</span></span> |
|<span data-ttu-id="07482-210">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="07482-210">**Possible values**</span></span>  | `RequiredDataOnly` <br/> `RequiredAndOptionalData`|
|<span data-ttu-id="07482-211">**Dostupnost**</span><span class="sxs-lookup"><span data-stu-id="07482-211">**Availability**</span></span> |<span data-ttu-id="07482-212">4.12 i novija</span><span class="sxs-lookup"><span data-stu-id="07482-212">4.12 and later</span></span> |

<span data-ttu-id="07482-213">Ako vašim korisnicima dopustite da vide ovaj dijalog, kada korisnik odabere**U redu**, vrijednost`RequiredDataOnly` zapisuje se u `AcknowledgedDataCollectionPolicy` i dijalog se više ne prikazuje korisniku.</span><span class="sxs-lookup"><span data-stu-id="07482-213">If you let your users see this dialog, then when the user chooses **OK**, the value `RequiredDataOnly` is written to `AcknowledgedDataCollectionPolicy` and the dialog is not shown to the user again.</span></span>


## <a name="related-topics"></a><span data-ttu-id="07482-214">Povezane teme</span><span class="sxs-lookup"><span data-stu-id="07482-214">Related topics</span></span>

- [<span data-ttu-id="07482-215">Referenca za konfiguraciju profila (dokumentacija za Appleove inženjere) </span><span class="sxs-lookup"><span data-stu-id="07482-215">Configuration Profile Reference (Apple developer documentation)</span></span>](https://go.microsoft.com/fwlink/p/?linkid=852998)
- [<span data-ttu-id="07482-216">Implementacija preferenci za Office za Mac</span><span class="sxs-lookup"><span data-stu-id="07482-216">Deploy preferences for Office for Mac</span></span>](../mac/deploy-preferences-for-office-for-mac.md)
- [<span data-ttu-id="07482-217">Postavke zaštite privatnosti računa</span><span class="sxs-lookup"><span data-stu-id="07482-217">Account Privacy Settings</span></span>](https://support.office.com/article/3e7bc183-bf52-4fd0-8e6b-78978f7f121b#ID0EAADAAA=Mac)
