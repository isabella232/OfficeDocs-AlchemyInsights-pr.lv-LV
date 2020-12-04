---
title: Papildu autentifikācijas principi, kas attiecas uz Microsoft Edge
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573523"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Papildu autentifikācijas principi, kas attiecas uz Microsoft Edge

Tālāk ir norādīti papildu autentifikācijas jēdzieni, kas attiecas uz Microsoft Edge:

**Proaktīvā autentifikācija**

Iespējojot [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) politiku, Microsoft Edge mēģinās proaktīvi autentificēt lietotājus, izmantojot Microsoft pakalpojumus. Regulāros intervālos tā izmantos tiešsaistes pakalpojumu, lai pārbaudītu, vai ir atjaunināts saraksts, kurā ir iekļauta konfigurācija, kas reglamentē proaktīvo autentifikāciju.

Priekšrocības: proaktīvā autentifikācija nodrošina autentifikāciju ar galvenajiem pakalpojumiem, piemēram, Office jaunās cilnes lapu. Turklāt, ja Bing tiek izmantots kā meklēšanas dzinējs, proaktīvā autentifikācija uzlabo adrešu joslas veiktspēju un palīdz ģenerēt meklēšanas rezultātus, kas ir personalizēti uzņēmuma vajadzībām.

**Windows Hello CredUI NTLM autentifikācijai**

Ja vienotā pierakstīšanās (SSO) nav pieejama, ja tīmekļa vietne mēģina lietotājam pierakstīties, izmantojot NTLM vai sarunas mehānismu, šis līdzeklis ļaus lietotājam kopīgot OS akreditācijas datus ar tīmekļa vietni un izpildīt autentifikācijas problēmu, izmantojot Windows Hello Cred UI. Šī pierakstīšanās plūsma būs pieejama tikai operētājsistēmā Windows 10 un tikai tiem lietotājiem, kas nesaņem SSO NTLM vai sarunas laikā.

**Saglabāto paroļu izmantošana, lai automātiski pierakstītos**

Lietotāji, kas saglabā paroles pārlūkprogrammā Microsoft Edge, var iespējot automātisko pierakstīšanos tīmekļa vietnēm, kurās ir saglabāti akreditācijas dati. Lietotāji var ieslēgt vai izslēgt šo līdzekli pakalpojumā edge://settings/passwords, un varat to konfigurēt [paroļu pārvaldnieka](https://go.microsoft.com/fwlink/?linkid=2134622) politikās.
