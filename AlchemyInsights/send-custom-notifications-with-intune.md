---
title: Nosūtīt pielāgotus paziņojumus ar Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720653"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="bedf1-102">Kā nosūtīt pielāgotus paziņojumus pārvaldīto iOS un Android ierīču lietotājiem</span><span class="sxs-lookup"><span data-stu-id="bedf1-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="bedf1-103">Pielāgotus paziņojumus for Intune apstrādā uzņēmuma portāla programma lietotāja ierīcē.</span><span class="sxs-lookup"><span data-stu-id="bedf1-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="bedf1-104">Programma pēc tam šajā ierīcē izveido pašpiegādes paziņojumu.</span><span class="sxs-lookup"><span data-stu-id="bedf1-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="bedf1-105">Tālāk ir norādīti ierīču priekšnosacījumi, lai nodrošinātu pielāgotu paziņojumu saņemšanu, un programma, lai izveidotu pašpiegādes paziņojumu:</span><span class="sxs-lookup"><span data-stu-id="bedf1-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="bedf1-106">Ierīcē jābūt instalētai uzņēmuma portāla lietojumprogrammai.</span><span class="sxs-lookup"><span data-stu-id="bedf1-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="bedf1-107">Ierīcei ir jāatļauj uzņēmuma portāla programma, lai nosūtītu pašpiegādes paziņojumus.</span><span class="sxs-lookup"><span data-stu-id="bedf1-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="bedf1-108">Kad programma ir instalēta vai atjaunināta, lietotājam tiek lūgts atļaut paziņojumus.</span><span class="sxs-lookup"><span data-stu-id="bedf1-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="bedf1-109">Android ierīcēs ir jāinstalē Google Play pakalpojumi.</span><span class="sxs-lookup"><span data-stu-id="bedf1-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="bedf1-110">Ierīcei jābūt reģistrētai ar Intune.</span><span class="sxs-lookup"><span data-stu-id="bedf1-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="bedf1-111">Papildinformāciju, tostarp, kā nosūtīt ziņojumu, skatiet sadaļā [līdzekļu dokumentācija](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="bedf1-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
