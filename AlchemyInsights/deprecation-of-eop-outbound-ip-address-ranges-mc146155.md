---
title: 1065 deprecation EOP izejošo IP adresi rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704604"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Izslēgšanas EOP izejošo IP adrešu diapazoni

Mēs esam konstatējis potenciālo problēmu ar jūsu organizāciju, kas (ja nav labots līdz 26 oktobris, 2018) var pārtraukt pasta plūsmu uz jūsu lokālo vai ārējiem galamērķiem. Kā iepriekš paziņots, lai vienkāršotu IP adrešu diapazona pārvaldību, mēs esam konsolidējot Exchange Online Protection (EOP) IP adrešu diapazonu, kas tiek izmantoti, lai nosūtītu un saņemtu e-pastu ārpus Microsoft 365. Mūsu analīze norāda, ka viens vai vairāki no ārējiem e-pasta avotiem vai galamērķiem, ko esat konfigurējis pasta plūsmas savienojumos, nepieņem savienojumus no [šeit](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)parādītā IP adrešu diapazona.

Act pirms oktobris 26, lai nodrošinātu, ka šie avoti un galamērķi pieņems savienojumus uz un no visām [publicētajām EOP IP adresēm](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Lai iegūtu papildinformāciju par šīm izmaiņām, lūdzu, skatiet ziņu centra ziņas [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)vai [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Piezīme**: ja iepriekš izmantojāt IP vai URL publicēšana, izmantojot HTML, XML un RSS galapunkta atjauninājumus, jums ir arī migrēt uz jauno Web pakalpojumu automatizēšana šāda veida atjauninājumus. Lai iegūtu papildinformāciju, skatiet [microsoft 365 galapunkta kategorijas un microsoft 365 IP adresi un URL tīmekļa pakalpojumu](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
