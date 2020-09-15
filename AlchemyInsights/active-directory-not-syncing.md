---
title: Active Directory netiek sinhronizēts
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697636"
---
# <a name="active-directory-not-syncing"></a>Active Directory netiek sinhronizēts

Ja saņemat sinhronizācijas kļūdas, piemēram, "nav pēdējās sinhronizācijas" vai paziņojums par direktorija sinhronizēšanas statusu Office administrēšanas portālā, tiek rādīts ziņojums "Pēdējoreiz sinhronizēts vairāk nekā pirms 3 dienām", iespējams, ka AADConnect ir nepareizi iestatījumi vai nepietiekamas atļaujas, lai veiktu sinhronizēšanu.  

AADConnect atkārtota instalēšana, izmantojot ekspresiestatījumus, var ātri atrisināt šo problēmu:

1. [Lejupielādējiet jaunāko AADConnect versiju](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Izpildiet norādījumus saistībā ar izteiktu instalēšanu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Papildinformāciju par AADConnect pakalpojumu kontiem skatiet rakstā [AZURE ad Connect: konti un atļaujas](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
