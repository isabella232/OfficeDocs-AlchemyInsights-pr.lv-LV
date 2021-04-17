---
title: Problēmas ar pierakstīšanos Microsoft 365 programmās
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833010"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Microsoft 365 programmu labošana: ziņojums "Jūsu datora uzticamās platformas modulis nedarbojas pareizi"

Lai novērstu šo kļūdu, izmēģiniet tālāk norādīto:

- Instalējiet jaunākos [Windows un](https://support.microsoft.com/help/4027667/windows-10-update) [Office atjauninājumus.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Notīriet Office akreditācijas](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) datus, izmantojot Windows akreditācijas datu pārvaldnieku.<br/>
    **Piezīme.** Office 2016 reģistra ceļi ir mainīti uz 16.0. (Piemēram, \Software\Microsoft\Office\16.0\Common\Identity\)
- Mēģiniet lietotāja [atkopšanas procesu,](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) lai izlabotu uzticamā platformas moduļa (TPM) kļūmes.
- Iestatiet EnableADAL = 0, veicot tālāk norādītās darbības.  
    1. Ar peles labo pogu noklikšķiniet uz Windows sākuma pogas, **izvēlieties Palaist,** ierakstiet **regedit** un pēc tam izvēlieties **Labi**.
    2. Atlasiet **Jā,** lai atļautu reģistra redaktoram veikt izmaiņas jūsu ierīcē.
    3. Reģistra redaktorā pievienojiet **EnableADAL** DWORD vērtību ar iestatījumu **0** sadaļā HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Papildinformāciju skatiet rakstā Savienojuma problēmas pierakstoties pēc atjaunināšanas uz [Office 2016 būvējumu 16.0.7967 operētājsistēmā Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)