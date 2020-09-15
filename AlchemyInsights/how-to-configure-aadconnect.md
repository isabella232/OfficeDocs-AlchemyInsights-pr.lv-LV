---
title: 646 kā konfigurēt AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704496"
---
# <a name="configure-sync-features"></a><span data-ttu-id="19ff5-102">Sinhronizācijas līdzekļu konfigurēšana</span><span class="sxs-lookup"><span data-stu-id="19ff5-102">Configure sync features</span></span>

<span data-ttu-id="19ff5-103">Azure AD Connect ietver vairākus līdzekļus, kas ir iespējoti pēc noklusējuma, vai arī tos var iespējot vēlāk.</span><span class="sxs-lookup"><span data-stu-id="19ff5-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="19ff5-104">Dažiem līdzekļiem ir nepieciešama papildu konfigurācija noteiktās vidēs.</span><span class="sxs-lookup"><span data-stu-id="19ff5-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="19ff5-105">[Filtrēšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) ierobežo objektu sinhronizēšanu ar Azure AD.</span><span class="sxs-lookup"><span data-stu-id="19ff5-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="19ff5-106">Pēc noklusējuma tiek sinhronizēti visi lietotāji, kontaktpersonas, grupas un Windows 10 datora konti.</span><span class="sxs-lookup"><span data-stu-id="19ff5-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="19ff5-107">Varat iekļaut vai izslēgt objektus atkarībā no domēniem, OU vai citiem atribūtiem.</span><span class="sxs-lookup"><span data-stu-id="19ff5-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="19ff5-108">[Paroļu jaukšanas sinhronizācija](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinhronizē paroļu hash no lokālā Active Directory uz Azure AD.</span><span class="sxs-lookup"><span data-stu-id="19ff5-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="19ff5-109">Tas nodrošina paroļu pārvaldību vienā atrašanās vietā, bet to pašu paroli izmanto gan lokālajā, gan mākoņa vidē.</span><span class="sxs-lookup"><span data-stu-id="19ff5-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="19ff5-110">Tā kā Active Directory ir autoritatīvais avots, varat izmantot savas paroļu politikas.</span><span class="sxs-lookup"><span data-stu-id="19ff5-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="19ff5-111">Pašapkalpošanās [paroles atiestatīšana (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) ļauj lietotājiem atiestatīt savas paroles mākonī, vienlaikus pievienojot savu lokālo paroļu politiku.</span><span class="sxs-lookup"><span data-stu-id="19ff5-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="19ff5-112">Izmantojot [ierīces arī atpakaļrakstīšanas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) , Azure AD reģistrētās ierīces tiek atveidotas atpakaļ uz lokālo Active Directory, lai tos varētu izmantot piekļuvei ar ierobežotu piekļuvi.</span><span class="sxs-lookup"><span data-stu-id="19ff5-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="19ff5-113">Ja pēc noklusējuma ir iespējota [nejauša](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) izdzēšana, lai novērstu vairāku vienlaicīgu objektu dzēšanu (vairāk nekā 500 objekti uz sinhronizāciju).</span><span class="sxs-lookup"><span data-stu-id="19ff5-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="19ff5-114">Jūs varat mainīt šo iestatījumu, lai apmierinātu savas organizācijas vajadzības.</span><span class="sxs-lookup"><span data-stu-id="19ff5-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="19ff5-115">[Automātiskā jaunināšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) pēc noklusējuma ir iespējota Express instalācijām un palīdz nodrošināt, ka jūsu Azure AD Connect versija vienmēr ir aktuāla.</span><span class="sxs-lookup"><span data-stu-id="19ff5-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
