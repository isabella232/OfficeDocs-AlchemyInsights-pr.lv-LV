---
title: Pielāgoto paziņojumu sūtīšana, izmantojot InTune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886864"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="b7fdd-102">Kā nosūtīt pielāgotus paziņojumus pārvaldīto iOS un Android ierīču lietotājiem</span><span class="sxs-lookup"><span data-stu-id="b7fdd-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="b7fdd-103">Pielāgotus paziņojumus par InTune apstrādā uzņēmuma portāla lietojumprogramma lietotāja ierīcē.</span><span class="sxs-lookup"><span data-stu-id="b7fdd-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="b7fdd-104">Pēc tam programma izveido pašpiegādes paziņojumu šajā ierīcē.</span><span class="sxs-lookup"><span data-stu-id="b7fdd-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="b7fdd-105">Tālāk ir norādīti ierīču priekšnosacījumi, lai atbalstītu pielāgotu paziņojumu saņemšanu, un, lai programma pēc tam izveidotu pašpiegādes paziņojumu:</span><span class="sxs-lookup"><span data-stu-id="b7fdd-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="b7fdd-106">Ierīcei jābūt instalētai uzņēmuma portāla programmai.</span><span class="sxs-lookup"><span data-stu-id="b7fdd-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="b7fdd-107">Ierīcei ir jāļauj uzņēmuma portāla programmai nosūtīt pašpiegādes paziņojumus.</span><span class="sxs-lookup"><span data-stu-id="b7fdd-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="b7fdd-108">Kad lietotne ir instalēta vai atjaunināta, tā liks lietotājam atļaut paziņojumus.</span><span class="sxs-lookup"><span data-stu-id="b7fdd-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="b7fdd-109">Android ierīcēs ir jābūt instalētam Google Play pakalpojumiem.</span><span class="sxs-lookup"><span data-stu-id="b7fdd-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="b7fdd-110">Ierīce ir uzņemti ar InTune.</span><span class="sxs-lookup"><span data-stu-id="b7fdd-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="b7fdd-111">Papildinformāciju, tostarp informāciju par to, kā nosūtīt ziņojumu, skatiet [līdzekļa dokumentācijā](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="b7fdd-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
