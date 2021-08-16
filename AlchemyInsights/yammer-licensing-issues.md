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
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989738"
---
# <a name="yammer-licensing-issues"></a>Yammer licencēšanas problēmas

Visiem lietotājiem ir nepieciešama licence, lai izmantotu Yammer Enterprise pakalpojumu, bet pēc Yammer nav nepieciešams, lai lietotājiem būtu licence, lai piekļūtu pakalpojumam. Kad administrators maina iestatījumu, lai bloķētu Microsoft 365 lietotājus bez Yammer licencēm, lietotāji, kuriem Yammer Enterprise licence, nevar piekļūt Yammer pakalpojumam. Papildinformāciju skatiet [rakstā Yammer licenču pārvaldība Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Kad lietotājiem tiek noņemtas licences, Yammer vairs netiek rādīts, un citi pakalpojumi var izmantot licenču noņemšanu, lai paslēptu līdzekļus. Citos gadījumos līdzekļi joprojām var būt redzami, taču tiem ir nepieciešama licenču piešķiršana darbības laikā.  

**Lietotājam netiek atjaunināta licence**  

Dažkārt lietotājam ir piešķirta licence, bet viņš joprojām nevar piekļūt Yammer. Aizkaves biežāk var rasties, kad tiek veikta lielapjoma licenču piešķiršana. Yammer lietotāji, iespējams, netiks atjaunināti tādā pašā secībā, kā licences tiek mainītas Azure AD, jo sistēma darbojas asinhroni. Uzgaidiet līdz 24 stundām, pirms atvērt atbalsta gadījumu, lai ziņotu par licenču sinhronizācijas problēmām.  

**Lielapjoma licenču piešķiršana**  

Licences var piešķirt, izmantojot administrēšanas centru vai PowerShell skriptēšanu. Papildinformāciju skatiet [rakstā Licenču piešķiršana lietotājiem un](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Licenču piešķiršana lietotāju [kontiem, izmantojot Office 365 PowerShell.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

Microsoft atbalsta dienests nenodrošina palīdzību saistībā ar skriptu izveidi, taču ir pieejama Yammer par licenču piešķiršanu. Papildinformāciju skatiet [rakstā Yammer licenču pārvaldība, izmantojot Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).