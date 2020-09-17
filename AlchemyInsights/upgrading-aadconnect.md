---
title: 932 jaunināšanas AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806046"
---
# <a name="upgrade-azure-ad-connect"></a>Azure AD Connect jaunināšana

Pēc noklusējuma Azure AD Connect ir iespējota automātiskā jaunināšana, kas palīdz nodrošināt, ka izmantojat jaunāko versiju. Lai pārbaudītu automātiskos jaunināšanas iestatījumus, izmantojiet Azure AD PowerShell **Get-ADSyncAutoUpgrade** cmdlet. Cmdlet atgriezīs vienu no tālāk norādītajām vērtībām.

- **Iespējots**: iespējota automātiskā jaunināšana.

- **Atspējots**: Automātiskā jaunināšana ir atspējota.

- **Apturēts**: sistēmai vairs nav tiesības saņemt automātiskus jauninājumus. Šo vērtību nevar konfigurēt. to iestata sistēma.

Papildinformāciju skatiet rakstā [Automātiskā jaunināšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Lai lejupielādētu jaunāko Azure AD Connect versiju, dodieties uz [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
