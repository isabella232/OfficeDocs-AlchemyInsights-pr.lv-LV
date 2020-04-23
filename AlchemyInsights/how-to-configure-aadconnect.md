---
title: 646 kā konfigurēt AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722570"
---
# <a name="configure-sync-features"></a><span data-ttu-id="3c166-102">Sinhronizācijas līdzekļu konfigurēšana</span><span class="sxs-lookup"><span data-stu-id="3c166-102">Configure sync features</span></span>

<span data-ttu-id="3c166-103">Azure AD Connect ietver vairākus līdzekļus, kas ir iespējoti pēc noklusējuma vai kurus var iespējot vēlāk.</span><span class="sxs-lookup"><span data-stu-id="3c166-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="3c166-104">Dažām funkcijām ir nepieciešama papildu konfigurācija konkrētās vidēs.</span><span class="sxs-lookup"><span data-stu-id="3c166-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="3c166-105">[Filtrēšanas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) ierobežojumi objekti tiek SINHRONIZĒTI Azure ad.</span><span class="sxs-lookup"><span data-stu-id="3c166-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="3c166-106">Pēc noklusējuma tiek sinhronizēti visi lietotāji, kontaktpersonas, grupas un Windows 10 datora konti.</span><span class="sxs-lookup"><span data-stu-id="3c166-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="3c166-107">Var iekļaut vai neiekļaut objektus, kuru pamatā ir domēni, OUs vai citi atribūti.</span><span class="sxs-lookup"><span data-stu-id="3c166-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="3c166-108">[Paroļu jaukšanas sinhronizēšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinhronizē paroli hash no lokālā Active Directory Azure ad.</span><span class="sxs-lookup"><span data-stu-id="3c166-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="3c166-109">Tas ļauj pārvaldīt paroli vienā atrašanās vietā, bet izmantot vienu un to pašu paroli gan lokālas, gan mākoņa vidē.</span><span class="sxs-lookup"><span data-stu-id="3c166-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="3c166-110">Tā kā Active Directory ir autoritatīvs avots, varat izmantot savas paroļu politikas.</span><span class="sxs-lookup"><span data-stu-id="3c166-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="3c166-111">[Pašapkalpošanās paroles atiestatīšana (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) ļauj lietotājiem atiestatīt savas paroles mākonī, joprojām lietojot lokālo paroļu politiku.</span><span class="sxs-lookup"><span data-stu-id="3c166-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="3c166-112">[Ierīce arī atpakaļrakstīšanas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) ļauj reģistrētas ierīces Azure ad jāraksta atpakaļ lokālā Active Directory, lai tos var izmantot ierobežotas piekļuves.</span><span class="sxs-lookup"><span data-stu-id="3c166-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="3c166-113">[Novērst nejaušu dzēšanu](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) ir iespējota pēc noklusējuma, lai palīdzētu novērst pārāk daudz vienlaicīgu objektu dzēšanu (vairāk nekā 500 objektus katrā sinhronizācijā).</span><span class="sxs-lookup"><span data-stu-id="3c166-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="3c166-114">Šo iestatījumu var mainīt, lai tas atbilstu jūsu organizācijas vajadzībām.</span><span class="sxs-lookup"><span data-stu-id="3c166-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="3c166-115">[Automātiskā jaunināšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) ir iespējota pēc noklusējuma Express instalācijas un palīdz nodrošināt savu VERSIJU Azure ad savienojumu vienmēr ir spēkā.</span><span class="sxs-lookup"><span data-stu-id="3c166-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
