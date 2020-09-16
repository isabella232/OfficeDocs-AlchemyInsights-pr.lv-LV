---
title: Microsoft 365 lietojumprogrammu labošana nevarēja atrast saistīto ziņojumu ar Office licencēm
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747702"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="1b840-102">Izlabojot Microsoft 365 lietojumprogrammas, tiek parādīts ziņojums "nevar atrast saistīto Office licenci"</span><span class="sxs-lookup"><span data-stu-id="1b840-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="1b840-103">Ja tiek parādīts šis ziņojums, izmēģiniet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="1b840-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="1b840-104">Pārbaudiet savu ugunsmūri, pretvīrusu programmatūru un starpniekservera iestatījumus, lai pārliecinātos, vai tie nebloķē interneta piekļuvi Microsoft 365 programmām.</span><span class="sxs-lookup"><span data-stu-id="1b840-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="1b840-105">Skatiet [Microsoft 365 vietrāžus URL un IP adrešu diapazoni](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="1b840-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="1b840-106">Noņemt un [atkārtoti piešķirt Office licenci](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) attiecīgajā lietotājam.</span><span class="sxs-lookup"><span data-stu-id="1b840-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="1b840-107">Atveriet kādu Office lietojumprogrammu un [izrakstieties](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) no visiem esošajiem lietotāju kontiem.</span><span class="sxs-lookup"><span data-stu-id="1b840-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="1b840-108">Dodieties uz Windows iestatījumi > **konti**  >  **e-pasta & konti**un noņemiet visus darba kontus, izņemot ietekmēto kontu.</span><span class="sxs-lookup"><span data-stu-id="1b840-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="1b840-109">Dodieties uz Windows iestatījumu > **konti**  >  **piekļūstiet darba vai mācību**iestādei un atvienojiet visus darba kontus, izņemot ietekmēto kontu.</span><span class="sxs-lookup"><span data-stu-id="1b840-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="1b840-110">Atiestatiet Office aktivizēšanas stāvokli.</span><span class="sxs-lookup"><span data-stu-id="1b840-110">Reset the Office activation state.</span></span> <span data-ttu-id="1b840-111">[Uzziniet, kā to](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)paveikt.</span><span class="sxs-lookup"><span data-stu-id="1b840-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="1b840-112">[Pierakstieties,](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) izmantojot ietekmēto lietotāja kontu.</span><span class="sxs-lookup"><span data-stu-id="1b840-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="1b840-113">Papildu problēmu novēršanas risinājumus skatiet rakstā [nelicencēts produkts un aktivizācijas kļūdas sistēmā Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="1b840-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>