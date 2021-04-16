---
title: Dublikāta ierīces ieraksts portālā
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
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814523"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="ffb92-102">Dublikāta ierīces ieraksts portālā</span><span class="sxs-lookup"><span data-stu-id="ffb92-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="ffb92-103">Ja ierīce nepareizi ziņo par līdzpārvaldības statusu konfigurācijas pārvaldnieka vietnē, iespējams, būs redzami divi ieraksti ierīcei portālā.</span><span class="sxs-lookup"><span data-stu-id="ffb92-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="ffb92-104">Lai pārbaudītu ierīces līdzpārvaldības statusu, pārskatiet ierīces **Līdzpārvaldības** kolonnu konfigurācijas pārvaldnieka konsolē.</span><span class="sxs-lookup"><span data-stu-id="ffb92-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="ffb92-105">Ja kolonna nav redzama, varat to pievienot, ar peles labo pogu noklikšķinot uz jebkuras kolonnas galvenes un atlasot to sarakstā.</span><span class="sxs-lookup"><span data-stu-id="ffb92-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="ffb92-106">Vienlaikus pārvaldītajai vērtībai ir jābūt **Jā**.</span><span class="sxs-lookup"><span data-stu-id="ffb92-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="ffb92-107">Ja vērtība ir **Nē**, atveriet konfigurācijas pārvaldnieka klienta sīklietotni klienta ierīcē un pārbaudiet, vai cilnē Vispārīgi **Līdzpārvaldības** rekvizītu.</span><span class="sxs-lookup"><span data-stu-id="ffb92-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="ffb92-108">Ja vērtība ir **Iespējota**, tas norāda uz problēmām ar klienta saziņu ar pārvaldības punktu.</span><span class="sxs-lookup"><span data-stu-id="ffb92-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="ffb92-109">Lūdzu, pārskatiet **CcmMessaging.log** ierīcē, lai izpētītu potenciālās savienojamības problēmas.</span><span class="sxs-lookup"><span data-stu-id="ffb92-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="ffb92-110">Ja vērtība ir **Atspējota** un ierīce ir reģistrēta Intune, lūdzu, pārliecinieties, vai ierīce ir saņēmusi pārvaldības politiku, pārskatot **CoManagementHandler.log** ierīcē.</span><span class="sxs-lookup"><span data-stu-id="ffb92-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
