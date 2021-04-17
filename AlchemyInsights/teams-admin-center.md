---
title: Teams administrēšanas centrs
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826386"
---
# <a name="teams-admin-center"></a><span data-ttu-id="e4faa-102">Teams administrēšanas centrs</span><span class="sxs-lookup"><span data-stu-id="e4faa-102">Teams Admin Center</span></span>

<span data-ttu-id="e4faa-103">Uzziniet par Teams pārvaldību, izmantojot [Teams administrēšanas centru](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="e4faa-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="e4faa-104">Ja nevarat piekļūt Teams administrēšanas centram, lūdzu, pārbaudiet tālāk norādīto.</span><span class="sxs-lookup"><span data-stu-id="e4faa-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="e4faa-105">Pārbaudiet, vai esat atļāvis atbilstošās [Office 365 IP adreses un URL](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) perimetra ierīcēs (ugunsmūrī utt.) vai ugunsmūra kārtulās jūsu lokālajā datorā.</span><span class="sxs-lookup"><span data-stu-id="e4faa-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="e4faa-106">Pārbaudiet, vai pieteikšanās informācija, kuru izmantojat, lai piekļūtu Teams administrēšanas portālam, atbilst jūsu lietotājvārdam, kas norādīts [Microsoft 365 administrēšanas portālā](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="e4faa-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="e4faa-107">Ja lietotāji netiek rādīti Teams administrēšanas centrā, lūdzu, pārbaudiet tālāk norādīto.</span><span class="sxs-lookup"><span data-stu-id="e4faa-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="e4faa-108">Vai esat izveidojis lietotājus vai piešķīris licences pēdējo 24 stundu laikā?</span><span class="sxs-lookup"><span data-stu-id="e4faa-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="e4faa-109">Lūdzu, pirms atbalsta biļetes atvēršanas nogaidiet vismaz 24 stundas.</span><span class="sxs-lookup"><span data-stu-id="e4faa-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="e4faa-110">Vai pārbaudījāt, vai esat piešķīris atbilstošas licences?</span><span class="sxs-lookup"><span data-stu-id="e4faa-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="e4faa-111">Ja izmantojat lokālo Active Directory, pārliecinieties, vai parametra [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) vērtība vai lokālā Active Directory lauka ProxyAddresses lauka SIP adrese ir unikāla un formāts atbilst **sip:** lietotāja lietotājvārds [no Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)administrēšanas centra.</span><span class="sxs-lookup"><span data-stu-id="e4faa-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="e4faa-112">Ja vēlaties paturēt Skype darbam Server izvietošanu un lietotāji ir mājās lokāli un tiešsaistē: izpildiet Skype darbam Server vadības paneļa sadaļā "Hibrīda iestatīšana ar Teams un Skype darbam **Online"** un pārvietojiet lietotājus tiešsaistē.</span><span class="sxs-lookup"><span data-stu-id="e4faa-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
