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
ms.openlocfilehash: a1fdd9f7d0fe2095b3a32f61f885f724f2259188
ms.sourcegitcommit: 02c4120c0b10bfe378d21d60699ae49aaef97834
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/15/2019
ms.locfileid: "37510205"
---
# <a name="use-preferences-to-manage-privacy-controls-for-office-for-mac"></a><span data-ttu-id="8577e-103">Upotreba postavki za upravljanje kontrolama za zaštitu privatnosti za Office za Mac</span><span class="sxs-lookup"><span data-stu-id="8577e-103">Use preferences to manage privacy controls for Office for Mac</span></span>

<span data-ttu-id="8577e-104">Počevši od verzije 16.28 sustava Office za Mac, postoje nove postavke preferenci kojima se omogućuje kontrola nad postavkama povezanima sa sljedećim:</span><span class="sxs-lookup"><span data-stu-id="8577e-104">Starting with Version 1904 of Office 365 ProPlus, there are new policy settings that will allow you to control settings related to the following:</span></span>

- <span data-ttu-id="8577e-105">***Dijagnostički podaci*** koji se prikupljaju i šalju Microsoftu o klijentskom softveru sustava Office koji se upotrebljava.</span><span class="sxs-lookup"><span data-stu-id="8577e-105">***Diagnostic data*** that is collected and sent to Microsoft about Office client software being used</span></span>

- <span data-ttu-id="8577e-106">***Povezana iskustva*** koja se koriste funkcijom utemeljenoj na oblaku da bi vama i vašim korisnicima ponudila poboljšane značajke sustava Office.</span><span class="sxs-lookup"><span data-stu-id="8577e-106">***Connected experiences*** that use cloud-based functionality to provide enhanced Office features to you and your users.</span></span>

<span data-ttu-id="8577e-107">Osim toga, tu je i nova postavka preferenci koja se odnosi na dijalog **Potrebne podatkovne obavijesti** za Microsoft AutoUpdate (MAU).</span><span class="sxs-lookup"><span data-stu-id="8577e-107">In addition, there is a new preference setting related to a **Required Data Notice** dialog for Microsoft AutoUpdate (MAU).</span></span>

<span data-ttu-id="8577e-108">Dodatne informacije o dijagnostičkim podacima i povezanim iskustvima potražite u članku [Pregled kontrola zaštite privatnosti](overview-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="8577e-108">For more information about diagnostic data and connected experiences, see [Overview of privacy controls](overview-privacy-controls.md).</span></span>

> [!NOTE]
> - <span data-ttu-id="8577e-109">Informacije o sličnim postavkama za Office na računalima sa sustavom Windows potražite u članku [Upotreba postavki pravilnika za upravljanje kontrolama za zaštitu privatnosti za Office 365 ProPlus](manage-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="8577e-109">For information about similar settings for Office on computers running Windows, see [Use policy settings to manage privacy controls for Office 365 ProPlus](manage-privacy-controls.md).</span></span>
> - <span data-ttu-id="8577e-110">Informacije o sličnim postavkama za Office na iOS uređajima potražite u [Upotreba postavki za upravljanje kontrolama za zaštitu privatnosti za Office na iOS uređajima](ios-privacy-preferences.md).</span><span class="sxs-lookup"><span data-stu-id="8577e-110">For information about similar settings for Office on iOS devices, see [Use preferences to manage privacy controls for Office on iOS devices](ios-privacy-preferences.md).</span></span>

## <a name="setting-preferences"></a><span data-ttu-id="8577e-111">Postavke preferenci</span><span class="sxs-lookup"><span data-stu-id="8577e-111">Setting preferences</span></span>

<span data-ttu-id="8577e-112">Te su nove postavke značajke CFPreference API-ja kompatibilne i mogu se postaviti s pomoću `defaults` naredbe u terminalu ili se primijeniti s pomoću profila za konfiguraciju ili poslužitelja za upravljanje mobilnim uređajima (MDM).</span><span class="sxs-lookup"><span data-stu-id="8577e-112">These new preference settings are CFPreferences API compatible and can be set using the `defaults` command in Terminal, or enforced through a Configuration Profile or Mobile Device Management (MDM) server.</span></span> <span data-ttu-id="8577e-113">Prilikom provedbe preferenci korisnici ne mogu promijeniti vrijednosti, a sve će se kontrole u aplikaciji prikazati onemogućenima.</span><span class="sxs-lookup"><span data-stu-id="8577e-113">When the preferences are enforced, the user cannot change the values, and any in-app controls will appear disabled.</span></span>

## <a name="preference-setting-for-diagnostic-data"></a><span data-ttu-id="8577e-114">Postavka preferenci za dijagnostičke podatke</span><span class="sxs-lookup"><span data-stu-id="8577e-114">Policy setting for diagnostic data</span></span>

<span data-ttu-id="8577e-115">Dijagnostički se podaci upotrebljavaju da bi Office uvijek bio siguran i ažuran, kao i radi otkrivanja, dijagnosticiranja i otklanjanja problema te poboljšavanja proizvoda.</span><span class="sxs-lookup"><span data-stu-id="8577e-115">Diagnostic data is used to keep Office secure and up-to-date, detect, diagnose and remediate problems, and also make product improvements.</span></span> <span data-ttu-id="8577e-116">Za više informacija pogledajte [Dijagnostički podaci koje Office 365 ProPlus šalje Microsoftu](overview-privacy-controls.md#diagnostic-data-sent-from-office-365-proplus-to-microsoft).</span><span class="sxs-lookup"><span data-stu-id="8577e-116">Diagnostic data sent from Office 365 ProPlus to Microsoft</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8577e-117">**Preference Domain**</span><span class="sxs-lookup"><span data-stu-id="8577e-117">**Preference Domain**</span></span>  | `com.microsoft.office` |
|<span data-ttu-id="8577e-118">**Tipka**</span><span class="sxs-lookup"><span data-stu-id="8577e-118">**Key**</span></span>  | `DiagnosticDataTypePreference`  |
|<span data-ttu-id="8577e-119">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="8577e-119">**Data Type**</span></span>  | <span data-ttu-id="8577e-120">Niz</span><span class="sxs-lookup"><span data-stu-id="8577e-120">String</span></span> |
|<span data-ttu-id="8577e-121">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="8577e-121">**Possible values**</span></span>  | <span data-ttu-id="8577e-122">`BasicDiagnosticData` *(time se razina postavlja na Obvezno)*</span><span class="sxs-lookup"><span data-stu-id="8577e-122">`BasicDiagnosticData` *(this sets the level to Required)*</span></span> <br/> <span data-ttu-id="8577e-123">`FullDiagnosticData` *(time se razina postavlja na Neobvezno)*</span><span class="sxs-lookup"><span data-stu-id="8577e-123">`FullDiagnosticData` *(this sets the level to Optional)*</span></span> <br/> <span data-ttu-id="8577e-124">`ZeroDiagnosticData` *(time se razina postavlja na Nijedno)*</span><span class="sxs-lookup"><span data-stu-id="8577e-124">`ZeroDiagnosticData` *(this sets the level to Neither)*</span></span> |
|<span data-ttu-id="8577e-125">**Dostupnost**</span><span class="sxs-lookup"><span data-stu-id="8577e-125">**Availability**</span></span> |<span data-ttu-id="8577e-126">16.28 i novija</span><span class="sxs-lookup"><span data-stu-id="8577e-126">16.28 and later</span></span> |

<span data-ttu-id="8577e-127">Počevši s novim instalacijama verzije 16.30, ako ne postavite tu preferencu, Microsoftu se šalju samo obvezni dijagnostički podaci ako su korisnici s pretplatom na Office 365 prijavljeni s pomoću računa poduzeća ili obrazovne ustanove ili ako korisnici imaju licencirane verzije sustava Office 2019 za Mac.</span><span class="sxs-lookup"><span data-stu-id="8577e-127">Starting with new installations of Version 16.30, if you don't set this preference, only required diagnostic data is sent to Microsoft if users with an Office 365 subscription are signed in with a work or school account or if users have a volume licensed version of Office 2019 for Mac.</span></span> <span data-ttu-id="8577e-128">Osim toga, ti korisnici ne mogu promijeniti razinu dijagnostičkih podataka bez obzira na to kako postavite tu preferencu.</span><span class="sxs-lookup"><span data-stu-id="8577e-128">Also, these users can't change the level of diagnostic data regardless of how you set this preference.</span></span>

> [!NOTE]
> - <span data-ttu-id="8577e-129">Ako instalirate verziju 16,28 ili 16,29 te ne postavljate tu preferencu, Microsoftu se šalju neobavezni i obavezni dijagnostički podaci.</span><span class="sxs-lookup"><span data-stu-id="8577e-129">If you install Version 16.28 or 16.29 and you don't set this preference, both optional and required diagnostic data is sent to Microsoft.</span></span> <span data-ttu-id="8577e-130">Ako ste zatim nadogradili na verziju 16.30 ili noviju, Microsoftu će se i dalje slati neobavezni i obavezni dijagnostički podaci, osim ako ne koristite tu preferencu da biste postavili neku drugu vrijednost.</span><span class="sxs-lookup"><span data-stu-id="8577e-130">If you then upgrade to Version 16.30 or later, both optional and required diagnostic data is still sent to Microsoft, unless you use this preference to set a different value.</span></span>
> - <span data-ttu-id="8577e-131">Ako postavite tu preferencu, primjenjivat će se i na verzije 1.00.217856 i novije Teams za Mac,i na verziju 16.28 i novije verzije Skype za tvrtke za Mac.</span><span class="sxs-lookup"><span data-stu-id="8577e-131">If you set this preference, it also will apply to Version 1.00.217856 and later of Teams for Mac and to Version 16.28 and later of Skype for Business for Mac.</span></span>

<span data-ttu-id="8577e-132">Drugim korisnicima, kao što su privatni korisnici s pretplatom na Office 365, šalju se samo obavezni dijagnostički podaci, osim ako korisnik odabere da šalje i neobavezne dijagnostičke podatke odlaskom na **Preference** > **Privatnost**.</span><span class="sxs-lookup"><span data-stu-id="8577e-132">For other users, such as home users with an Office 365 subscription, only required diagnostic data is sent, unless the user chooses to also send optional diagnostic data by going to **Preferences** > **Privacy**.</span></span>

## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a><span data-ttu-id="8577e-133">Postavka preferenci za povezana iskustva kojima se analizira vaš sadržaj</span><span class="sxs-lookup"><span data-stu-id="8577e-133">Policy setting for connected experiences that analyze your content</span></span>

<span data-ttu-id="8577e-134">Povezana iskustva koja analiziraju vaš sadržaj iskustva su koja koriste vaš sadržaj iz sustava Office da bi vam ponudila preporuke dizajna, prijedloge za uređivanje, uvide u podatke i slične značajke.</span><span class="sxs-lookup"><span data-stu-id="8577e-134">Connected experiences that analyze your content are experiences that use your Office content to provide you with design recommendations, editing suggestions, data insights, and similar features.</span></span> <span data-ttu-id="8577e-135">Na primjer, PowerPoint Designer ili Istraživač u programu Word.</span><span class="sxs-lookup"><span data-stu-id="8577e-135">For example, PowerPoint Designer or Editor in Word.</span></span> <span data-ttu-id="8577e-136">Popis tih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="8577e-136">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8577e-137">**Preference Domain**</span><span class="sxs-lookup"><span data-stu-id="8577e-137">**Preference Domain**</span></span>  | `com.microsoft.office` |
|<span data-ttu-id="8577e-138">**Tipka**</span><span class="sxs-lookup"><span data-stu-id="8577e-138">**Key**</span></span>  | `OfficeExperiencesAnalyzingContentPreference`  |
|<span data-ttu-id="8577e-139">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="8577e-139">**Data Type**</span></span>  | <span data-ttu-id="8577e-140">Booleov</span><span class="sxs-lookup"><span data-stu-id="8577e-140">Boolean</span></span> |
|<span data-ttu-id="8577e-141">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="8577e-141">**Possible values**</span></span>  | <span data-ttu-id="8577e-142">`TRUE` *(omogućeno)*</span><span class="sxs-lookup"><span data-stu-id="8577e-142">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="8577e-143">`FALSE` *(onemogućeno)*</span><span class="sxs-lookup"><span data-stu-id="8577e-143">`FALSE` *(disabled)*</span></span>|
|<span data-ttu-id="8577e-144">**Dostupnost**</span><span class="sxs-lookup"><span data-stu-id="8577e-144">**Availability**</span></span> |<span data-ttu-id="8577e-145">16.28 i novija</span><span class="sxs-lookup"><span data-stu-id="8577e-145">16.28 and later</span></span> |

<span data-ttu-id="8577e-146">Ako ne postavite tu preferencu, povezana iskustva kojima se analizira sadržaj dostupna su korisnicima.</span><span class="sxs-lookup"><span data-stu-id="8577e-146">If you don't set this preference, connected experiences that analyze content are available to users.</span></span> 

<span data-ttu-id="8577e-147">Ako korisnik ima pretplatu na Office 365 te se prijavi s pomoću računa poduzeća ili obrazovne ustanove ili ako ima licenciranu verziju sustava Office 2019 za Mac, ne može isključiti povezana iskustva kojima se analizira sadržaj.</span><span class="sxs-lookup"><span data-stu-id="8577e-147">If the user has an Office 365 subscription and is signed in with a work or school account or if the user has a volume licensed version of Office 2019 for Mac, then the user can't turn off connected experiences that analyze content.</span></span>

<span data-ttu-id="8577e-148">Za druge korisnike, kao što su korisnici s pretplatom na Office 365, korisnik može odabrati da isključi povezana iskustva kojima se analizira sadržaj odlaskom na **Preference** > **Privatnost**.</span><span class="sxs-lookup"><span data-stu-id="8577e-148">For other users, such as home users with an Office 365 subscription, the user can choose to turn off connected experiences that analyze content by going to **Preferences** > **Privacy**.</span></span>

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a><span data-ttu-id="8577e-149">Postavka preferenci za povezana iskustva kojima se preuzima internetski sadržaj</span><span class="sxs-lookup"><span data-stu-id="8577e-149">Policy setting for connected experiences that download online content</span></span>

<span data-ttu-id="8577e-150">Povezana iskustva koja preuzimaju internetski sadržaj iskustva su koja omogućuju pretraživanje i preuzimanje internetskih sadržaja – uključujući predloške, slike, 3D modele, videozapise i referentne materijale – radi poboljšavanja vaših dokumenata.</span><span class="sxs-lookup"><span data-stu-id="8577e-150">Connected experiences that download online content are experiences that allow you to search and download online content including templates, images, 3D models, videos, and reference materials to enhance your documents.</span></span> <span data-ttu-id="8577e-151">Na primjer, predlošci sustava Office ili alat za brz početak rada s programom PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="8577e-151">For example, Office templates or PowerPoint QuickStarter.</span></span> <span data-ttu-id="8577e-152">Popis tih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="8577e-152">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8577e-153">**Preference Domain**</span><span class="sxs-lookup"><span data-stu-id="8577e-153">**Preference Domain**</span></span>  | `com.microsoft.office` |
|<span data-ttu-id="8577e-154">**Tipka**</span><span class="sxs-lookup"><span data-stu-id="8577e-154">**Key**</span></span>  | `OfficeExperiencesDownloadingContentPreference`  |
|<span data-ttu-id="8577e-155">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="8577e-155">**Data Type**</span></span>  | <span data-ttu-id="8577e-156">Booleov</span><span class="sxs-lookup"><span data-stu-id="8577e-156">Boolean</span></span> |
|<span data-ttu-id="8577e-157">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="8577e-157">**Possible values**</span></span>  | <span data-ttu-id="8577e-158">`TRUE` *(omogućeno)*</span><span class="sxs-lookup"><span data-stu-id="8577e-158">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="8577e-159">`FALSE` *(onemogućeno)*</span><span class="sxs-lookup"><span data-stu-id="8577e-159">`FALSE` *(disabled)*</span></span>|
|<span data-ttu-id="8577e-160">**Dostupnost**</span><span class="sxs-lookup"><span data-stu-id="8577e-160">**Availability**</span></span> |<span data-ttu-id="8577e-161">16.28 i novija</span><span class="sxs-lookup"><span data-stu-id="8577e-161">16.28 and later</span></span> |

<span data-ttu-id="8577e-162">Ako ne postavite tu preferencu, povezana iskustva kojima se preuzima internetski sadržaj dostupna su korisnicima.</span><span class="sxs-lookup"><span data-stu-id="8577e-162">If you don't set this preference, connected experiences that download online content are available to users.</span></span>

<span data-ttu-id="8577e-163">Ako korisnik ima pretplatu na Office 365 te se prijavi s pomoću računa poduzeća ili obrazovne ustanove ili ako ima licenciranu verziju sustava Office 2019 za Mac, ne može isključiti povezana iskustva kojima se preuzima internetski sadržaj.</span><span class="sxs-lookup"><span data-stu-id="8577e-163">If the user has an Office 365 subscription and is signed in with a work or school account or if the user has a volume licensed version of Office 2019 for Mac, then the user can't turn off connected experiences that download online content.</span></span>

<span data-ttu-id="8577e-164">Za druge korisnike, kao što su korisnici s pretplatom na Office 365, korisnik može odabrati da isključi povezana iskustva kojima se preuzima internetski sadržaj odlaskom na **Preference** > **Privatnost**.</span><span class="sxs-lookup"><span data-stu-id="8577e-164">For other users, such as home users with an Office 365 subscription, a user can choose to turn off connected experiences that download online content by going to **Preferences** > **Privacy**.</span></span>

## <a name="preference-setting-for-optional-connected-experiences"></a><span data-ttu-id="8577e-165">Postavka preferenci za neobvezna povezana iskustva</span><span class="sxs-lookup"><span data-stu-id="8577e-165">Policy setting for optional connected experiences</span></span>

<span data-ttu-id="8577e-166">Osim prethodno spomenutih povezanih iskustava postoje i neka neobvezna povezana iskustva za koja korisnicima možete omogućiti da im pristupaju upotrebom računa poduzeća ili ustanove, koji se ponekad naziva račun poduzeća ili račun obrazovne ustanove.</span><span class="sxs-lookup"><span data-stu-id="8577e-166">In addition to the connected experiences mentioned above, there are some optional connected experiences that you may choose to allow your users to access with their organization account, which is sometimes referred to as a work or school account.</span></span> <span data-ttu-id="8577e-167">Na primjer, značajke povezane uz LinkedIn u pomoćniku za životopis u programu Word ili Traka vremenske prognoze u programu Outlook, koja se koristi servisom MSN Vrijeme.</span><span class="sxs-lookup"><span data-stu-id="8577e-167">For example, the LinkedIn features of the Resume Assistant in Word or the 3D Maps feature in Excel, which uses Bing.</span></span> <span data-ttu-id="8577e-168">Dodatne primjere potražite u članku [Pregled neobveznih povezanih iskustava za Office](optional-connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="8577e-168">For more examples, see [Overview of optional connected experiences in Office](optional-connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8577e-169">**Preference Domain**</span><span class="sxs-lookup"><span data-stu-id="8577e-169">**Preference Domain**</span></span>  | `com.microsoft.office` |
|<span data-ttu-id="8577e-170">**Tipka**</span><span class="sxs-lookup"><span data-stu-id="8577e-170">**Key**</span></span>  | `OptionalConnectedExperiencesPreference`  |
|<span data-ttu-id="8577e-171">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="8577e-171">**Data Type**</span></span>  | <span data-ttu-id="8577e-172">Booleov</span><span class="sxs-lookup"><span data-stu-id="8577e-172">Boolean</span></span> |
|<span data-ttu-id="8577e-173">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="8577e-173">**Possible values**</span></span>  | <span data-ttu-id="8577e-174">`TRUE` *(omogućeno)*</span><span class="sxs-lookup"><span data-stu-id="8577e-174">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="8577e-175">`FALSE` *(onemogućeno)*</span><span class="sxs-lookup"><span data-stu-id="8577e-175">`FALSE` *(disabled)*</span></span>|
|<span data-ttu-id="8577e-176">**Dostupnost**</span><span class="sxs-lookup"><span data-stu-id="8577e-176">**Availability**</span></span> |<span data-ttu-id="8577e-177">16.28 i novija</span><span class="sxs-lookup"><span data-stu-id="8577e-177">16.28 and later</span></span> |

<span data-ttu-id="8577e-178">Ako ne postavite tu preferencu, neobvezna povezana iskustva dostupna su korisnicima s pretplatom na Office 365 na koji se prijavljuje s pomoću računa poduzeća ili obrazovne ustanove ili korisnicima koji imaju licencirane verzije sustava Office 2019 za Mac.</span><span class="sxs-lookup"><span data-stu-id="8577e-178">If you don't set this preference, optional connected experiences are available to users with an Office 365 subscription that are signed in with a work or school account or users who have a volume licensed version of Office 2019 for Mac.</span></span> <span data-ttu-id="8577e-179">Osim ako niste postavili tu preferencu na `FALSE`, ti korisnici mogu odabrati da isključe neobvezno povezano iskustvo odlaskom na **Preference** > **Privatnost**.</span><span class="sxs-lookup"><span data-stu-id="8577e-179">Unless you have set this preference to `FALSE`, these users can choose to turn off optional connected experiences by going to **Preferences** > **Privacy**.</span></span>

<span data-ttu-id="8577e-180">Za druge korisnike, kao što su privatni korisnici s pretplatom na Office 365, ne postoji opcija isključivanja neobveznih povezanih iskustava.</span><span class="sxs-lookup"><span data-stu-id="8577e-180">For other users, such as home users with an Office 365 subscription, there isn't an option to turn off optional connected experiences.</span></span>

## <a name="preference-setting-for-most-connected-experiences"></a><span data-ttu-id="8577e-181">Postavka preferenci za većinu povezanih iskustava</span><span class="sxs-lookup"><span data-stu-id="8577e-181">Policy setting for most connected experiences</span></span>

<span data-ttu-id="8577e-182">Tu preferencu možete upotrijebiti kako biste kontrolirali je li većina povezanih iskustava dostupna vašim korisnicima.</span><span class="sxs-lookup"><span data-stu-id="8577e-182">You can use this preference to control whether most connected experiences are available to your users.</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8577e-183">**Preference Domain**</span><span class="sxs-lookup"><span data-stu-id="8577e-183">**Preference Domain**</span></span>  | `com.microsoft.office` |
|<span data-ttu-id="8577e-184">**Tipka**</span><span class="sxs-lookup"><span data-stu-id="8577e-184">**Key**</span></span>  | `ConnectedOfficeExperiencesPreference`  |
|<span data-ttu-id="8577e-185">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="8577e-185">**Data Type**</span></span>  | <span data-ttu-id="8577e-186">Booleov</span><span class="sxs-lookup"><span data-stu-id="8577e-186">Boolean</span></span> |
|<span data-ttu-id="8577e-187">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="8577e-187">**Possible values**</span></span>  | <span data-ttu-id="8577e-188">`TRUE` *(omogućeno)*</span><span class="sxs-lookup"><span data-stu-id="8577e-188">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="8577e-189">`FALSE` *(onemogućeno)*</span><span class="sxs-lookup"><span data-stu-id="8577e-189">`FALSE` *(disabled)*</span></span>|
|<span data-ttu-id="8577e-190">**Dostupnost**</span><span class="sxs-lookup"><span data-stu-id="8577e-190">**Availability**</span></span> |<span data-ttu-id="8577e-191">16.28 i novija</span><span class="sxs-lookup"><span data-stu-id="8577e-191">16.28 and later</span></span> |

<span data-ttu-id="8577e-192">Ako ne postavite tu preferencu, sva su povezana iskustva dostupna vašim korisnicima, osim ako ste postavili neku od drugih preferenci za povezana iskustva koja su prethodno navedena, kao na primjer `OfficeExperiencesAnalyzingContentPreference`.</span><span class="sxs-lookup"><span data-stu-id="8577e-192">If you don't set this preference, all connected experiences are available to your users, unless you have set one of the other preferences for connected experiences previously mentioned, such as `OfficeExperiencesAnalyzingContentPreference`.</span></span>

<span data-ttu-id="8577e-193">Na primjer, ako ovu preferencu postavite na `FALSE`, sljedeće vrste povezanih iskustava neće biti dostupne vašim korisnicima:</span><span class="sxs-lookup"><span data-stu-id="8577e-193">For example, if you set this preference to `FALSE`, the following types of connected experiences won't be available to your users:</span></span>
- <span data-ttu-id="8577e-194">iskustva koja analiziraju sadržaj</span><span class="sxs-lookup"><span data-stu-id="8577e-194">Experiences that analyze your content</span></span>
- <span data-ttu-id="8577e-195">iskustva koja preuzimaju internetski sadržaj</span><span class="sxs-lookup"><span data-stu-id="8577e-195">Experiences that download online content</span></span>
- <span data-ttu-id="8577e-196">neobavezna povezana iskustva</span><span class="sxs-lookup"><span data-stu-id="8577e-196">Optional connected experiences</span></span>

<span data-ttu-id="8577e-197">Usto, ako podesite ovu preferencu na `FALSE`, isključuje se i većina drugih povezanih iskustava, kao što su suautorstvo i internetski prostor za pohranu datoteka.</span><span class="sxs-lookup"><span data-stu-id="8577e-197">In addition, if you disable this policy setting, most other connected experiences are also turned off, such as co-authoring and online file storage.</span></span> <span data-ttu-id="8577e-198">Popis tih drugih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="8577e-198">For a list of these other connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

<span data-ttu-id="8577e-199">No čak i ako podesite ovu preferencu na`FALSE`, ostat će dostupna ograničena funkcionalnost sustava Office, kao što je sinkronizacija poštanskog sandučića u programu Outlook, pa će Teams i Skype za tvrtke i dalje funkcionirati.</span><span class="sxs-lookup"><span data-stu-id="8577e-199">But even if you disable this policy setting, limited Office functionality will remain available, such as synching a mailbox in Outlook, and Teams and Skype for Business will continue to work.</span></span> <span data-ttu-id="8577e-200">[Ključni servisi](essential-services.md), poput servisa za licenciranje, kojima se potvrđuje da imate ispravnu licenciju za upotrebu sustava Office, također će ostati dostupni.</span><span class="sxs-lookup"><span data-stu-id="8577e-200">[Essential services](essential-services.md), such as the licensing service that confirms that you’re properly licensed to use Office, will also remain available.</span></span>

<span data-ttu-id="8577e-201">Ako korisnik ima pretplatu na Office 365 te se prijavi s pomoću računa poduzeća ili obrazovne ustanove ili ako ima licenciranu verziju sustava Office 2019 za Mac, ne može isključiti većinu povezanih iskustava.</span><span class="sxs-lookup"><span data-stu-id="8577e-201">If the user has an Office 365 subscription and is signed in with a work or school account or if the user has a volume licensed version of Office 2019 for Mac, then the user can't turn off most connected experiences.</span></span>

<span data-ttu-id="8577e-202">Za druge korisnike, kao što su privatni korisnici s pretplatom na Office 365, korisnik može odabrati da isključi većinu povezanih iskustava odlaskom na **Preference** > **Privatnost**.</span><span class="sxs-lookup"><span data-stu-id="8577e-202">For other users, such as home users with an Office 365 subscription, a user can choose to turn off most connected experiences by going to **Preferences** > **Privacy**.</span></span>

## <a name="preference-setting-for-the-required-data-notice-dialog-for-microsoft-autoupdate"></a><span data-ttu-id="8577e-203">Postavka preferenci u dijalogu potrebne podatkovne obavijesti za Microsoft AutoUpdate</span><span class="sxs-lookup"><span data-stu-id="8577e-203">Preference setting for the Required Data Notice dialog for Microsoft AutoUpdate</span></span>

<span data-ttu-id="8577e-204">Prvi put kada se pokrene verzija 4.12 ili novija programa Microsoft AutoUpdate (MAU), korisnici će vidjeti dijalog **Potrebne podatkovne obavijesti** kojim im se omogućuju informacije o podacima iz MAU-a koji se šalju Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="8577e-204">The first time Version 4.12 or later of Microsoft AutoUpdate (MAU) is launched, users will see a **Required Data Notice** dialog which provides them with information about what data from MAU is sent to Microsoft.</span></span>

<span data-ttu-id="8577e-205">Ako ne želite da korisnici vide dijalog **Potrebne podatkovne obavijesti** za Microsoft AutoUpdate, možete postaviti sljedeću preferencu.</span><span class="sxs-lookup"><span data-stu-id="8577e-205">If you don't want your users to see this **Required Data Notice** dialog for Microsoft AutoUpdate, you can set the following preference.</span></span> <span data-ttu-id="8577e-206">Bez obzira na to koju vrijednost postavite, dijalog se neće prikazati vašim korisnicima.</span><span class="sxs-lookup"><span data-stu-id="8577e-206">Regardless of which value you set, the dialog won't be shown to your users.</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8577e-207">**Preference Domain**</span><span class="sxs-lookup"><span data-stu-id="8577e-207">**Preference Domain**</span></span>  | `com.microsoft.autoupdate2` |
|<span data-ttu-id="8577e-208">**Tipka**</span><span class="sxs-lookup"><span data-stu-id="8577e-208">**Key**</span></span>  | `AcknowledgedDataCollectionPolicy`  |
|<span data-ttu-id="8577e-209">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="8577e-209">**Data Type**</span></span>  | <span data-ttu-id="8577e-210">Niz</span><span class="sxs-lookup"><span data-stu-id="8577e-210">String</span></span> |
|<span data-ttu-id="8577e-211">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="8577e-211">**Possible values**</span></span>  | `RequiredDataOnly` <br/> `RequiredAndOptionalData`|
|<span data-ttu-id="8577e-212">**Dostupnost**</span><span class="sxs-lookup"><span data-stu-id="8577e-212">**Availability**</span></span> |<span data-ttu-id="8577e-213">4.12 i novija</span><span class="sxs-lookup"><span data-stu-id="8577e-213">4.12 and later</span></span> |

<span data-ttu-id="8577e-214">Ako vašim korisnicima dopustite da vide ovaj dijalog, kada korisnik odabere**U redu**, vrijednost`RequiredDataOnly` zapisuje se u `AcknowledgedDataCollectionPolicy` i dijalog se više ne prikazuje korisniku.</span><span class="sxs-lookup"><span data-stu-id="8577e-214">If you let your users see this dialog, then when the user chooses **OK**, the value `RequiredDataOnly` is written to `AcknowledgedDataCollectionPolicy` and the dialog is not shown to the user again.</span></span>


## <a name="related-topics"></a><span data-ttu-id="8577e-215">Povezane teme</span><span class="sxs-lookup"><span data-stu-id="8577e-215">Related topics</span></span>

- [<span data-ttu-id="8577e-216">Referenca za konfiguraciju profila (dokumentacija za Appleove inženjere) </span><span class="sxs-lookup"><span data-stu-id="8577e-216">Configuration Profile Reference (Apple developer documentation)</span></span>](https://go.microsoft.com/fwlink/p/?linkid=852998)
- [<span data-ttu-id="8577e-217">Implementacija preferenci za Office za Mac</span><span class="sxs-lookup"><span data-stu-id="8577e-217">Deploy preferences for Office for Mac</span></span>](../mac/deploy-preferences-for-office-for-mac.md)
- [<span data-ttu-id="8577e-218">Postavke zaštite privatnosti računa</span><span class="sxs-lookup"><span data-stu-id="8577e-218">Account Privacy Settings</span></span>](https://support.office.com/article/3e7bc183-bf52-4fd0-8e6b-78978f7f121b#ID0EAADAAA=Mac)