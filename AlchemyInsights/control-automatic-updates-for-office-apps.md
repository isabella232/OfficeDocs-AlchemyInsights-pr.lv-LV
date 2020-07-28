---
title: Office programmu automātisko atjauninājumu kontrolēšana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439335"
---
# <a name="control-automatic-updates-for-office-apps"></a>Office programmu automātisko atjauninājumu kontrolēšana

Pēc noklusējuma Office programmu atjauninājumi tiek lejupielādēti automātiski un izmantoti fonā bez lietotāja iejaukšanās. Taču administratori var kontrolēt, kā atjauninājumi tiek lietoti, izmantojot Office atjaunināšanas iestatījumus. Atjaunināšanas iestatījumi ļauj administratoriem iespējot vai atspējot automātisko atjaunināšanu, rādīt vai paslēpt Office **atjaunināšanas** pogu, iestatīt atjaunināšanas termiņus un veikt citas funkcijas. Detalizētu informāciju skatiet rakstā:

- [Office atjaunināšanas iestatījumu konfigurēšana](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Office automātiskā atjaunināšana nav iespējota](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Kā definēt, kā Office tiek atjaunināts pēc tam, kad tā ir instalēta](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Lai pārskatītu klienta datoram lietotos atjauninājumus, veiciet tālāk norādītās darbības.

1. Atveriet reģistra redaktoru, dodoties uz **Sākt**  >  **palaist**  >  **regedit**.
2. Pārslēdzieties uz šo atrašanās vietu un pārskatiet Office atjaunināšanas iestatījumus.  
    izveide. HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**Piezīmes**  Ja OfficeMgmtCOM atslēga ir iestatīta, iespējams, tiek rādīts ziņojums "atjauninājumi tiek pārvaldīti sistēmas administrators" **Office**  >  **konta**  >  **Office atjauninājumos**. Papildinformāciju skatiet rakstā [microsoft 365 programmu atjauninājumu pārvaldība, izmantojot Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  