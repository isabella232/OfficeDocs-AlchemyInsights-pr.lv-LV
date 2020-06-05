---
title: Problēmas pierakstoties Microsoft 365 Apps
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
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579908"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tukšu pierakstīšanās ekrānu Microsoft 365 Apps

Lai atrisinātu šo problēmu, mēģiniet veikt šādas darbības:
- Instalējiet jaunākos [Windows](https://support.microsoft.com/help/4027667/windows-10-update) un [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)atjauninājumus.
- Atiestatīt Internet Explorer opcijas: dodieties uz **Rīki**,  >  **interneta opcijas**  >  **Advanced**  >  ,**Atiestatīt Internet Explorer iestatījumus** (ņemiet vērā, ka tiks zaudēti pielāgotie iestatījumi) un pēc tam mēģiniet pierakstīties pakalpojumā Office vēlreiz.
- Atspējojiet Windows Defender lietojumprogrammu aizsargs (WDAG) vai citu līdzīgu ugunsmūri vai pretvīrusu programmu:
    1. Vadības panelī atveriet **programmas**un pēc tam izvēlieties **ieslēgt vai izslēgt Windows līdzekļus**.
    2. Ja ir iespējots Windows Defender lietojumprogrammu aizsargs, atspējojiet to.<br/>
    **Piezīme:** Iespējams, būs jārestartē dators.
- Pārliecinieties, ka Microsoft. AAD. BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nav bloķē jebkura lietojumprogramma vai ugunsmūra/anti-virus programmu.
- [Notīrīt Office akreditācijas datus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , izmantojot Windows akreditācijas datu pārvaldnieku.<br/>
    **Piezīme:** Office 2016 reģistra ceļi ir mainījušies 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Lai iegūtu papildinformāciju, skatiet [savienojuma problēmas pierakstīšanās pēc atjauninājuma Office 2016 veidot 16.0.7967 operētājsistēmā Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).