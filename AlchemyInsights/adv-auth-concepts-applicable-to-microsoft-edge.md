---
title: Paplašinātie autentifikācijas jēdzieni, kas attiecas uz Microsoft Edge
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
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398592"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Paplašinātie autentifikācijas jēdzieni, kas attiecas uz Microsoft Edge

Tālāk ir papildu autentifikācijas jēdzieni, kas attiecas uz Microsoft Edge:

**Proactive Authentication**

Ja iespējojat [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) politiku, Microsoft Edge mēģina proaktīvi autentificēt pierakstītos lietotājus, izmantojot Microsoft pakalpojumus. Regulāros intervālos tas izmantos tiešsaistes pakalpojumu, lai meklētu atjauninātu manifestu, kas ietver konfigurāciju, kas nosaka proaktīvu autentifikāciju.

Priekšrocības. Proaktīvā autentifikācija iespējo autentifikāciju atslēgas pakalpojumiem, piemēram, Office jaunas cilnes lapai. Turklāt, ja Bing tiek izmantota kā meklētājprogramma, proaktīvā autentifikācija uzlabo adrešu joslas veiktspēju un palīdz ģenerēt meklēšanas rezultātus, kas pielāgoti jūsu uzņēmuma vajadzībām.

**Windows Hello CredUI NTLM autentifikācijai**

Ja vienotā pierakstīšanās (single sign-on — SSO) nav pieejama, tīmekļa vietne mēģina pierakstīties lietotājam, izmantojot NTLM vai apspriedēm mehānismu, šis līdzeklis sniedz lietotājam iespēju koplietot operētājsistēmas akreditācijas datus ar tīmekļa vietni un izpildīt autentifikācijas uzdevumu, izmantojot Windows Hello akreditācijas datu lietotāja interfeisu. Šī pierakstīšanās plūsma tiks rādīta tikai sistēmā Windows 10 un tikai tiem lietotājiem, kuri nesaņem SSO NTLM vai apspriedīs uzdevumu.

**Saglabāto paroļu izmantošana, lai pierakstītos automātiski**

Lietotāji, kas saglabā paroles programmā Microsoft Edge, var iespējot automātisko pierakstīšanu tīmekļa vietnēs, kurās viņi ir saglabājis akreditācijas datus. Lietotāji var ieslēgt vai izslēgt šo līdzekli edge://settings/passwords un varat to konfigurēt paroļu [pārvaldnieka politikās.](https://go.microsoft.com/fwlink/?linkid=2134622)
