---
title: OneDrive pieteikšanās kļūdas AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982482"
---
# <a name="onedrive-login-error-aadsts50011"></a><span data-ttu-id="8c1b9-102">OneDrive pieteikšanās kļūdas AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="8c1b9-102">OneDrive login error AADSTS50011</span></span>

<span data-ttu-id="8c1b9-103">Ja saņemat kļūdas ziņojumu "AADSTS50011: pieprasījumā norādītais atbildes vietrādis URL neatbilst atbildei", kad pierakstāties lietojumprogrammā OneDrive, pārbaudiet, vai:</span><span class="sxs-lookup"><span data-stu-id="8c1b9-103">If you receive an error "AADSTS50011: The reply URL specified in the request does not match the reply" when signing into the OneDrive app, check for the following:</span></span>

<span data-ttu-id="8c1b9-104">Jūsu OneDrive versijai ir jābūt vienādai vai lielākai par versiju 20.052. XXXX. XXXX.</span><span class="sxs-lookup"><span data-stu-id="8c1b9-104">Your OneDrive version needs to be equal to or greater than version 20.052.XXXX.XXXX.</span></span> <span data-ttu-id="8c1b9-105">Lai pārbaudītu savu versiju, paziņojumu apgabalā noklikšķiniet uz zilās OneDrive ikonas, atlasiet **palīdzības & iestatījumi > iestatījumi > par**.</span><span class="sxs-lookup"><span data-stu-id="8c1b9-105">To check your version, click on the blue OneDrive icon in the notification area, select **Help & Settings > Settings > About**.</span></span>

<span data-ttu-id="8c1b9-106">Jūsu tīkls var bloķēt trafiku uz **g.Live.com** un **oneclient.SFX.MS**.</span><span class="sxs-lookup"><span data-stu-id="8c1b9-106">Your network might block traffic to **g.live.com** and **oneclient.sfx.ms**.</span></span> <span data-ttu-id="8c1b9-107">Ja šī satiksme ir bloķēta, OneDrive nevar veikt atjaunināšanu.</span><span class="sxs-lookup"><span data-stu-id="8c1b9-107">If that traffic is blocked, OneDrive cannot update itself.</span></span> <span data-ttu-id="8c1b9-108">Strādājiet ar tīkla administratoru, lai nodrošinātu piekļuvi šiem vietrāžiem URL.</span><span class="sxs-lookup"><span data-stu-id="8c1b9-108">Work with your network administrator to ensure you have access to those URLs.</span></span> <span data-ttu-id="8c1b9-109">[Šiem galapunktiem](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) jāsasniedz klienti, kas izmanto Microsoft 365 plānus.</span><span class="sxs-lookup"><span data-stu-id="8c1b9-109">[These endpoints](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) should be reachable for customers using Microsoft 365 plans.</span></span>

<span data-ttu-id="8c1b9-110">Ja jums ir manuāli jāiegūst pašreizējā OneDrive versija, apmeklējiet vietni [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .</span><span class="sxs-lookup"><span data-stu-id="8c1b9-110">If you need to manually get a current version of OneDrive, visit [https://aka.ms/getonedrive](https://aka.ms/getonedrive).</span></span>
