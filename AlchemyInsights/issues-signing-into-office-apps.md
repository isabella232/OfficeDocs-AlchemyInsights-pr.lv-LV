---
title: Problēmas saistībā ar pierakstīšanos Microsoft 365 lietojumprogrammās
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709113"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Microsoft 365 programmu labošana "jūsu datora uzticamā platformas modulis nedarbojas pareizi" ziņojums

Lai novērstu šo kļūdu, izmēģiniet tālāk norādīto:

- Instalējiet jaunākos [Windows](https://support.microsoft.com/help/4027667/windows-10-update) un [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)atjauninājumus.
- [Notīriet Office akreditācijas datus](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) , izmantojot Windows akreditācijas datu pārvaldnieku.<br/>
    **Piezīme:** Office 2016 reģistra ceļi ir mainīti uz 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Izmēģiniet [lietotāja atkopšanas procesu](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) , lai novērstu uzticamas platformas moduļa (TPM) kļūmes.
- Iestatiet EnableADAL = 0, veicot tālāk norādītās darbības.  
    1. Ar peles labo pogu noklikšķiniet uz Windows sākuma pogas, izvēlieties **palaist**, ierakstiet **regedit** un pēc tam izvēlieties **Labi**.
    2. Atlasiet **Jā** , lai atļautu reģistra redaktoram veikt izmaiņas jūsu ierīcē.
    3. Reģistra redaktorā pievienojiet DWORD vērtību **EnableADAL** ar iestatījumu **0** sadaļā HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Papildinformāciju skatiet rakstā [savienojuma problēmas ar pierakstīšanos pēc atjaunināšanas uz Office 2016 būvējumu 16.0.7967 operētājsistēmā Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).