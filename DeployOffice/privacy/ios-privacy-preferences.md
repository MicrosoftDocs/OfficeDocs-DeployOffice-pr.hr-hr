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
ms.openlocfilehash: ac8b3428734649981f20a82be2f0793c857e09ee
ms.sourcegitcommit: 81295dff0f2fa474f0db39fd40560e3a23fff32a
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45092146"
---
# <a name="use-preferences-to-manage-privacy-controls-for-office-on-ios-devices"></a><span data-ttu-id="2b36c-103">Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office na iOS uređajima</span><span class="sxs-lookup"><span data-stu-id="2b36c-103">Use preferences to manage privacy controls for Office on iOS devices</span></span>

<span data-ttu-id="2b36c-104">Postoje nove postavke preferenci kojima se omogućuje kontrola nad postavkama povezanima sa sljedećim:</span><span class="sxs-lookup"><span data-stu-id="2b36c-104">There are new preference settings for Office on iOS devices that allow you to control settings related to the following:</span></span>

- <span data-ttu-id="2b36c-105">***Dijagnostički podaci*** koji se prikupljaju i šalju Microsoftu o klijentskom softveru sustava Office koji se upotrebljava.</span><span class="sxs-lookup"><span data-stu-id="2b36c-105">***Diagnostic data*** that is collected and sent to Microsoft about Office client software being used.</span></span>

- <span data-ttu-id="2b36c-106">***Povezana iskustva*** koja se koriste funkcijom utemeljenoj na oblaku da bi vama i vašim korisnicima ponudila poboljšane značajke sustava Office.</span><span class="sxs-lookup"><span data-stu-id="2b36c-106">***Connected experiences*** that use cloud-based functionality to provide enhanced Office features to you and your users.</span></span>

<span data-ttu-id="2b36c-107">Dodatne informacije o dijagnostičkim podacima i povezanim iskustvima potražite u članku [Pregled kontrola zaštite privatnosti](overview-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="2b36c-107">For more information about diagnostic data and connected experiences, see [Overview of privacy controls](overview-privacy-controls.md).</span></span>

<span data-ttu-id="2b36c-108">Te preference postavki odnose se na sljedeće aplikacije:</span><span class="sxs-lookup"><span data-stu-id="2b36c-108">These preference settings apply to the following applications:</span></span>
- <span data-ttu-id="2b36c-109">Verzija 2.30 i novije aplikacije Word za iOS, Excel za iOS i PowerPoint za iOS.</span><span class="sxs-lookup"><span data-stu-id="2b36c-109">Version 2.30 and later of Word for iOS, Excel for iOS, and PowerPoint for iOS.</span></span>
- <span data-ttu-id="2b36c-110">Verzija 4.30.0 i novije aplikacije Outlook za iOS</span><span class="sxs-lookup"><span data-stu-id="2b36c-110">Version 4.30.0 and later of Outlook for iOS</span></span>
- <span data-ttu-id="2b36c-111">Verzija 16.30 i novije aplikacije OneNote za iOS.</span><span class="sxs-lookup"><span data-stu-id="2b36c-111">Version 16.30 and later of OneNote for iOS.</span></span>
- <span data-ttu-id="2b36c-112">Verzija 11.19.11 i novije aplikacije OneDrive za iOS.</span><span class="sxs-lookup"><span data-stu-id="2b36c-112">Version 11.19.11 and later of OneDrive for iOS.</span></span>
- <span data-ttu-id="2b36c-113">Verzija 1.17 i novije programa Preglednik za Visio za iOS.</span><span class="sxs-lookup"><span data-stu-id="2b36c-113">Version 1.17 and later of Visio Viewer for iOS.</span></span>
- <span data-ttu-id="2b36c-114">Verzija 2.34 i novija aplikacije Office za iOS.</span><span class="sxs-lookup"><span data-stu-id="2b36c-114">Version 2.34 and later of the Office app for iOS.</span></span>

> [!NOTE]
> <span data-ttu-id="2b36c-115">Informacije o sličnim postavkama za Office na računalima sa sustavom macOS potražite u odjeljku [Upotreba postavki za upravljanje kontrolama za zaštitu privatnosti za Office za Mac](mac-privacy-preferences.md)</span><span class="sxs-lookup"><span data-stu-id="2b36c-115">For information about similar settings for Office on computers running macOS, see [Use preferences to manage privacy controls for Office for Mac](mac-privacy-preferences.md)</span></span>


## <a name="setting-device-preferences"></a><span data-ttu-id="2b36c-116">Postavljanje preferenci uređaja</span><span class="sxs-lookup"><span data-stu-id="2b36c-116">Setting device preferences</span></span>
<span data-ttu-id="2b36c-117">Ove nove preference postavki također se mogu postaviti na razini uređaja putem poslužitelja za upravljanje mobilnim uređajima (MDM) kada je instaliran program Office.</span><span class="sxs-lookup"><span data-stu-id="2b36c-117">These new preference settings can also be set at the device level by a Mobile Device Management (MDM) server when the Office application is installed.</span></span> <span data-ttu-id="2b36c-118">Mnogi MDM poslužitelji omogućuju IT administratorima da dodaju neobavezni konfiguracijski rječnik kada poslužitelj pošalje `InstallApplication` MDM naredbu na iOS uređaj.</span><span class="sxs-lookup"><span data-stu-id="2b36c-118">Many MDM servers allow IT administrators to add an optional configuration dictionary when the server sends the `InstallApplication` MDM command to an iOS device.</span></span> <span data-ttu-id="2b36c-119">Pojedinosti potražite u dokumentaciji vašeg MDM poslužitelja.</span><span class="sxs-lookup"><span data-stu-id="2b36c-119">Refer to your MDM server documentation for more details.</span></span>

<span data-ttu-id="2b36c-120">Rječnik je predstavljen kao skup parova ključeva/vrijednosti u XML obliku.</span><span class="sxs-lookup"><span data-stu-id="2b36c-120">The dictionary is represented as a set of key/value pairs in XML format.</span></span> <span data-ttu-id="2b36c-121">Na primjer:</span><span class="sxs-lookup"><span data-stu-id="2b36c-121">For example:</span></span>

```xml
<dict>
    <key>DiagnosticDataTypePreference</key>
    <string>BasicDiagnosticData</string>
</dict>
```

<span data-ttu-id="2b36c-122">Nakon slanja na uređaj, konfiguracijski rječnik nalazit će se pod `com.apple.managed.configuration` ključem, gdje će se čitati kada se pokrene aplikacija Office.</span><span class="sxs-lookup"><span data-stu-id="2b36c-122">Once sent to the device, the configuration dictionary will reside under the `com.apple.managed.configuration` key, where it will be read when the Office application is launched.</span></span>

> [!NOTE]
> <span data-ttu-id="2b36c-123">Također možete koristiti servis za pravilnike u oblaku sustava Office i sljedeće četiri postavke pravilnika:</span><span class="sxs-lookup"><span data-stu-id="2b36c-123">You can also use the Office cloud policy service and these 4 policy settings:</span></span>
> - <span data-ttu-id="2b36c-124">Konfiguriranje razine dijagnostičkih podataka o klijentskom softveru koje Office šalje Microsoftu</span><span class="sxs-lookup"><span data-stu-id="2b36c-124">Configure the level of client software diagnostic data sent by Office to Microsoft</span></span>
> - <span data-ttu-id="2b36c-125">dopusti korištenje povezanih iskustava koja analiziraju sadržaj u sustavu Office </span><span class="sxs-lookup"><span data-stu-id="2b36c-125">Allow the use of connected experiences in Office that analyze content</span></span>
> - <span data-ttu-id="2b36c-126">dopusti korištenje povezanih iskustava koja preuzimaju internetski sadržaj u sustavu Office </span><span class="sxs-lookup"><span data-stu-id="2b36c-126">Allow the use of connected experiences in Office that download online content</span></span>
> - <span data-ttu-id="2b36c-127">Dopusti korištenje dodatnih neobaveznih povezanih iskustava u sustavu Office</span><span class="sxs-lookup"><span data-stu-id="2b36c-127">Allow the use of additional optional connected experiences in Office</span></span>
>
> <span data-ttu-id="2b36c-128">Postavke zaštite privatnosti za Outlook za iOS i OneDrive za iOS mogu se konfigurirati samo pomoću servisa za pravilnike u oblaku sustava Office.</span><span class="sxs-lookup"><span data-stu-id="2b36c-128">Privacy settings for Outlook for iOS and OneDrive for iOS can only be configured by using the Office cloud policy service.</span></span>
>
> <span data-ttu-id="2b36c-129">Dodatne informacije o upotrebi servisa za pravilnike u oblaku sustava Office potražite u članku [Pregled servisa pravilnika u oblaku sustava Office](../overview-office-cloud-policy-service.md).</span><span class="sxs-lookup"><span data-stu-id="2b36c-129">For more information on using the Office cloud policy service, see [Overview of the Office cloud policy service](../overview-office-cloud-policy-service.md).</span></span>

## <a name="preference-setting-for-diagnostic-data"></a><span data-ttu-id="2b36c-130">Postavka preferenci za dijagnostičke podatke</span><span class="sxs-lookup"><span data-stu-id="2b36c-130">Preference setting for diagnostic data</span></span>

<span data-ttu-id="2b36c-131">Dijagnostički podaci koriste se da bi Office uvijek bio siguran i ažuran, kao i radi otkrivanja, dijagnosticiranja i otklanjanja problema te poboljšavanja proizvoda.</span><span class="sxs-lookup"><span data-stu-id="2b36c-131">Diagnostic data is used to keep Office secure and up-to-date, detect, diagnose and remediate problems, and also make product improvements.</span></span> <span data-ttu-id="2b36c-132">Dodatne informacije potražite u članku [Dijagnostički podaci koje Microsoft 365 Apps za velike tvrtke šalje Microsoftu](overview-privacy-controls.md#diagnostic-data-sent-from-microsoft-365-apps-for-enterprise-to-microsoft).</span><span class="sxs-lookup"><span data-stu-id="2b36c-132">For more information, see [Diagnostic data sent from Microsoft 365 Apps for enterprise to Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-microsoft-365-apps-for-enterprise-to-microsoft).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b36c-133">**Ključ**</span><span class="sxs-lookup"><span data-stu-id="2b36c-133">**Key**</span></span>  | `DiagnosticDataTypePreference`  |
|<span data-ttu-id="2b36c-134">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="2b36c-134">**Data Type**</span></span>  | <span data-ttu-id="2b36c-135">Niz</span><span class="sxs-lookup"><span data-stu-id="2b36c-135">String</span></span> |
|<span data-ttu-id="2b36c-136">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="2b36c-136">**Possible values**</span></span>  | <span data-ttu-id="2b36c-137">`BasicDiagnosticData` *(time se razina postavlja na Obvezno)*</span><span class="sxs-lookup"><span data-stu-id="2b36c-137">`BasicDiagnosticData` *(this sets the level to Required)*</span></span> <br/> <span data-ttu-id="2b36c-138">`FullDiagnosticData` *(time se razina postavlja na Neobvezno)*</span><span class="sxs-lookup"><span data-stu-id="2b36c-138">`FullDiagnosticData` *(this sets the level to Optional)*</span></span> <br/> <span data-ttu-id="2b36c-139">`ZeroDiagnosticData` *(time se razina postavlja na Nijedno)*</span><span class="sxs-lookup"><span data-stu-id="2b36c-139">`ZeroDiagnosticData` *(this sets the level to Neither)*</span></span> |

<span data-ttu-id="2b36c-140">Ako ne postavite tu preferencu, Microsoftu se šalju samo obvezni dijagnostički podaci ako su korisnici s pretplatom na Office 365 (ili Microsoft 365) prijavljeni pomoću računa poduzeća ili obrazovne ustanove.</span><span class="sxs-lookup"><span data-stu-id="2b36c-140">If you don't set this preference, only required diagnostic data is sent to Microsoft if users with an Office 365 (or Microsoft 365) subscription are signed in with a work or school account.</span></span> <span data-ttu-id="2b36c-141">Osim toga, ti korisnici ne mogu promijeniti razinu dijagnostičkih podataka bez obzira na to kako postavite tu preferencu.</span><span class="sxs-lookup"><span data-stu-id="2b36c-141">Also, these users can't change the level of diagnostic data regardless of how you set this preference.</span></span>

<span data-ttu-id="2b36c-142">Drugim korisnicima, kao što su privatni korisnici s pretplatom na Office 365 (ili Microsoft 365), šalju se samo obavezni dijagnostički podaci, osim ako korisnik odabere da šalje i neobavezne dijagnostičke podatke odlaskom na **Postavke** > **Postavke privatnosti**.</span><span class="sxs-lookup"><span data-stu-id="2b36c-142">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, only required diagnostic data is sent, unless the user chooses to also send optional diagnostic data by going to **Settings** > **Privacy Settings**.</span></span>


## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a><span data-ttu-id="2b36c-143">Postavka preferenci za povezana iskustva kojima se analizira vaš sadržaj</span><span class="sxs-lookup"><span data-stu-id="2b36c-143">Preference setting for connected experiences that analyze your content</span></span>

<span data-ttu-id="2b36c-144">Povezana iskustva koja analiziraju vaš sadržaj iskustva su koja koriste vaš sadržaj iz sustava Office da bi vam ponudila preporuke dizajna, prijedloge za uređivanje, uvide u podatke i slične značajke.</span><span class="sxs-lookup"><span data-stu-id="2b36c-144">Connected experiences that analyze your content are experiences that use your Office content to provide you with design recommendations, editing suggestions, data insights, and similar features.</span></span> <span data-ttu-id="2b36c-145">Na primjer, Ideje za dizajn u programu PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="2b36c-145">For example, Design Ideas in PowerPoint.</span></span> <span data-ttu-id="2b36c-146">Popis tih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="2b36c-146">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b36c-147">**Ključ**</span><span class="sxs-lookup"><span data-stu-id="2b36c-147">**Key**</span></span>  | `OfficeExperiencesAnalyzingContentPreference`  |
|<span data-ttu-id="2b36c-148">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="2b36c-148">**Data Type**</span></span>  | <span data-ttu-id="2b36c-149">Booleov</span><span class="sxs-lookup"><span data-stu-id="2b36c-149">Boolean</span></span> |
|<span data-ttu-id="2b36c-150">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="2b36c-150">**Possible values**</span></span>  | <span data-ttu-id="2b36c-151">`TRUE` *(omogućeno)*</span><span class="sxs-lookup"><span data-stu-id="2b36c-151">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="2b36c-152">`FALSE` *(onemogućeno)*</span><span class="sxs-lookup"><span data-stu-id="2b36c-152">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="2b36c-153">Ako ne postavite tu preferencu, povezana iskustva kojima se analizira sadržaj dostupna su korisnicima.</span><span class="sxs-lookup"><span data-stu-id="2b36c-153">If you don't set this preference, connected experiences that analyze content are available to users.</span></span>

<span data-ttu-id="2b36c-154">Ako korisnik ima pretplatu na Office 365 (ili Microsoft 365) te se prijavi s pomoću računa poduzeća ili obrazovne ustanove, ne može isključiti povezana iskustva kojima se analizira sadržaj.</span><span class="sxs-lookup"><span data-stu-id="2b36c-154">If the user has an Office 365 (or Microsoft 365) subscription and is signed in with a work or school account, then the user can't turn off connected experiences that analyze content.</span></span>

<span data-ttu-id="2b36c-155">Za druge korisnike, kao što su korisnici s pretplatom na Office 365 (ili Microsoft 365), korisnik može odabrati da isključi povezana iskustva kojima se analizira sadržaj odlaskom na **Postavke** > **Postavke privatnosti**.</span><span class="sxs-lookup"><span data-stu-id="2b36c-155">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, the user can choose to turn off connected experiences that analyze content by going to **Settings** > **Privacy Settings**.</span></span>

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a><span data-ttu-id="2b36c-156">Postavka preferenci za povezana iskustva kojima se preuzima internetski sadržaj</span><span class="sxs-lookup"><span data-stu-id="2b36c-156">Preference setting for connected experiences that download online content</span></span>

<span data-ttu-id="2b36c-157">Povezana iskustva koja preuzimaju internetski sadržaj iskustva su koja omogućuju pretraživanje i preuzimanje internetskih sadržaja – uključujući predloške, slike, videozapise i referentne materijale – radi poboljšavanja vaših dokumenata.</span><span class="sxs-lookup"><span data-stu-id="2b36c-157">Connected experiences that download online content are experiences that allow you to search and download online content including templates, images, videos, and reference materials to enhance your documents.</span></span> <span data-ttu-id="2b36c-158">Na primjer, predlošci sustava Office ili umetanje mrežne ikone.</span><span class="sxs-lookup"><span data-stu-id="2b36c-158">For example, Office templates or inserting an online icon.</span></span> <span data-ttu-id="2b36c-159">Popis tih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="2b36c-159">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b36c-160">**Ključ**</span><span class="sxs-lookup"><span data-stu-id="2b36c-160">**Key**</span></span>  | `OfficeExperiencesDownloadingContentPreference`  |
|<span data-ttu-id="2b36c-161">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="2b36c-161">**Data Type**</span></span>  | <span data-ttu-id="2b36c-162">Booleov</span><span class="sxs-lookup"><span data-stu-id="2b36c-162">Boolean</span></span> |
|<span data-ttu-id="2b36c-163">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="2b36c-163">**Possible values**</span></span>  | <span data-ttu-id="2b36c-164">`TRUE` *(omogućeno)*</span><span class="sxs-lookup"><span data-stu-id="2b36c-164">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="2b36c-165">`FALSE` *(onemogućeno)*</span><span class="sxs-lookup"><span data-stu-id="2b36c-165">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="2b36c-166">Ako ne postavite tu preferencu, povezana iskustva kojima se preuzima internetski sadržaj dostupna su korisnicima.</span><span class="sxs-lookup"><span data-stu-id="2b36c-166">If you don't set this preference, connected experiences that download online content are available to users.</span></span>

<span data-ttu-id="2b36c-167">Ako korisnik ima pretplatu na Office 365 (ili Microsoft 365) te se prijavi s pomoću računa poduzeća ili obrazovne ustanove, ne može isključiti povezana iskustva kojima se preuzima sadržaj na mreži.</span><span class="sxs-lookup"><span data-stu-id="2b36c-167">If the user has an Office 365 (or Microsoft 365) subscription and is signed in with a work or school account, then the user can't turn off connected experiences that download online content.</span></span>

<span data-ttu-id="2b36c-168">Za druge korisnike, kao što su korisnici s pretplatom na Office 365 (ili Microsoft 365), korisnik može odabrati da isključi povezana iskustva kojima se preuzima sadržaj na mreži odlaskom na **Postavke** > **Postavke privatnosti**.</span><span class="sxs-lookup"><span data-stu-id="2b36c-168">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, the user can choose to turn off connected experiences that download online content by going to **Settings** > **Privacy Settings**.</span></span>

## <a name="preference-setting-for-optional-connected-experiences"></a><span data-ttu-id="2b36c-169">Postavka preferenci za neobavezna povezana iskustva</span><span class="sxs-lookup"><span data-stu-id="2b36c-169">Preference setting for optional connected experiences</span></span>

<span data-ttu-id="2b36c-170">Osim prethodno spomenutih povezanih iskustava postoje i neka neobavezna povezana iskustva za koja korisnicima možete omogućiti da im pristupaju upotrebom računa poduzeća ili ustanove, koji se ponekad naziva račun poduzeća ili račun obrazovne ustanove.</span><span class="sxs-lookup"><span data-stu-id="2b36c-170">In addition to the connected experiences mentioned above, there are some optional connected experiences that you may choose to allow your users to access with their organization account, which is sometimes referred to as a work or school account.</span></span> <span data-ttu-id="2b36c-171">Na primjer, dodaci sustava Office koji se preuzimaju putem trgovine sustava Office na vaš uređaj.</span><span class="sxs-lookup"><span data-stu-id="2b36c-171">For example, Office add-ins that are downloaded through the Office Store to your device.</span></span> <span data-ttu-id="2b36c-172">Dodatne primjere potražite u članku [Pregled neobaveznih povezanih iskustava za Office](optional-connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="2b36c-172">For more examples, see [Overview of optional connected experiences in Office](optional-connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b36c-173">**Ključ**</span><span class="sxs-lookup"><span data-stu-id="2b36c-173">**Key**</span></span>  | `OptionalConnectedExperiencesPreference`  |
|<span data-ttu-id="2b36c-174">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="2b36c-174">**Data Type**</span></span>  | <span data-ttu-id="2b36c-175">Booleov</span><span class="sxs-lookup"><span data-stu-id="2b36c-175">Boolean</span></span> |
|<span data-ttu-id="2b36c-176">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="2b36c-176">**Possible values**</span></span>  | <span data-ttu-id="2b36c-177">`TRUE` *(omogućeno)*</span><span class="sxs-lookup"><span data-stu-id="2b36c-177">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="2b36c-178">`FALSE` *(onemogućeno)*</span><span class="sxs-lookup"><span data-stu-id="2b36c-178">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="2b36c-179">Ako ne postavite tu preferencu, neobavezna povezana iskustva dostupna su korisnicima s pretplatom na Office 365 (ili Microsoft 365) na koji se prijavljuje s pomoću računa poduzeća ili obrazovne ustanove.</span><span class="sxs-lookup"><span data-stu-id="2b36c-179">If you don't set this preference, optional connected experiences are available to users with an Office 365 (or Microsoft 365) subscription that are signed in with a work or school account.</span></span> <span data-ttu-id="2b36c-180">Osim ako niste postavili tu preferencu na FALSE, ti korisnici mogu odabrati da isključe neobavezno povezano iskustvo odlaskom na **Postavke** > **Postavke privatnosti**.</span><span class="sxs-lookup"><span data-stu-id="2b36c-180">Unless you have set this preference to FALSE, these users can choose to turn off optional connected experiences by going to **Settings** > **Privacy Settings**.</span></span>

<span data-ttu-id="2b36c-181">Za druge korisnike, kao što su privatni korisnici s pretplatom na Office 365 (ili Microsoft 365), ne postoji opcija isključivanja neobveznih povezanih iskustava.</span><span class="sxs-lookup"><span data-stu-id="2b36c-181">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, there isn't an option to turn off optional connected experiences.</span></span>