---
title: Yammer licencēšanas problēmas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657283"
---
# <a name="yammer-licensing-issues"></a>Yammer licencēšanas problēmas

Visiem lietotājiem ir jābūt licencei, lai izmantotu Yammer Enterprise pakalpojumu, bet pēc noklusējuma Yammer neprasa lietotājiem piekļūt pakalpojumam. Ja administrators maina iestatījumu Microsoft 365 lietotāju bloķēšanai bez Yammer licencēm, lietotāji, kuriem nav piešķirtas Yammer Enterprise licences, nevar piekļūt Yammer pakalpojumam. Papildinformāciju skatiet rakstā [Yammer lietotāju licenču pārvaldība pakalpojumā Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Ja licences tiek noņemtas no lietotājiem, Yammer elements vairs netiek rādīts, un citi pakalpojumi var izmantot licences noņemšanu, lai paslēptu līdzekļus. Citos gadījumos līdzekļi joprojām var tikt rādīti, taču ir nepieciešama licences piešķiršana darbībai.  

**Licence lietotājam netiek atjaunināta**  

Dažkārt lietotājam ir piešķirta licence, bet joprojām nevar piekļūt pakalpojumam Yammer. Aizkaves var rasties, ja notiek masveida licenču piešķiršana. Yammer lietotāji, iespējams, netiek atjaunināti tādā pašā secībā, kā licences tiek mainītas Azure AD, jo sistēma darbojas asinhroni. Pirms atbalsta lietas atvēršanas jāgaida līdz pat 24 stundām, lai ziņotu par licenču sinhronizācijas problēmām.  

**Lielapjoma licenču piešķiršana**  

Licences var piešķirt no administrēšanas centra vai PowerShell skriptošanas. Papildinformāciju skatiet rakstā [licenču piešķiršana lietotājiem](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) un [licenču piešķiršana lietotāju kontiem, izmantojot Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Microsoft atbalsts nesniedz palīdzību par skriptu izveidi, bet ir pieejama dokumentācija par Yammer licenču piešķiršanu. Papildinformāciju skatiet rakstā [Yammer licenču pārvaldība, izmantojot Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).