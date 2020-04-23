---
title: 932 jaunināšana AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766500"
---
# <a name="upgrade-azure-ad-connect"></a>Azure AD savienojuma jaunināšana

Pēc noklusējuma ir iespējota automātiskā jaunināšana Azure AD savienojumu, kas palīdz nodrošināt jūs izmantojat jaunāko versiju. Lai pārbaudītu automātiskās jaunināšanas iestatījumus, izmantojiet Azure AD PowerShell cmdlet **Get ADSyncAutoUpgrade** . Cmdlet atgriezīs vienu no šīm vērtībām:

- **Iespējota**: Automātiskā jaunināšana ir iespējota.

- **Atspējots**: Automātiskā jaunināšana ir atspējota.

- **Apturēta**: sistēma vairs nav tiesīga saņemt automātiskus uzlabojumus. Šo vērtību nevar konfigurēt; to iestata sistēma.

Papildinformāciju skatiet sadaļā [Automātiska jaunināšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Lai lejupielādētu jaunāko versiju Azure AD savienojumu, dodieties uz [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
