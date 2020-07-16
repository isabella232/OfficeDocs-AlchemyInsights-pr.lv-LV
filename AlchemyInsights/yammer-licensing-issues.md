---
title: Yammer licencēšanas problēmas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148313"
---
# <a name="yammer-licensing-issues"></a>Yammer licencēšanas problēmas

Visiem lietotājiem ir jābūt licencei izmantot Pakalpojumu Yammer Enterprise, bet pēc noklusējuma Yammer nepieprasa lietotājiem ir licence, lai piekļūtu pakalpojumam. Kad administrators maina iestatījumu, lai bloķētu Microsoft 365 lietotājiem bez Yammer licences, lietotājiem nav piešķirta Yammer uzņēmuma licence nevar piekļūt Yammer pakalpojumu. Papildinformāciju skatiet rakstā [Yammer lietotāju licenču pārvaldība pakalpojumā Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Kad licences tiek noņemtas no lietotājiem, Yammer elements vairs netiek rādīts un citi pakalpojumi var izmantot licences noņemšanas paslēpt līdzekļus. Citos gadījumos funkcijas joprojām var parādīties, bet pieprasīt licences piešķiršanu, lai darbotos.  

**Licence nesaņem lietotājam atjauninātu**  

Reizēm lietotājam tiek piešķirta licence, bet joprojām nevar piekļūt Yammer. Aizkaves, visticamāk, radīsies, ja notiek masveida licences piešķiršana. Yammer lietotāji, iespējams, netiks atjaunināti tādā pašā secībā kā licences tiek mainīti Azure AD, jo sistēma darbojas asinhroni. Uzgaidiet līdz 24 stundām pirms atbalsta pieteikuma atvēršanas, lai ziņotu par licences sinhronizācijas problēmām.  

**Lielapjoma licenču piešķiršana**  

Licences var piešķirt, izmantojot administrēšanas centru vai PowerShell skriptu. Papildinformāciju skatiet rakstā [Licenču piešķiršana lietotājiem un Licenču](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) [piešķiršana lietotāju kontiem pakalpojumā Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Microsoft atbalsts nenodrošina palīdzību skriptu izveidei, bet ir pieejama dokumentācija par Yammer licences piešķiršanu. Papildinformāciju skatiet rakstā [Yammer licenču pārvaldība, izmantojot programmu Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).