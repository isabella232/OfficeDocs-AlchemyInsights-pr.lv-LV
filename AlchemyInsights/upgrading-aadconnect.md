---
title: 932 AADConnect jaunināšana
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
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104819"
---
# <a name="upgrade-azure-ad-connect"></a>Azure AD jaunināšanas Savienošana

Pēc noklusējuma Azure AD Savienošana ir iespējota automātiskā jaunināšana, kas palīdz nodrošināt, ka izmantojat jaunāko versiju. Lai pārbaudītu automātiskās jaunināšanas iestatījumus, izmantojiet **Get-ADSyncAutoUpgrade** cmdlet azure AD PowerShell. Cmdlet atgriezīs vienu no šīm vērtībām:

- **Iespējota:** automātiskā jaunināšana ir iespējota.

- **Atspējots:** automātiskā jaunināšana ir atspējota.

- **Aizturēts:** sistēma vairs nav piemērota automātisko jauninājumu saņemšanai. Jūs nevarat konfigurēt šo vērtību; to iestata sistēma.

Papildinformāciju skatiet sadaļā [Automātiska jaunināšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Lai lejupielādētu Jaunāko Azure AD Savienošana versiju, dodieties uz [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
