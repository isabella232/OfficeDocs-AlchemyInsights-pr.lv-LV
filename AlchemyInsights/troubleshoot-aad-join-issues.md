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
ms.openlocfilehash: 8e902aea30e6891717e08027cc009576d390c9cf2ba1649cbbc68d64883937f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939926"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Azure AD pievienošanās problēmu novēršana

1. Ja iestatāt ierīču reģistrācijas pirmo reizi, pārliecinieties, vai esat pārskatījis Ievads par ierīču pārvaldību programmā [Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/devices/overview) kas palīdzēs iegūt ierīces Azure AD vadīklā. 
1. Ja reģistrējat ierīces Azure AD tieši un reģistrējat tās Intune, jums vispirms ir jākonfigurē [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) un vispirms jāveic licencēšana. [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign)
1. Pārliecinieties, vai esat pilnvarots veikt darbības Azure AD. Ierīču reģistrāciju iestatījumus var pārvaldīt tikai Azure Active Directory globālais administrators.
1. Lai ieviestu Azure AD savienojumu, skatiet [rakstu Azure AD pievienošanās plānošana.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Papildinformāciju par bieži sastopamo problēmu novēršanu saistībā ar Azure AD savienojumu skatiet rakstā Bieži uzdotie jautājumi par [Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) un Windows 10 pro ierīcēm skatiet rakstā Nevar pievienoties Windows 10 Pro datoram ar Azure AD — Jaunināšana — Microsoft [kopiena](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)
