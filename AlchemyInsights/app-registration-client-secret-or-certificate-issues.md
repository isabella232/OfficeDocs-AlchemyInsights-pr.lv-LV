---
title: Programmas reģistrācijas klienta slepens vai sertifikātu problēmas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404784"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="96ea6-102">Programmas reģistrācijas klienta slepens vai sertifikātu problēmas</span><span class="sxs-lookup"><span data-stu-id="96ea6-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="96ea6-103">Vai beidzas programmas klienta slepenība?</span><span class="sxs-lookup"><span data-stu-id="96ea6-103">Application client secret expiring?</span></span>

<span data-ttu-id="96ea6-104">Neatkarīgi no tā, kā tika izveidota reģistrēta programma , lietojumprogrammu reģistrācijas portālā izmantojot standarta reģistrācijas procesu, vai arī, ja jūsu nomniekā tika izveidots pakalpojuma pamatsumma, izmantojot lietojumprogrammas piekrišanu, pirms pašreizējā paziņojuma termiņa beigām būs jāizveido jauns klienta noslēpums, kas atjaunināts saistītajā programmas kodā.</span><span class="sxs-lookup"><span data-stu-id="96ea6-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="96ea6-105">Maksimālais derīguma periods ir 2 gadi.</span><span class="sxs-lookup"><span data-stu-id="96ea6-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="96ea6-106">Atgādinot, ka slepenā vērtība ir jāreģistrē, jo tā vairs nebūs redzama pēc programmu reģistrācijas lapas iziešanas portālā.</span><span class="sxs-lookup"><span data-stu-id="96ea6-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="96ea6-107">Papildinformāciju skatiet [rakstā Īsā pamācība: programmas](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) reģistrēšana Microsoft identitātes platformā un Microsoft identitātes platformas labākā [prakse](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span><span class="sxs-lookup"><span data-stu-id="96ea6-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="96ea6-108">Papildinformāciju skatiet [rakstā Azure AD lietojumprogrammas izveide & identitātes izveide portālā — Microsoft identitātes platforma.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)</span><span class="sxs-lookup"><span data-stu-id="96ea6-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
