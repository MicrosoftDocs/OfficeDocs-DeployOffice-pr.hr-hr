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
# <a name="use-preferences-to-manage-privacy-controls-for-office-on-ios-devices"></a><span data-ttu-id="67c7e-103">Korištenje postavki za upravljanje kontrolama za zaštitu privatnosti za Office na iOS uređajima</span><span class="sxs-lookup"><span data-stu-id="67c7e-103">Use preferences to manage privacy controls for Office on iOS devices</span></span>

<span data-ttu-id="67c7e-104">Postoje nove postavke preferenci kojima se omogućuje kontrola nad postavkama povezanima sa sljedećim:</span><span class="sxs-lookup"><span data-stu-id="67c7e-104">There are new preference settings for Office on iOS devices that allow you to control settings related to the following:</span></span>

- <span data-ttu-id="67c7e-105">***Dijagnostički podaci*** koji se prikupljaju i šalju Microsoftu o klijentskom softveru sustava Office koji se upotrebljava.</span><span class="sxs-lookup"><span data-stu-id="67c7e-105">***Diagnostic data*** that is collected and sent to Microsoft about Office client software being used.</span></span>

- <span data-ttu-id="67c7e-106">***Povezana iskustva*** koja se koriste funkcijom utemeljenoj na oblaku da bi vama i vašim korisnicima ponudila poboljšane značajke sustava Office.</span><span class="sxs-lookup"><span data-stu-id="67c7e-106">***Connected experiences*** that use cloud-based functionality to provide enhanced Office features to you and your users.</span></span>

<span data-ttu-id="67c7e-107">Dodatne informacije o dijagnostičkim podacima i povezanim iskustvima potražite u članku [Pregled kontrola zaštite privatnosti](overview-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="67c7e-107">For more information about diagnostic data and connected experiences, see [Overview of privacy controls](overview-privacy-controls.md).</span></span>

<span data-ttu-id="67c7e-108">Te preference postavki odnose se na sljedeće aplikacije:</span><span class="sxs-lookup"><span data-stu-id="67c7e-108">These preference settings apply to the following applications:</span></span>
- <span data-ttu-id="67c7e-109">Verzija 2.30 i novije aplikacije Word za iOS, Excel za iOS i PowerPoint za iOS.</span><span class="sxs-lookup"><span data-stu-id="67c7e-109">Version 2.30 and later of Word for iOS, Excel for iOS, and PowerPoint for iOS.</span></span>
- <span data-ttu-id="67c7e-110">Verzija 16.30 i novije aplikacije OneNote za iOS.</span><span class="sxs-lookup"><span data-stu-id="67c7e-110">Version 16.30 and later of OneNote for iOS.</span></span>
- <span data-ttu-id="67c7e-111">Verzija 1.17 i novije programa Preglednik za Visio za iOS.</span><span class="sxs-lookup"><span data-stu-id="67c7e-111">Version 1.17 and later of Visio Viewer for iOS.</span></span>

> [!NOTE]
> <span data-ttu-id="67c7e-112">Informacije o sličnim postavkama za Office na računalima sa sustavom macOS potražite u odjeljku [Upotreba postavki za upravljanje kontrolama za zaštitu privatnosti za Office za Mac](mac-privacy-preferences.md)</span><span class="sxs-lookup"><span data-stu-id="67c7e-112">For information about similar settings for Office on computers running Windows, see [Use policy settings to manage privacy controls for Office 365 ProPlus](mac-privacy-preferences.md).</span></span>


## <a name="setting-device-preferences"></a><span data-ttu-id="67c7e-113">Postavljanje preferenci uređaja</span><span class="sxs-lookup"><span data-stu-id="67c7e-113">Setting device preferences</span></span>
<span data-ttu-id="67c7e-114">Ove nove preference postavki također se mogu postaviti na razini uređaja putem poslužitelja za upravljanje mobilnim uređajima (MDM) kada je instaliran program Office.</span><span class="sxs-lookup"><span data-stu-id="67c7e-114">These new preference settings can also be set at the device level by a Mobile Device Management (MDM) server when the Office application is installed.</span></span> <span data-ttu-id="67c7e-115">Mnogi MDM poslužitelji omogućuju IT administratorima da dodaju neobavezni konfiguracijski rječnik kada poslužitelj pošalje `InstallApplication` MDM naredbu na iOS uređaj.</span><span class="sxs-lookup"><span data-stu-id="67c7e-115">Many MDM servers allow IT administrators to add an optional configuration dictionary when the server sends the `InstallApplication` MDM command to an iOS device.</span></span> <span data-ttu-id="67c7e-116">Pojedinosti potražite u dokumentaciji vašeg MDM poslužitelja.</span><span class="sxs-lookup"><span data-stu-id="67c7e-116">Refer to your MDM server documentation for more details.</span></span>

<span data-ttu-id="67c7e-117">Rječnik je predstavljen kao skup parova ključeva/vrijednosti u XML obliku.</span><span class="sxs-lookup"><span data-stu-id="67c7e-117">The dictionary is represented as a set of key/value pairs in XML format.</span></span> <span data-ttu-id="67c7e-118">Na primjer:</span><span class="sxs-lookup"><span data-stu-id="67c7e-118">For example:</span></span>

```xml
<dict>
    <key>DiagnosticDataTypePreference</key>
    <string>BasicDiagnosticData</string>
</dict>
```

<span data-ttu-id="67c7e-119">Nakon slanja na uređaj, konfiguracijski rječnik nalazit će se pod `com.apple.managed.configuration` ključem, gdje će se čitati kada se pokrene aplikacija Office.</span><span class="sxs-lookup"><span data-stu-id="67c7e-119">Once sent to the device, the configuration dictionary will reside under the `com.apple.managed.configuration` key, where it will be read when the Office application is launched.</span></span>

## <a name="preference-setting-for-diagnostic-data"></a><span data-ttu-id="67c7e-120">Postavka preferenci za dijagnostičke podatke</span><span class="sxs-lookup"><span data-stu-id="67c7e-120">Preference setting for diagnostic data</span></span>

<span data-ttu-id="67c7e-121">Dijagnostički se podaci upotrebljavaju da bi Office uvijek bio siguran i ažuran, kao i radi otkrivanja, dijagnosticiranja i otklanjanja problema te poboljšavanja proizvoda.</span><span class="sxs-lookup"><span data-stu-id="67c7e-121">Diagnostic data is used to keep Office secure and up-to-date, detect, diagnose and remediate problems, and also make product improvements.</span></span> <span data-ttu-id="67c7e-122">Za više informacija pogledajte [Dijagnostički podaci koje Office 365 ProPlus šalje Microsoftu](overview-privacy-controls.md#diagnostic-data-sent-from-office-365-proplus-to-microsoft).</span><span class="sxs-lookup"><span data-stu-id="67c7e-122">For more information, see [Diagnostic data sent from Office 365 ProPlus to Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-office-365-proplus-to-microsoft).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="67c7e-123">**Ključ**</span><span class="sxs-lookup"><span data-stu-id="67c7e-123">**Key**</span></span>  | `DiagnosticDataTypePreference`  |
|<span data-ttu-id="67c7e-124">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="67c7e-124">**Data Type**</span></span>  | <span data-ttu-id="67c7e-125">Niz</span><span class="sxs-lookup"><span data-stu-id="67c7e-125">String</span></span> |
|<span data-ttu-id="67c7e-126">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="67c7e-126">**Possible values**</span></span>  | <span data-ttu-id="67c7e-127">`BasicDiagnosticData` *(time se razina postavlja na Obvezno)*</span><span class="sxs-lookup"><span data-stu-id="67c7e-127">`BasicDiagnosticData` *(this sets the level to Required)*</span></span> <br/> <span data-ttu-id="67c7e-128">`FullDiagnosticData` *(time se razina postavlja na Neobvezno)*</span><span class="sxs-lookup"><span data-stu-id="67c7e-128">`FullDiagnosticData` *(this sets the level to Optional)*</span></span> <br/> <span data-ttu-id="67c7e-129">`ZeroDiagnosticData` *(time se razina postavlja na Nijedno)*</span><span class="sxs-lookup"><span data-stu-id="67c7e-129">`ZeroDiagnosticData` *(this sets the level to Neither)*</span></span> |

<span data-ttu-id="67c7e-130">Ako ne postavite tu preferencu, Microsoftu se šalju samo obvezni dijagnostički podaci ako su korisnici s pretplatom na Office 365 prijavljeni pomoću računa poduzeća ili obrazovne ustanove.</span><span class="sxs-lookup"><span data-stu-id="67c7e-130">Starting with new installations of Version 16.30, if you don't set this preference, only required diagnostic data is sent to Microsoft if users with an Office 365 subscription are signed in with a work or school account or if users have a volume licensed version of Office 2019 for Mac.</span></span> <span data-ttu-id="67c7e-131">Osim toga, ti korisnici ne mogu promijeniti razinu dijagnostičkih podataka bez obzira na to kako postavite tu preferencu.</span><span class="sxs-lookup"><span data-stu-id="67c7e-131">Also, these users can't change the level of diagnostic data regardless of how you set this preference.</span></span>

<span data-ttu-id="67c7e-132">Drugim korisnicima, kao što su privatni korisnici s pretplatom na Office 365, šalju se samo obavezni dijagnostički podaci, osim ako korisnik odabere da šalje i neobavezne dijagnostičke podatke odlaskom na **Postavke** > **Postavke privatnosti**.</span><span class="sxs-lookup"><span data-stu-id="67c7e-132">For other users, such as home users with an Office 365 subscription, only required diagnostic data is sent, unless the user chooses to also send optional diagnostic data by going to **Preferences** > **Privacy**.</span></span>


## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a><span data-ttu-id="67c7e-133">Postavka preferenci za povezana iskustva kojima se analizira vaš sadržaj</span><span class="sxs-lookup"><span data-stu-id="67c7e-133">Preference setting for connected experiences that analyze your content</span></span>

<span data-ttu-id="67c7e-134">Povezana iskustva koja analiziraju vaš sadržaj iskustva su koja koriste vaš sadržaj iz sustava Office da bi vam ponudila preporuke dizajna, prijedloge za uređivanje, uvide u podatke i slične značajke.</span><span class="sxs-lookup"><span data-stu-id="67c7e-134">Connected experiences that analyze your content are experiences that use your Office content to provide you with design recommendations, editing suggestions, data insights, and similar features.</span></span> <span data-ttu-id="67c7e-135">Na primjer, Ideje za dizajn u programu PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="67c7e-135">For example, Design Ideas in PowerPoint.</span></span> <span data-ttu-id="67c7e-136">Popis tih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="67c7e-136">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="67c7e-137">**Ključ**</span><span class="sxs-lookup"><span data-stu-id="67c7e-137">**Key**</span></span>  | `OfficeExperiencesAnalyzingContentPreference`  |
|<span data-ttu-id="67c7e-138">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="67c7e-138">**Data Type**</span></span>  | <span data-ttu-id="67c7e-139">Booleov</span><span class="sxs-lookup"><span data-stu-id="67c7e-139">Boolean</span></span> |
|<span data-ttu-id="67c7e-140">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="67c7e-140">**Possible values**</span></span>  | <span data-ttu-id="67c7e-141">`TRUE` *(omogućeno)*</span><span class="sxs-lookup"><span data-stu-id="67c7e-141">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="67c7e-142">`FALSE` *(onemogućeno)*</span><span class="sxs-lookup"><span data-stu-id="67c7e-142">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="67c7e-143">Ako ne postavite tu preferencu, povezana iskustva kojima se analizira sadržaj dostupna su korisnicima.</span><span class="sxs-lookup"><span data-stu-id="67c7e-143">If you don't set this preference, connected experiences that analyze content are available to users.</span></span>

<span data-ttu-id="67c7e-144">Ako korisnik ima pretplatu na Office 365 te se prijavi s pomoću računa poduzeća ili obrazovne ustanove, ne može isključiti povezana iskustva kojima se analizira sadržaj.</span><span class="sxs-lookup"><span data-stu-id="67c7e-144">If the user has an Office 365 subscription and is signed in with a work or school account or if the user has a volume licensed version of Office 2019 for Mac, then the user can't turn off connected experiences that analyze content.</span></span>

<span data-ttu-id="67c7e-145">Za druge korisnike, kao što su korisnici s pretplatom na Office 365, korisnik može odabrati da isključi povezana iskustva kojima se analizira sadržaj odlaskom na **Postavke** > **Postavke privatnosti**.</span><span class="sxs-lookup"><span data-stu-id="67c7e-145">For other users, such as home users with an Office 365 subscription, the user can choose to turn off connected experiences that analyze content by going to **Preferences** > **Privacy**.</span></span>

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a><span data-ttu-id="67c7e-146">Postavka preferenci za povezana iskustva kojima se preuzima internetski sadržaj</span><span class="sxs-lookup"><span data-stu-id="67c7e-146">Preference setting for connected experiences that download online content</span></span>

<span data-ttu-id="67c7e-147">Povezana iskustva koja preuzimaju internetski sadržaj iskustva su koja omogućuju pretraživanje i preuzimanje internetskih sadržaja – uključujući predloške, slike, videozapise i referentne materijale – radi poboljšavanja vaših dokumenata.</span><span class="sxs-lookup"><span data-stu-id="67c7e-147">Connected experiences that download online content are experiences that allow you to search and download online content including templates, images, 3D models, videos, and reference materials to enhance your documents.</span></span> <span data-ttu-id="67c7e-148">Na primjer, predlošci sustava Office ili umetanje mrežne ikone.</span><span class="sxs-lookup"><span data-stu-id="67c7e-148">For example, Office templates or inserting an online icon.</span></span> <span data-ttu-id="67c7e-149">Popis tih povezanih iskustava potražite u članku [Povezana iskustva u sustavu Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="67c7e-149">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="67c7e-150">**Ključ**</span><span class="sxs-lookup"><span data-stu-id="67c7e-150">**Key**</span></span>  | `OfficeExperiencesDownloadingContentPreference`  |
|<span data-ttu-id="67c7e-151">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="67c7e-151">**Data Type**</span></span>  | <span data-ttu-id="67c7e-152">Booleov</span><span class="sxs-lookup"><span data-stu-id="67c7e-152">Boolean</span></span> |
|<span data-ttu-id="67c7e-153">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="67c7e-153">**Possible values**</span></span>  | <span data-ttu-id="67c7e-154">`TRUE` *(omogućeno)*</span><span class="sxs-lookup"><span data-stu-id="67c7e-154">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="67c7e-155">`FALSE` *(onemogućeno)*</span><span class="sxs-lookup"><span data-stu-id="67c7e-155">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="67c7e-156">Ako ne postavite tu preferencu, povezana iskustva kojima se preuzima internetski sadržaj dostupna su korisnicima.</span><span class="sxs-lookup"><span data-stu-id="67c7e-156">If you don't set this preference, connected experiences that download online content are available to users.</span></span>

<span data-ttu-id="67c7e-157">Ako korisnik ima pretplatu na Office 365 te se prijavi s pomoću računa poduzeća ili obrazovne ustanove, ne može isključiti povezana iskustva kojima se preuzima internetski sadržaj.</span><span class="sxs-lookup"><span data-stu-id="67c7e-157">If the user has an Office 365 subscription and is signed in with a work or school account or if the user has a volume licensed version of Office 2019 for Mac, then the user can't turn off connected experiences that download online content.</span></span>

<span data-ttu-id="67c7e-158">Za druge korisnike, kao što su korisnici s pretplatom na Office 365, korisnik može odabrati da isključi povezana iskustva kojima se preuzima internetski sadržaj odlaskom na **Postavke** > **Postavke privatnosti**.</span><span class="sxs-lookup"><span data-stu-id="67c7e-158">For other users, such as home users with an Office 365 subscription, a user can choose to turn off connected experiences that download online content by going to **Preferences** > **Privacy**.</span></span>

## <a name="preference-setting-for-optional-connected-experiences"></a><span data-ttu-id="67c7e-159">Postavka preferenci za neobavezna povezana iskustva</span><span class="sxs-lookup"><span data-stu-id="67c7e-159">Preference setting for optional connected experiences</span></span>

<span data-ttu-id="67c7e-160">Osim prethodno spomenutih povezanih iskustava postoje i neka neobavezna povezana iskustva za koja korisnicima možete omogućiti da im pristupaju upotrebom računa poduzeća ili ustanove, koji se ponekad naziva račun poduzeća ili račun obrazovne ustanove.</span><span class="sxs-lookup"><span data-stu-id="67c7e-160">In addition to the connected experiences mentioned above, there are some optional connected experiences that you may choose to allow your users to access with their organization account, which is sometimes referred to as a work or school account.</span></span> <span data-ttu-id="67c7e-161">Na primjer, dodaci sustava Office koji se preuzimaju putem trgovine sustava Office na vaš uređaj.</span><span class="sxs-lookup"><span data-stu-id="67c7e-161">For example, Office add-ins that are downloaded through the Office Store to your device.</span></span> <span data-ttu-id="67c7e-162">Dodatne primjere potražite u članku [Pregled neobaveznih povezanih iskustava za Office](optional-connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="67c7e-162">For more examples, see [Overview of optional connected experiences in Office](optional-connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="67c7e-163">**Ključ**</span><span class="sxs-lookup"><span data-stu-id="67c7e-163">**Key**</span></span>  | `OptionalConnectedExperiencesPreference`  |
|<span data-ttu-id="67c7e-164">**Vrsta podataka**</span><span class="sxs-lookup"><span data-stu-id="67c7e-164">**Data Type**</span></span>  | <span data-ttu-id="67c7e-165">Booleov</span><span class="sxs-lookup"><span data-stu-id="67c7e-165">Boolean</span></span> |
|<span data-ttu-id="67c7e-166">**Moguće vrijednosti**</span><span class="sxs-lookup"><span data-stu-id="67c7e-166">**Possible values**</span></span>  | <span data-ttu-id="67c7e-167">`TRUE` *(omogućeno)*</span><span class="sxs-lookup"><span data-stu-id="67c7e-167">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="67c7e-168">`FALSE` *(onemogućeno)*</span><span class="sxs-lookup"><span data-stu-id="67c7e-168">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="67c7e-169">Ako ne postavite tu preferencu, neobavezna povezana iskustva dostupna su korisnicima s pretplatom na Office 365 na koji se prijavljuje s pomoću računa poduzeća ili obrazovne ustanove.</span><span class="sxs-lookup"><span data-stu-id="67c7e-169">If you don't set this preference, optional connected experiences are available to users with an Office 365 subscription that are signed in with a work or school account or users who have a volume licensed version of Office 2019 for Mac.</span></span> <span data-ttu-id="67c7e-170">Osim ako niste postavili tu preferencu na FALSE, ti korisnici mogu odabrati da isključe neobavezno povezano iskustvo odlaskom na **Postavke** > **Postavke privatnosti**.</span><span class="sxs-lookup"><span data-stu-id="67c7e-170">Unless you have set this preference to , these users can choose to turn off optional connected experiences by going to Preferences  Privacy.</span></span>

<span data-ttu-id="67c7e-171">Za druge korisnike, kao što su privatni korisnici s pretplatom na Office 365, ne postoji opcija isključivanja neobaveznih povezanih iskustava.</span><span class="sxs-lookup"><span data-stu-id="67c7e-171">For other users, such as home users with an Office 365 subscription, there isn't an option to turn off optional connected experiences.</span></span>