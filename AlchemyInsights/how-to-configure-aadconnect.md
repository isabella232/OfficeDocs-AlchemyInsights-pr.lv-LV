---
title: 646 kā konfigurēt AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 44b2532c634bf17d87c562f9506cc1e81cc7e84a
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/13/2019
ms.locfileid: "31856663"
---
# <a name="configure-sync-features"></a><span data-ttu-id="cfe36-102">Konfigurēt sinhronizāciju līdzekļus</span><span class="sxs-lookup"><span data-stu-id="cfe36-102">Configure sync features</span></span>

<span data-ttu-id="cfe36-103">Debeszils AD Connect ir iekļauti vairāki līdzekļi, kas ir iespējoti pēc noklusējuma, vai varat aktivizēt vēlāk.</span><span class="sxs-lookup"><span data-stu-id="cfe36-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="cfe36-104">Dažas funkcijas pieprasa papildu konfigurācijas noteiktu vidē.</span><span class="sxs-lookup"><span data-stu-id="cfe36-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="cfe36-105">[Filtrēšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) robežas objekti tiek sinhronizēti ar debeszils reklāmu.</span><span class="sxs-lookup"><span data-stu-id="cfe36-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="cfe36-106">Pēc noklusējuma, visi lietotāji, kontakti, grupas un Windows 10 datoru konti tiek sinhronizēti.</span><span class="sxs-lookup"><span data-stu-id="cfe36-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="cfe36-107">Var iekļaut vai neiekļaut objektus, pamatojoties uz domēniem, OU vai citiem atribūtiem.</span><span class="sxs-lookup"><span data-stu-id="cfe36-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="cfe36-108">[Parole hash sinhronizācijas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinhronizē paroli hash no lokālā Active Directory debeszils reklāmu.</span><span class="sxs-lookup"><span data-stu-id="cfe36-108">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="cfe36-109">Tas ļauj paroles pārvaldība vienā atrašanās vietā, bet izmanto vienu un to pašu paroli abos telpās un mākonis vidēs.</span><span class="sxs-lookup"><span data-stu-id="cfe36-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="cfe36-110">Tā kā Active Directory ir uzticams avots, var izmantot savas paroles politikas.</span><span class="sxs-lookup"><span data-stu-id="cfe36-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="cfe36-111">[Pašapkalpošanās paroles atiestatīšanas (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) ļauj lietotājiem atiestatīt savas paroles mākonis joprojām lietojot lokālā parole politika.</span><span class="sxs-lookup"><span data-stu-id="cfe36-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="cfe36-112">[Writeback ierīce](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) ļauj reģistrētajām ierīcēm debeszils reklāmu rakstīšanu atpakaļ lokālā Active Directory, tāpēc tos var izmantot, lai ierobežotu piekļuvi.</span><span class="sxs-lookup"><span data-stu-id="cfe36-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="cfe36-113">[Novērst nejaušu dzēš](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) pēc noklusējuma ir iespējota, lai nepieļautu, ka pārāk daudz vienlaicīgas objektu dzēšanu (vairāk nekā 500 objekti vienā sinhronizācija).</span><span class="sxs-lookup"><span data-stu-id="cfe36-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="cfe36-114">Jūs varat mainīt šo iestatījumu, lai atbilstu jūsu organizācijas prasībām.</span><span class="sxs-lookup"><span data-stu-id="cfe36-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="cfe36-115">[Automātiska jaunināšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) tiek iespējota pēc noklusējuma izteikt instalācijām un palīdz nodrošināt Azure reklāmas, savienotu jūsu versija vienmēr ir pašreizējā.</span><span class="sxs-lookup"><span data-stu-id="cfe36-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
