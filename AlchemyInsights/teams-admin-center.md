---
title: Teams administrēšanas centrs
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 29e54e0f8255b4ce84c433f2cc827aaedf35327626f0095788faef802763bc53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049351"
---
# <a name="teams-admin-center"></a>Teams administrēšanas centrs

Uzziniet par Teams pārvaldību, izmantojot [Teams administrēšanas centru](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Ja nevarat piekļūt Teams administrēšanas centram, lūdzu, pārbaudiet tālāk norādīto.

- Pārbaudiet, vai esat atļāvis atbilstošās [Office 365 IP adreses un URL](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) perimetra ierīcēs (ugunsmūrī utt.) vai ugunsmūra kārtulās jūsu lokālajā datorā.
- Pārbaudiet, vai pieteikšanās informācija, kuru izmantojat, lai piekļūtu Teams administrēšanas portālam, atbilst jūsu lietotājvārdam, kas norādīts [Microsoft 365 administrēšanas portālā](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Ja lietotāji netiek rādīti Teams administrēšanas centrā, lūdzu, pārbaudiet tālāk norādīto.

- Vai esat izveidojis lietotājus vai piešķīris licences pēdējo 24 stundu laikā? Lūdzu, pirms atbalsta biļetes atvēršanas nogaidiet vismaz 24 stundas.
- Vai pārbaudījāt, vai esat piešķīris atbilstošas licences?
- Ja izmantojat lokālo Active Directory, pārbaudiet, vai [lauka msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) vērtība vai lokālā Active Directory laukā ProxyAddresses parametra SIP adrese ir unikāla un formāts atbilst **sip:** lietotāja lietotājvārds no [Microsoft 365 administrēšanas centrs](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Ja vēlaties paturēt Skype darbam Server izvietošanu un lietotāji ir mājās lokāli un tiešsaistē: izpildiet sava Skype darbam Server vadības paneļa sadaļā "Hibrīda iestatīšana ar Teams un **Skype darbam Online"** un pārvietojiet lietotājus tiešsaistē.
