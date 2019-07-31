---
title: Pierakstīšanās pakalpojumā Office apps jautājumiem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938272"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Nosakot Biroja apps "datora uzticamo platformas modulis nedarbojas pareizi" ziņojums

Lai novērstu šo kļūdu, rīkojieties šādi:

- [Windows](https://support.microsoft.com/help/4027667/windows-10-update) un [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)instalētu jaunākos atjauninājumus.
- [Notīrīt biroja akreditācijas datus](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , izmantojot Windows Credential Manager.<br/>
    **Piezīme:** Ir mainījušies 16,0 Office 2016 reģistra ceļus. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Izmēģiniet [lietotāja atkopšanas process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) uzticamā platformas moduļa (TPM) nepilnības novērst.
- Noteikt EnableADAL = 0, veicot šādas darbības:  
    1. Ar peles labo pogu noklikšķiniet uz Windows pogas Sākt, izvēlēties **palaist**, ierakstiet **regedit**un pēc tam izvēlieties **Labi**.
    2. Izvēlieties **Jā** lai varētu reģistra redaktoru, lai veiktu izmaiņas jūsu ierīcē.
    3. Registry Editor pievienojiet DWORD vērtība ir **EnableADAL** iestatījums **0** zem HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Papildinformāciju skatiet sadaļā [savienojuma problēmas pierakstīšanās pēc Biroja 2016 būvēt 16.0.7967 10 Windows atjauninājums](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).