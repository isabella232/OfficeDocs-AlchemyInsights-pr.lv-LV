---
title: Paroļu žurnāli
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527174"
---
# <a name="password-logs"></a><span data-ttu-id="56249-102">Paroļu žurnāli</span><span class="sxs-lookup"><span data-stu-id="56249-102">Password logs</span></span>

<span data-ttu-id="56249-103">**Man ir problēmas ar piekļuvi paroļu atiestatīšanas audita žurnāliem**</span><span class="sxs-lookup"><span data-stu-id="56249-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="56249-104">Lai novērstu problēmas saistībā ar piekļuvi paroles atiestatīšanas audita žurnāliem, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="56249-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="56249-105">Pārliecinieties, vai esat autorizēts skatīt audita žurnālus.</span><span class="sxs-lookup"><span data-stu-id="56249-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="56249-106">Atļauta ir tikai tālāk norādītās lomas:</span><span class="sxs-lookup"><span data-stu-id="56249-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="56249-107">Globālais administrators</span><span class="sxs-lookup"><span data-stu-id="56249-107">Global administrator</span></span>
 - <span data-ttu-id="56249-108">Drošības administrators</span><span class="sxs-lookup"><span data-stu-id="56249-108">Security administrator</span></span>
 - <span data-ttu-id="56249-109">Drošības lasītājs</span><span class="sxs-lookup"><span data-stu-id="56249-109">Security reader</span></span>

<span data-ttu-id="56249-110">**Es vēlos redzēt visus paroles atiestatīšanas audita notikumus no sākotnēji izvietotā laika**</span><span class="sxs-lookup"><span data-stu-id="56249-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="56249-111">Līdz 120 000 Paroļu atiestatīšana/reģistrācijas notikumi tiek glabāti pēdējo 30 dienu atskaitēs.</span><span class="sxs-lookup"><span data-stu-id="56249-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="56249-112">Šis maksimālais ierobežojums attiecas uz UI, lejupielādējot CSV.</span><span class="sxs-lookup"><span data-stu-id="56249-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="56249-113">1 000 000 notikumi ir pieejami, izmantojot PowerShell.</span><span class="sxs-lookup"><span data-stu-id="56249-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="56249-114">Lai iegūtu papildinformāciju, skatiet tālāk norādītās saites.</span><span class="sxs-lookup"><span data-stu-id="56249-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="56249-115">Pašapkalpošanās paroles atiestatīšanas notikumi no Azure AD atskaitēm un notikumu API</span><span class="sxs-lookup"><span data-stu-id="56249-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="56249-116">Kā lejupielādēt paroles atiestatīšanas reģistrācijas notikumus ātri, izmantojot PowerShell</span><span class="sxs-lookup"><span data-stu-id="56249-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="56249-117">**Vēlos uzzināt vairāk par paroļu atiestatīšanas atskaišu iespējām**</span><span class="sxs-lookup"><span data-stu-id="56249-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="56249-118">Pārbaudiet, kurš reģistrē vai atiestata paroles ar Azure AD paroles atiestatīšanas audita žurnālus Azure portālā sadaļā **lietotāji un grupas**.</span><span class="sxs-lookup"><span data-stu-id="56249-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="56249-119">Lai iegūtu papildinformāciju, skatiet tālāk norādītās saites.</span><span class="sxs-lookup"><span data-stu-id="56249-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="56249-120">Pārskats par paroles atiestatīšanu</span><span class="sxs-lookup"><span data-stu-id="56249-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="56249-121">Kā skatīt paroles atiestatīšanas atskaites Azure portālā</span><span class="sxs-lookup"><span data-stu-id="56249-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="56249-122">Pašapkalpošanās paroles atiestatīšanas notikumi no Azure AD atskaitēm un notikumu API</span><span class="sxs-lookup"><span data-stu-id="56249-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="56249-123">Kā lejupielādēt paroles atiestatīšanas reģistrācijas notikumus ātri, izmantojot PowerShell</span><span class="sxs-lookup"><span data-stu-id="56249-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


