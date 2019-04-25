---
title: Pārvēršot koplietojamās pastkastes lietotāja pastkasti?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374330"
---
Lietotāja pastkastē var konvertēt tikai koplietojamā pastkasti, ja lietotājam ir Exchange licences. Pēc konvertēšanas pastkasti, tā turpinās, jo šis saraksts ietver kopīgu pastkastes Aktīvie lietotāji sarakstā parādās. Tomēr konvertēto pastkastītē arī parādīsies koplietojamo pastkastu sarakstā. 
  
Ja jūs mēģināt konvertēt ar pastkasti Exchange administratora konsole un konversijas neizdodas, notīrīt pārlūkprogrammas kešatmiņu un sīkfailus un mēģiniet vēlreiz. Ja tas joprojām nedarbojas, mēģiniet konvertēt uz pastkasti Exchange Management Shell, izpildot šādu komandu:
  
```
Set-Mailbox -Type Shared
```

Vairākas pastkastes konversijas informācija ir pieejama [pārvērst koplietojamās pastkastes lietotāja pastkastes](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
