---
title: 1065 EOP izejošā IP adrešu diapazona novecošanaMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031269"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>EOP izejošo IP adrešu diapazonu novecošana

Ir konstatēta potenciāla problēma jūsu organizācijā, kas (ja 2018. gada 26. oktobris nav izlabojusi) var izraisīt pasta plūsmas pārtraukumu jūsu lokālajā vai ārējā galamērķī. Kā paziņots iepriekš, lai vienkāršotu IP adrešu diapazonu pārvaldību, mēs apvienojam Exchange Online Protection (EOP) IP adrešu diapazonus, kas tiek izmantoti, lai sūtītu un saņemtu e-pastu ārpus Microsoft 365. Mūsu analīze norāda, ka viens vai vairāki ārēji e-pasta avoti vai galamērķi, kurus esat konfigurējis pasta plūsmas savienotājos, nepieņem savienojumus no šeit parādītajiem IP adrešu [diapazoniem.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Rīkojieties līdz 26. oktobrim, lai nodrošinātu, ka šie avoti un galamērķi akceptēs savienojumus ar visām publicētām [EOP IP adresēm](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)un no tām.

Papildinformāciju par izmaiņām skatiet rakstā Ziņojumu centra ziņas [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)vai [MC149274.](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**Piezīme.** Ja galapunktu atjauninājumiem iepriekš izmantojāt IP vai URL publicēšanu, izmantojot HTML, XML un RSS, jums ir jāmigrē arī uz jaunajiem tīmekļa pakalpojumiem, lai automatizētu šāda veida atjauninājumus. Papildinformāciju skatiet rakstā [Microsoft 365 kategoriju un IP Microsoft 365 URL tīmekļa pakalpojuma informācija.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
