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
ms.openlocfilehash: d0ef27e7c03eb8bcd9de74c58a5e0398d8892a6eb0ab50944b3c2201247fa0b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/11/2021
ms.locfileid: "57889225"
---
# <a name="active-directory-not-syncing"></a>Active Directory netiek sinhronizēts

Ja saņemat sinhronizācijas kļūdas, piemēram, "nav nesenas sinhronizācijas" vai saņemat paziņojumu par direktorija sinhronizēšanas statusu Office administrēšanas portālā, tiek norādīts "Pēdējoreiz sinhronizēts pirms vairāk nekā 3 dienām", iespējams, AADConnect ir nepareizi iestatījumi vai nepietiekamas atļaujas sinhronizācijas veikšanai.  

AADConnect atkārtota instalēšana, izmantojot ekspresiesta iestatījumus, var ātri atrisināt problēmu:

1. [Lejupielādējiet AADConnect jaunāko versiju.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Izpildiet norādījumus par ekspresinstalēšanu.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect ir jāinstalē Windows Server 2012 vai jaunākā versijā. Šim serverim ir jābūt pievienotam domēnam, un tas var būt domēna kontrolleris vai dalībnieku serveris. Lai iegūtu pilnu Azure AD ad Savienošana prasības un priekšnosacījumus, pārskatiet [Azure AD](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)Savienošana .

Papildinformāciju par AADConnect pakalpojumu kontiem skatiet rakstā [Azure AD Savienošana: Konti un atļaujas.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
