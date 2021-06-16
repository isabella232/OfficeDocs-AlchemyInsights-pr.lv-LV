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
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930982"
---
# <a name="active-directory-not-syncing"></a>Active Directory netiek sinhronizēts

Ja saņemat sinhronizācijas kļūdas, piemēram, "nav nesenas sinhronizācijas" vai saņemat paziņojumu par direktorija sinhronizēšanas statusu Office administrēšanas portālā, tiek parādīts ziņojums "Pēdējoreiz sinhronizēts pirms vairāk nekā 3 dienām", iespējams, AADConnect ir nepareizi iestatījumi vai nepietiekamas atļaujas sinhronizācijas veikšanai.  

AADConnect atkārtota instalēšana, izmantojot ekspresiestatādes iestatījumus, var ātri atrisināt problēmu:

1. [Lejupielādējiet AADConnect jaunāko versiju.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Izpildiet norādījumus par ekspresinstalēšanu.](/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect ir jāinstalē Windows Server 2012 vai jaunākā versijā. Šim serverim ir jābūt pievienotam domēnam, un tas var būt domēna kontrolleris vai dalībnieku serveris. Lai iegūtu pilnu Azure AD ad Savienošana prasības un priekšnosacījumus, pārskatiet [Azure AD](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)Savienošana .

Papildinformāciju par AADConnect pakalpojumu kontiem skatiet rakstā [Azure AD Savienošana: Konti un atļaujas.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)
