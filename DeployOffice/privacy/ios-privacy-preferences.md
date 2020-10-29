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
ms.openlocfilehash: ed24ac934625bba61eac25e764a892d48365c005
ms.sourcegitcommit: 596a0a60394011aafe1119f353ac76f27e1a4d1b
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48794649"
---
# <a name="use-preferences-to-manage-privacy-controls-for-office-on-ios-devices"></a><span data-ttu-id="b6c8c-103">Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office na iOS uređajima</span><span class="sxs-lookup"><span data-stu-id="b6c8c-103">Use preferences to manage privacy controls for Office on iOS devices</span></span>

> [!NOTE]
> <span data-ttu-id="b6c8c-104">Popis proizvoda sustava Office obuhvaćenih ovim informacijama o zaštiti privatnosti potražite u članku [Kontrole za zaštitu privatnosti dostupne za proizvode Office](products-versions-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="b6c8c-104">For a list of Office products covered by this privacy information, see [Privacy controls available for Office products](products-versions-privacy-controls.md).</span></span>

<span data-ttu-id="b6c8c-105">Postoje nove postavke preferenci kojima se omogućuje kontrola nad postavkama povezanima sa sljedećim:</span><span class="sxs-lookup"><span data-stu-id="b6c8c-105">There are new preference settings for Office on iOS devices that allow you to control settings related to the following:</span></span>

- <span data-ttu-id="b6c8c-106">\***Dijagnostički podaci** _ koji se prikupljaju i šalju Microsoftu o klijentskom softveru sustava Office koji se upotrebljava.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-106">\***Diagnostic data** _ that is collected and sent to Microsoft about Office client software being used.</span></span>

- <span data-ttu-id="b6c8c-107">_*_Povezana iskustva_*_ koja koriste funkcije utemeljene na oblaku da bi vama i vašim korisnicima ponudila poboljšane značajke sustava Office.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-107">_*_Connected experiences_*_ that use cloud-based functionality to provide enhanced Office features to you and your users.</span></span>

<span data-ttu-id="b6c8c-108">Dodatne informacije o dijagnostičkim podacima i povezanim iskustvima potražite u članku [Pregled kontrola zaštite privatnosti](overview-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="b6c8c-108">For more information about diagnostic data and connected experiences, see [Overview of privacy controls](overview-privacy-controls.md).</span></span>

> [!NOTE]
> <span data-ttu-id="b6c8c-109">Informacije o sličnim postavkama za Office na računalima sa sustavom macOS potražite u odjeljku [Upotreba postavki za upravljanje kontrolama za zaštitu privatnosti za Office za Mac](mac-privacy-preferences.md)</span><span class="sxs-lookup"><span data-stu-id="b6c8c-109">For information about similar settings for Office on computers running macOS, see [Use preferences to manage privacy controls for Office for Mac](mac-privacy-preferences.md)</span></span>


## <a name="setting-device-preferences"></a><span data-ttu-id="b6c8c-110">Postavljanje preferenci uređaja</span><span class="sxs-lookup"><span data-stu-id="b6c8c-110">Setting device preferences</span></span>
<span data-ttu-id="b6c8c-111">Ove nove preference postavki također se mogu postaviti na razini uređaja putem poslužitelja za upravljanje mobilnim uređajima (MDM) kada je instaliran program Office.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-111">These new preference settings can also be set at the device level by a Mobile Device Management (MDM) server when the Office application is installed.</span></span> <span data-ttu-id="b6c8c-112">Mnogi MDM poslužitelji omogućuju IT administratorima da dodaju neobavezni konfiguracijski rječnik kada poslužitelj pošalje `InstallApplication` MDM naredbu na iOS uređaj.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-112">Many MDM servers allow IT administrators to add an optional configuration dictionary when the server sends the `InstallApplication` MDM command to an iOS device.</span></span> <span data-ttu-id="b6c8c-113">Pojedinosti potražite u dokumentaciji vašeg MDM poslužitelja.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-113">Refer to your MDM server documentation for more details.</span></span>

<span data-ttu-id="b6c8c-114">Rječnik je predstavljen kao skup parova ključeva/vrijednosti u XML obliku.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-114">The dictionary is represented as a set of key/value pairs in XML format.</span></span> <span data-ttu-id="b6c8c-115">Na primjer:</span><span class="sxs-lookup"><span data-stu-id="b6c8c-115">For example:</span></span>

```xml
<dict>
    <key>DiagnosticDataTypePreference</key>
    <string>BasicDiagnosticData</string>
</dict>
```

<span data-ttu-id="b6c8c-116">Nakon slanja na uređaj, konfiguracijski rječnik nalazit će se pod `com.apple.managed.configuration` ključem, gdje će se čitati kada se pokrene aplikacija Office.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-116">Once sent to the device, the configuration dictionary will reside under the `com.apple.managed.configuration` key, where it will be read when the Office application is launched.</span></span>

> [!NOTE]
> <span data-ttu-id="b6c8c-117">Također možete koristiti servis za pravilnike u oblaku sustava Office i sljedeće četiri postavke pravilnika:</span><span class="sxs-lookup"><span data-stu-id="b6c8c-117">You can also use the Office cloud policy service and these 4 policy settings:</span></span>
> - <span data-ttu-id="b6c8c-118">Konfiguriranje razine dijagnostičkih podataka o klijentskom softveru koje Office šalje Microsoftu</span><span class="sxs-lookup"><span data-stu-id="b6c8c-118">Configure the level of client software diagnostic data sent by Office to Microsoft</span></span>
> - <span data-ttu-id="b6c8c-119">dopusti korištenje povezanih iskustava koja analiziraju sadržaj u sustavu Office </span><span class="sxs-lookup"><span data-stu-id="b6c8c-119">Allow the use of connected experiences in Office that analyze content</span></span>
> - <span data-ttu-id="b6c8c-120">dopusti korištenje povezanih iskustava koja preuzimaju internetski sadržaj u sustavu Office </span><span class="sxs-lookup"><span data-stu-id="b6c8c-120">Allow the use of connected experiences in Office that download online content</span></span>
> - <span data-ttu-id="b6c8c-121">Dopusti korištenje dodatnih neobaveznih povezanih iskustava u sustavu Office</span><span class="sxs-lookup"><span data-stu-id="b6c8c-121">Allow the use of additional optional connected experiences in Office</span></span>
>
> <span data-ttu-id="b6c8c-122">Postavke zaštite privatnosti za Outlook za iOS i OneDrive za iOS mogu se konfigurirati samo pomoću servisa za pravilnike u oblaku sustava Office.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-122">Privacy settings for Outlook for iOS and OneDrive for iOS can only be configured by using the Office cloud policy service.</span></span>
>
> <span data-ttu-id="b6c8c-123">Dodatne informacije o upotrebi servisa za pravilnike u oblaku sustava Office potražite u članku [Pregled servisa pravilnika u oblaku sustava Office](../overview-office-cloud-policy-service.md).</span><span class="sxs-lookup"><span data-stu-id="b6c8c-123">For more information on using the Office cloud policy service, see [Overview of the Office cloud policy service](../overview-office-cloud-policy-service.md).</span></span>

## <a name="preference-setting-for-diagnostic-data"></a><span data-ttu-id="b6c8c-124">Postavka preferenci za dijagnostičke podatke</span><span class="sxs-lookup"><span data-stu-id="b6c8c-124">Preference setting for diagnostic data</span></span>

<span data-ttu-id="b6c8c-125">Dijagnostički podaci koriste se da bi Office uvijek bio siguran i ažuran, kao i radi otkrivanja, dijagnosticiranja i otklanjanja problema te poboljšavanja proizvoda.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-125">Diagnostic data is used to keep Office secure and up-to-date, detect, diagnose and remediate problems, and also make product improvements.</span></span> <span data-ttu-id="b6c8c-126">Dodatne informacije potražite u članku [Dijagnostički podaci koje Microsoft 365 Apps za velike tvrtke šalje Microsoftu](overview-privacy-controls.md#diagnostic-data-sent-from-microsoft-365-apps-for-enterprise-to-microsoft).</span><span class="sxs-lookup"><span data-stu-id="b6c8c-126">For more information, see [Diagnostic data sent from Microsoft 365 Apps for enterprise to Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-microsoft-365-apps-for-enterprise-to-microsoft).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6c8c-127">_ *Tipka*\*</span><span class="sxs-lookup"><span data-stu-id="b6c8c-127">_ *Key*\*</span></span>  | `DiagnosticDataTypePreference`  |
|<span data-ttu-id="b6c8c-128">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="b6c8c-128">**Data Type**</span></span>  | <span data-ttu-id="b6c8c-129">Niz</span><span class="sxs-lookup"><span data-stu-id="b6c8c-129">String</span></span> |
|<span data-ttu-id="b6c8c-130">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="b6c8c-130">**Possible values**</span></span>  | <span data-ttu-id="b6c8c-131">`BasicDiagnosticData` *(time se razina postavlja na Obvezno)*</span><span class="sxs-lookup"><span data-stu-id="b6c8c-131">`BasicDiagnosticData` *(this sets the level to Required)*</span></span> <br/> <span data-ttu-id="b6c8c-132">`FullDiagnosticData` *(time se razina postavlja na Neobvezno)*</span><span class="sxs-lookup"><span data-stu-id="b6c8c-132">`FullDiagnosticData` *(this sets the level to Optional)*</span></span> <br/> <span data-ttu-id="b6c8c-133">`ZeroDiagnosticData` *(time se razina postavlja na Nijedno)*</span><span class="sxs-lookup"><span data-stu-id="b6c8c-133">`ZeroDiagnosticData` *(this sets the level to Neither)*</span></span> |

<span data-ttu-id="b6c8c-134">Ako ne postavite tu preferencu, Microsoftu se šalju samo obvezni dijagnostički podaci ako su korisnici s pretplatom na Office 365 (ili Microsoft 365) prijavljeni pomoću računa poduzeća ili obrazovne ustanove.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-134">If you don't set this preference, only required diagnostic data is sent to Microsoft if users with an Office 365 (or Microsoft 365) subscription are signed in with a work or school account.</span></span> <span data-ttu-id="b6c8c-135">Osim toga, ti korisnici ne mogu promijeniti razinu dijagnostičkih podataka bez obzira na to kako postavite tu preferencu.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-135">Also, these users can't change the level of diagnostic data regardless of how you set this preference.</span></span>

<span data-ttu-id="b6c8c-136">Drugim korisnicima, kao što su privatni korisnici s pretplatom na Office 365 (ili Microsoft 365), šalju se samo obavezni dijagnostički podaci, osim ako korisnik odabere da šalje i neobavezne dijagnostičke podatke odlaskom na **Postavke** > **Postavke privatnosti** .</span><span class="sxs-lookup"><span data-stu-id="b6c8c-136">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, only required diagnostic data is sent, unless the user chooses to also send optional diagnostic data by going to **Settings** > **Privacy Settings** .</span></span>


## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a><span data-ttu-id="b6c8c-137">Postavka preferenci za povezana iskustva kojima se analizira vaš sadržaj</span><span class="sxs-lookup"><span data-stu-id="b6c8c-137">Preference setting for connected experiences that analyze your content</span></span>

<span data-ttu-id="b6c8c-138">Povezana iskustva koja analiziraju vaš sadržaj iskustva su koja koriste vaš sadržaj iz sustava Office da bi vam ponudila preporuke dizajna, prijedloge za uređivanje, uvide u podatke i slične značajke.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-138">Connected experiences that analyze your content are experiences that use your Office content to provide you with design recommendations, editing suggestions, data insights, and similar features.</span></span> <span data-ttu-id="b6c8c-139">Na primjer, Ideje za dizajn u programu PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-139">For example, Design Ideas in PowerPoint.</span></span> <span data-ttu-id="b6c8c-140">Popis tih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="b6c8c-140">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6c8c-141">**Ključ**</span><span class="sxs-lookup"><span data-stu-id="b6c8c-141">**Key**</span></span>  | `OfficeExperiencesAnalyzingContentPreference`  |
|<span data-ttu-id="b6c8c-142">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="b6c8c-142">**Data Type**</span></span>  | <span data-ttu-id="b6c8c-143">Booleov</span><span class="sxs-lookup"><span data-stu-id="b6c8c-143">Boolean</span></span> |
|<span data-ttu-id="b6c8c-144">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="b6c8c-144">**Possible values**</span></span>  | <span data-ttu-id="b6c8c-145">`TRUE` *(omogućeno)*</span><span class="sxs-lookup"><span data-stu-id="b6c8c-145">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="b6c8c-146">`FALSE` *(onemogućeno)*</span><span class="sxs-lookup"><span data-stu-id="b6c8c-146">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="b6c8c-147">Ako ne postavite tu preferencu, povezana iskustva kojima se analizira sadržaj dostupna su korisnicima.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-147">If you don't set this preference, connected experiences that analyze content are available to users.</span></span>

<span data-ttu-id="b6c8c-148">Ako korisnik ima pretplatu na Office 365 (ili Microsoft 365) te se prijavi s pomoću računa poduzeća ili obrazovne ustanove, ne može isključiti povezana iskustva kojima se analizira sadržaj.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-148">If the user has an Office 365 (or Microsoft 365) subscription and is signed in with a work or school account, then the user can't turn off connected experiences that analyze content.</span></span>

<span data-ttu-id="b6c8c-149">Za druge korisnike, kao što su korisnici s pretplatom na Office 365 (ili Microsoft 365), korisnik može odabrati da isključi povezana iskustva kojima se analizira sadržaj odlaskom na **Postavke** > **Postavke privatnosti** .</span><span class="sxs-lookup"><span data-stu-id="b6c8c-149">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, the user can choose to turn off connected experiences that analyze content by going to **Settings** > **Privacy Settings** .</span></span>

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a><span data-ttu-id="b6c8c-150">Postavka preferenci za povezana iskustva kojima se preuzima internetski sadržaj</span><span class="sxs-lookup"><span data-stu-id="b6c8c-150">Preference setting for connected experiences that download online content</span></span>

<span data-ttu-id="b6c8c-151">Povezana iskustva koja preuzimaju internetski sadržaj iskustva su koja omogućuju pretraživanje i preuzimanje internetskih sadržaja – uključujući predloške, slike, videozapise i referentne materijale – radi poboljšavanja vaših dokumenata.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-151">Connected experiences that download online content are experiences that allow you to search and download online content including templates, images, videos, and reference materials to enhance your documents.</span></span> <span data-ttu-id="b6c8c-152">Na primjer, predlošci sustava Office ili umetanje mrežne ikone.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-152">For example, Office templates or inserting an online icon.</span></span> <span data-ttu-id="b6c8c-153">Popis tih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="b6c8c-153">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6c8c-154">**Ključ**</span><span class="sxs-lookup"><span data-stu-id="b6c8c-154">**Key**</span></span>  | `OfficeExperiencesDownloadingContentPreference`  |
|<span data-ttu-id="b6c8c-155">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="b6c8c-155">**Data Type**</span></span>  | <span data-ttu-id="b6c8c-156">Booleov</span><span class="sxs-lookup"><span data-stu-id="b6c8c-156">Boolean</span></span> |
|<span data-ttu-id="b6c8c-157">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="b6c8c-157">**Possible values**</span></span>  | <span data-ttu-id="b6c8c-158">`TRUE` *(omogućeno)*</span><span class="sxs-lookup"><span data-stu-id="b6c8c-158">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="b6c8c-159">`FALSE` *(onemogućeno)*</span><span class="sxs-lookup"><span data-stu-id="b6c8c-159">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="b6c8c-160">Ako ne postavite tu preferencu, povezana iskustva kojima se preuzima internetski sadržaj dostupna su korisnicima.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-160">If you don't set this preference, connected experiences that download online content are available to users.</span></span>

<span data-ttu-id="b6c8c-161">Ako korisnik ima pretplatu na Office 365 (ili Microsoft 365) te se prijavi s pomoću računa poduzeća ili obrazovne ustanove, ne može isključiti povezana iskustva kojima se preuzima sadržaj na mreži.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-161">If the user has an Office 365 (or Microsoft 365) subscription and is signed in with a work or school account, then the user can't turn off connected experiences that download online content.</span></span>

<span data-ttu-id="b6c8c-162">Za druge korisnike, kao što su korisnici s pretplatom na Office 365 (ili Microsoft 365), korisnik može odabrati da isključi povezana iskustva kojima se preuzima sadržaj na mreži odlaskom na **Postavke** > **Postavke privatnosti** .</span><span class="sxs-lookup"><span data-stu-id="b6c8c-162">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, the user can choose to turn off connected experiences that download online content by going to **Settings** > **Privacy Settings** .</span></span>

## <a name="preference-setting-for-optional-connected-experiences"></a><span data-ttu-id="b6c8c-163">Postavka preferenci za neobavezna povezana iskustva</span><span class="sxs-lookup"><span data-stu-id="b6c8c-163">Preference setting for optional connected experiences</span></span>

<span data-ttu-id="b6c8c-164">Osim prethodno spomenutih povezanih iskustava postoje i neka neobavezna povezana iskustva za koja korisnicima možete omogućiti da im pristupaju upotrebom računa poduzeća ili ustanove, koji se ponekad naziva račun poduzeća ili račun obrazovne ustanove.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-164">In addition to the connected experiences mentioned above, there are some optional connected experiences that you may choose to allow your users to access with their organization account, which is sometimes referred to as a work or school account.</span></span> <span data-ttu-id="b6c8c-165">Na primjer, dodaci sustava Office koji se preuzimaju putem trgovine sustava Office na vaš uređaj.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-165">For example, Office add-ins that are downloaded through the Office Store to your device.</span></span> <span data-ttu-id="b6c8c-166">Dodatne primjere potražite u članku [Pregled neobaveznih povezanih iskustava za Office](optional-connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="b6c8c-166">For more examples, see [Overview of optional connected experiences in Office](optional-connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6c8c-167">**Ključ**</span><span class="sxs-lookup"><span data-stu-id="b6c8c-167">**Key**</span></span>  | `OptionalConnectedExperiencesPreference`  |
|<span data-ttu-id="b6c8c-168">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="b6c8c-168">**Data Type**</span></span>  | <span data-ttu-id="b6c8c-169">Booleov</span><span class="sxs-lookup"><span data-stu-id="b6c8c-169">Boolean</span></span> |
|<span data-ttu-id="b6c8c-170">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="b6c8c-170">**Possible values**</span></span>  | <span data-ttu-id="b6c8c-171">`TRUE` *(omogućeno)*</span><span class="sxs-lookup"><span data-stu-id="b6c8c-171">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="b6c8c-172">`FALSE` *(onemogućeno)*</span><span class="sxs-lookup"><span data-stu-id="b6c8c-172">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="b6c8c-173">Ako ne postavite tu preferencu, neobavezna povezana iskustva dostupna su korisnicima s pretplatom na Office 365 (ili Microsoft 365) na koji se prijavljuje s pomoću računa poduzeća ili obrazovne ustanove.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-173">If you don't set this preference, optional connected experiences are available to users with an Office 365 (or Microsoft 365) subscription that are signed in with a work or school account.</span></span> <span data-ttu-id="b6c8c-174">Osim ako niste postavili tu preferencu na FALSE, ti korisnici mogu odabrati da isključe neobavezno povezano iskustvo odlaskom na **Postavke** > **Postavke privatnosti** .</span><span class="sxs-lookup"><span data-stu-id="b6c8c-174">Unless you have set this preference to FALSE, these users can choose to turn off optional connected experiences by going to **Settings** > **Privacy Settings** .</span></span>

<span data-ttu-id="b6c8c-175">Za druge korisnike, kao što su privatni korisnici s pretplatom na Office 365 (ili Microsoft 365), ne postoji opcija isključivanja neobveznih povezanih iskustava.</span><span class="sxs-lookup"><span data-stu-id="b6c8c-175">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, there isn't an option to turn off optional connected experiences.</span></span>