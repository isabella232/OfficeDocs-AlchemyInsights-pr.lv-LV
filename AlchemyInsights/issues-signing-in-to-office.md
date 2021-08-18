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
- "2556"
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088043"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tukšs pierakstīšanās ekrāns Microsoft 365 programmās

Lai novērstu šo problēmu, mēģiniet veikt šādas darbības:
- Instalējiet jaunākos atjauninājumus [lietojumprogrammām Windows](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Internet Explorer opciju atiestatīšana. Dodieties uz sadaļu Rīki Internet Options Internet Explorer papildu  >    >    >  **atiestatīšanas Iestatījumi** (ņemiet vērā, ka zaudēsit pielāgotos iestatījumus) un pēc tam vēlreiz mēģiniet pierakstīties programmā Office.
- Atspējojiet Windows Defender Application Guard (WDAG) vai citu līdzīgu ugunsmūri vai pretvīrusu programmu:
    1. Vadības panelī dodieties uz **Sadaļu** Programmas un pēc **tam Windows ieslēgt vai izslēgt šos līdzekļus.**
    2. Ja Windows Defender Application Guard ir iespējots, mēģiniet to atspējot.<br/>
    **Piezīme.** Iespējams, būs jārestartē dators.
- Pārliecinieties, vai Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) spraudni nebloķē neviena lietojumprogramma vai ugunsmūra/pretvīrusu programma.
- [Notīriet Office akreditācijas](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) datus, Windows akreditācijas datu pārvaldnieku.<br/>
    **Piezīme.** 2016. Office gada reģistra ceļi ir mainīti uz 16.0. (Piemēram: \Software\Microsoft\Office\16.0\Common\Identity\)

Papildinformāciju skatiet rakstā Savienojuma problēmas pierakstoties pēc atjaunināšanas uz [Office 2016 būvējumu 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).