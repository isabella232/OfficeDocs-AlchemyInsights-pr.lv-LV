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
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833046"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tukšs pierakstīšanās ekrāns Microsoft 365 programmās

Lai novērstu šo problēmu, mēģiniet veikt šādas darbības:
- Instalējiet jaunākos [Windows un](https://support.microsoft.com/help/4027667/windows-10-update) [Office atjauninājumus.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Atiestatiet Internet Explorer opcijas. Dodieties uz Sadaļu Rīki Interneta opcijas Internet Explorer papildu atiestatīšanas iestatījumi (ņemiet vērā, ka zaudēsit pielāgotos iestatījumus) un pēc tam vēlreiz mēģiniet  >    >    >   pierakstīties sistēmā Office.
- Atspējojiet Windows Defender Application Guard (WDAG) vai citu līdzīgu ugunsmūri vai pretvīrusu programmu:
    1. Vadības panelī dodieties uz **sadaļu Programmas** un pēc tam **izvēlieties Ieslēgt vai izslēgt Windows līdzekļus.**
    2. Ja līdzeklis Windows Defender Application Guard ir iespējots, mēģiniet to atspējot.<br/>
    **Piezīme.** Iespējams, būs jārestartē dators.
- Pārliecinieties, vai Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) spraudni nebloķē neviena lietojumprogramma vai ugunsmūra/pretvīrusu programma.
- [Notīriet Office akreditācijas](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) datus, izmantojot Windows akreditācijas datu pārvaldnieku.<br/>
    **Piezīme.** Office 2016 reģistra ceļi ir mainīti uz 16.0. (Piemēram, \Software\Microsoft\Office\16.0\Common\Identity\)

Papildinformāciju skatiet rakstā Savienojuma problēmas pierakstoties pēc atjaunināšanas uz [Office 2016 būvējumu 16.0.7967 operētājsistēmā Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)