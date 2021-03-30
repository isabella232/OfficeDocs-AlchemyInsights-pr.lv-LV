---
title: Azure AD pievienošanās problēmu novēršana
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405129"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Azure AD pievienošanās problēmu novēršana

1. Ja iestatāt ierīču reģistrācijas pirmo reizi, pārliecinieties, vai esat pārskatījis Ievads par ierīču pārvaldību pakalpojumā [Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/devices/overview) kas sniegs norādījumus par to, kā Azure AD vadīklā iegūt ierīces. 
1. Ja reģistrējat ierīces Azure AD tieši un reģistrējat tās Intune, jums vispirms ir jākonfigurē [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) un vispirms jāveic licencēšana. [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign)
1. Pārliecinieties, vai esat pilnvarots veikt darbības Azure AD. Ierīces reģistrāciju iestatījumus var pārvaldīt tikai globālais administrators Azure AD.
1. Lai ieviestu Azure AD savienojumu, skatiet [rakstu Azure AD pievienošanās plānošana.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Lai iegūtu papildinformāciju par bieži sastopamo problēmu novēršanu saistībā ar Azure AD savienojumu, skatiet rakstu Bieži uzdotie jautājumi par [Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) un Windows 10 pro ierīcēm, skatiet rakstu Nevar pievienoties Windows [10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) datoram uz Azure AD — Jaunināšana — Microsoft kopiena
