---
title: Active Directory netiek sinhronizēts
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
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: d4615d335b9aeef69148cd93ff9f44bec6d7d876
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314211"
---
# <a name="active-directory-not-syncing"></a>Active Directory netiek sinhronizēts

Ja saņemat sinhronizācijas kļūdas, piemēram, "nav nesenas sinhronizācijas" vai saņemat paziņojumu par direktorija sinhronizēšanas statusu Office administrēšanas portālā tiek parādīts ziņojums "Pēdējoreiz sinhronizēts pirms vairāk nekā 3 dienām", iespējams, AADConnect ir nepareizi iestatījumi vai nepietiekamas atļaujas sinhronizācijas veikšanai.  

AADConnect atkārtota instalēšana, izmantojot ekspresiesta iestatījumus, var ātri atrisināt problēmu:

1. [Lejupielādējiet AADConnect jaunāko versiju.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Izpildiet norādījumus par ekspresinstalēšanu.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect ir jāinstalē Windows Server 2012 vai jaunākā versijā. Šim serverim ir jābūt pievienotam domēnam, un tas var būt domēna kontrolleris vai dalībnieku serveris. Lai iegūtu pilnu Azure AD ad Savienošana prasības un priekšnosacījumus, pārskatiet [Azure AD](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)Savienošana .

Papildinformāciju par AADConnect pakalpojumu kontiem skatiet rakstā [Azure AD Savienošana: Konti un atļaujas.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
