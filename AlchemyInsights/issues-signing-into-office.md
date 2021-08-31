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
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744653"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Problēmas ar pierakstīšanos Microsoft 365 programmas

Piezīme. Ja izmantojat vecāku Windows versiju (piemēram, Windows 7 SP1, Windows Server 2008 R2), izmantojiet [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) vienkāršo labojumu, lai iespējotu TLS 1.2 kā noklusējumu. Papildinformāciju skatiet rakstā Atjaunināšana, lai [iespējotu TLS 1.1 un TLS 1.2 kā noklusējuma drošos protokolus programmā WinHTTP Windows.](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Lai novērstu pierakstīšanās problēmas ar Microsoft 365 programmām, ietekmētajā datorā izmēģiniet šādas opcijas:  

- Informāciju Windows skatiet [Ieteikumi par biežāk sastopamo pierakstīšanās problēmu novēršanu](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- Ja jums ir Mac dators, [skatiet rakstu Nevar pierakstīties lietojumprogrammā Office 2016 for Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Padoms** Windows datoros mēs varam diagnosticēt un automātiski risināt vairākas bieži sastopamas Office pierakstīšanās problēmas. Lejupielādējiet un palaidiet  **[Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SaRA-OfficeSignInScenario)**, lai izmantotu mūsu automatizēto rīku.

**Piezīme.** Nav ieteicams atspējot moderno autentifikāciju (ADAL) vai tīmekļa konta pārvaldību (Web Account Management — WAM), lai labotu pierakstīšanās **vai aktivizācijas problēmas.** Ja rodas kļūdas, veidojot savienojumu ar Microsoft 365 izmantojot Office 2013, pārliecinieties, vai iespējojat [moderno](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) autentifikāciju Office klientam.

Konkrētas problēmu novēršanas darbības skatiet tālāk redzamajā rakstā.

[Savienojuma problēmas pierakstoties pēc atjaunināšanas uz Office 2016 būvējumu 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Nevarat pierakstīties savā organizācijas kontā, piemēram, pakalpojumā Office 365, Azure vai Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Kā novērst problēmas, kas nav saistītas ar programmām pārlūkprogrammā, kas nevar pierakstīties pakalpojumā Office 365, Azure vai Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Atkārtoti tiek prasīti akreditācijas dati programmā Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)