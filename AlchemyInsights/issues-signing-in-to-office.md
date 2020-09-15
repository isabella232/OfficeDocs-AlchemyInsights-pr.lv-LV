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
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695294"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tukšs pierakstīšanās ekrāns Microsoft 365 lietojumprogrammās

Lai novērstu šo problēmu, mēģiniet veikt šādas darbības:
- Instalējiet jaunākos [Windows](https://support.microsoft.com/help/4027667/windows-10-update) un [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)atjauninājumus.
- Atiestatīt Internet Explorer opcijas: dodieties uz sadaļu **Rīki**  >  **interneta opcijas**  >  **papildu**  >  **Atiestatīt Internet Explorer iestatījumus** (ņemiet vērā, ka zudīs pielāgoti iestatījumi) un pēc tam vēlreiz mēģiniet pierakstīties sistēmā Office.
- Atspējojiet Windows Defender lietojumprogrammas aizsargu (WDAG) vai kādu līdzīgu ugunsmūru vai pretvīrusu programmu.
    1. Vadības panelī atveriet sadaļu **programmas**un pēc tam izvēlieties **Ieslēgt vai izslēgt Windows līdzekļus**.
    2. Ja ir iespējots Windows Defender lietojumprogrammas aizsargs, mēģiniet to atspējot.<br/>
    **Piezīme:** Iespējams, būs jārestartē dators.
- Pārliecinieties, vai Microsoft. AAD. BrokerPlugin [AAD WAM spraudni](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nebloķē neviena lietojumprogramma vai ugunsmūris/pretvīrusu programma.
- [Notīriet Office akreditācijas datus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , izmantojot Windows akreditācijas datu pārvaldnieku.<br/>
    **Piezīme:** Office 2016 reģistra ceļi ir mainīti uz 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Papildinformāciju skatiet rakstā [savienojuma problēmas ar pierakstīšanos pēc atjaunināšanas uz Office 2016 būvējumu 16.0.7967 operētājsistēmā Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).