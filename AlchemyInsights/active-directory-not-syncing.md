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
ms.openlocfilehash: 4bfbe6b2dd9a2112f0cb7af0d6e7a46693bc70680895fd674ddb0332b7071797
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937108"
---
# <a name="active-directory-not-syncing"></a>Active Directory netiek sinhronizēts

Ja saņemat sinhronizācijas kļūdas, piemēram, "nav nesenas sinhronizācijas" vai saņemat paziņojumu par direktorija sinhronizēšanas statusu Office administrēšanas portālā, tiek parādīts ziņojums "Pēdējoreiz sinhronizēts pirms vairāk nekā 3 dienām", iespējams, AADConnect ir nepareizi iestatījumi vai nepietiekamas atļaujas sinhronizācijas veikšanai.  

AADConnect atkārtota instalēšana, izmantojot ekspresiestatādes iestatījumus, var ātri atrisināt problēmu:

1. [Lejupielādējiet AADConnect jaunāko versiju.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Izpildiet norādījumus par ekspresinstalēšanu.](/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect ir jāinstalē Windows Server 2012 vai jaunākā versijā. Šim serverim ir jābūt pievienotam domēnam, un tas var būt domēna kontrolleris vai dalībnieku serveris. Lai iegūtu pilnu Azure AD ad Savienošana prasības un priekšnosacījumus, pārskatiet [Azure AD](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)Savienošana .

Papildinformāciju par AADConnect pakalpojumu kontiem skatiet rakstā [Azure AD Savienošana: Konti un atļaujas.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)
