---
title: Galapunkta DLP licencēšanas kļūda
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: 1e242abe18717e5ef64d6f067ab3ec6fa8833cb672dd21c85e577ce640240ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090154"
---
# <a name="endpoint-dlp-licensing-error"></a>Galapunkta DLP licencēšanas kļūda

Ja, mēģinot iestatīt galapunkta DLP, tiek parādīts šāds kļūdas ziņojums:

`Your organization is missing the licenses required to manage these devices`.

Pārliecinieties, vai jums ir viens no šiem abonementiem vai pievienojum pievienojumdēiem:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 atbilstība
- Microsoft 365 A5 atbilstība
- Microsoft 365 E5 informācijas aizsardzība un pārvaldība
- Microsoft 365 A5 informācijas aizsardzība un pārvaldība

> [!NOTE]
> Tas nedarbojas licenču kombinācijām, piemēram, Win E5 + O365 E5 + EMS E5. Lai varētu iestatīt šo līdzekli, ir nepieciešama tikai M365 E5 licence.

Papildinformāciju par galapunkta DLP licencēšanu skatiet rakstā [Galapunkta DLP licencēšana.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
