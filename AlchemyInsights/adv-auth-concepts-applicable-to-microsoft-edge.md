---
title: Paplašinātās autentifikācijas jēdzieni, kas attiecas uz Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934372"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Paplašinātās autentifikācijas jēdzieni, kas attiecas uz Microsoft Edge

Tālāk ir papildu autentifikācijas jēdzieni, kas attiecas uz Microsoft Edge:

**Proactive Authentication**

Ja iespējojat [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) politiku, Microsoft Edge proaktīvi autentificēt pierakstītos lietotājus, izmantojot Microsoft pakalpojumi. Regulāros intervālos tas izmantos tiešsaistes pakalpojumu, lai meklētu atjauninātu manifestu, kas ietver konfigurāciju, kas nosaka proaktīvu autentifikāciju.

Priekšrocības. Proaktīvā autentifikācija iespējo autentifikāciju atslēgas pakalpojumiem, piemēram, Office jaunas cilnes lapai. Turklāt, ja Bing meklētājprogramma, proactive Authentication uzlabo adrešu joslas veiktspēju un palīdz ģenerēt meklēšanas rezultātus, kas pielāgoti jūsu uzņēmuma vajadzībām.

**Windows Hello CredUI NTLM autentifikācijai**

Ja vienotā pierakstīšanās (single sign-on — SSO) nav pieejama, ja tīmekļa vietne mēģina pierakstīties lietotājam, izmantojot NTLM vai apspriedēšanas mehānismu, šis līdzeklis sniedz lietotājam iespēju koplietot OS akreditācijas datus ar tīmekļa vietni un izpildīt autentifikācijas uzdevumu, izmantojot Windows Hello akreditācijas datu lietotāja interfeisu. Šī pierakstīšanās plūsma būs redzama tikai pakalpojumā Windows 10 un tikai tiem lietotājiem, kuri nesaņem SSO NTLM vai apspriedīšanas izaicinājuma laikā.

**Saglabāto paroļu izmantošana, lai pierakstītos automātiski**

Lietotāji, kas saglabā paroles pakalpojumā Microsoft Edge var iespējot automātisko pierakstīšanu tīmekļa vietnēs, kurās viņi ir saglabāuši akreditācijas datus. Lietotāji var ieslēgt vai izslēgt šo līdzekli edge://settings/passwords un varat to konfigurēt paroļu [pārvaldnieka politikās.](https://go.microsoft.com/fwlink/?linkid=2134622)
