---
title: Ieplānoto atjauninājumu pauzēšana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555511"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="37457-102">Ieplānoto atjauninājumu pauzēšana</span><span class="sxs-lookup"><span data-stu-id="37457-102">Pausing scheduled updates</span></span>

<span data-ttu-id="37457-103">Kad komanda pauze ir izdota, ierīces neapstrādā komandu līdz nākamajai reizei, kad tās atmeklēs Intune.</span><span class="sxs-lookup"><span data-stu-id="37457-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="37457-104">Šī iemesla dēļ jūsu ierīces var būt:</span><span class="sxs-lookup"><span data-stu-id="37457-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="37457-105">Pirms atdošanas instalējāt plānotos atjauninājumus.</span><span class="sxs-lookup"><span data-stu-id="37457-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="37457-106">Izslēgts, kad izsniedzat komandu pauze.</span><span class="sxs-lookup"><span data-stu-id="37457-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="37457-107">Šajā gadījumā, kad ierīces bija ieslēgtas, tās, iespējams, pirms reģistrēšanās ir lejupielādējusi un instalējusi plānotos atjauninājumus.</span><span class="sxs-lookup"><span data-stu-id="37457-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>