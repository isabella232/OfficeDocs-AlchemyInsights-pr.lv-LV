---
title: Hibrīda Azure Active Directory savienojuma problēmu novēršana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939278"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Hibrīda Azure Active Directory savienojuma problēmu novēršana

Ļoti ieteicams nodrošināt, ka ierīce var piekļūt ierīces reģistrācijas galapunktiem sistēmas kontā, izmantojot [Ierīces reģistrācijas savienojamības testa skriptu](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Ja ierīču reģistrācijas iestatāt pirmo reizi, noteikti pārskatiet sadaļu [Ievads par ierīču pārvaldību Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/), lai uzzinātu, kā pārvaldīt Azure Active Directory.
1. Ja tieši reģistrējat ierīces Azure AD un reģistrējat tās Intune, pārliecinieties, vai esat [konfigurējis Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) un ka instalētas [licences](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Pārliecinieties, vai esat pilnvarots veikt darbības Azure Active Directory un lokālajā Active Directory. Ierīču reģistrāciju iestatījumus var pārvaldīt tikai Azure Active Directory globālais administrators. Turklāt, ja iestatāt automātiskas reģistrācijas lokālajā Active Directory, jums būs jābūt Active Directory un AD FS administratoram (ja piemērojams).

Papildinformāciju par iespējamo hibrīdā savienojuma problēmu risināšanu skatiet rakstā [Hibrīda savienojuma problēmu novēršana](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current), lai iestatītu hibrīda Azure Active Directory pievienotās un pārvaldītās ierīces, izmantojot Azure Active Directory portālu, skatiet rakstu [Hibrīda Azure AD pievienoto (lokālajam domēnam pievienoto) ierīču iestatīšana](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) un [Ierīču pārvaldība, izmantojot Azure portālu](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Lai novērstu bieži sastopamas problēmas ar hibrīda Azure Active Directory (AD) savienojumu, skatiet rakstu [Bieži uzdotie jautājumi par hibrīda Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
