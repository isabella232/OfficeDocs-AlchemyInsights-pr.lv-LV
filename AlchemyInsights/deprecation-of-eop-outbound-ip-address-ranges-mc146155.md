---
title: 1065 izstāšanās no EOP izejošā IP adreses rangesMC146155
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
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806802"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Izejošo IP adrešu diapazonu EOP novecošana

Mēs esam noteikuši potenciālu problēmu ar jūsu organizāciju, kas (ja nav novērsta ar 26. oktobri, 2018), var sadalīt pasta plūsmu uz jūsu lokāliem vai ārējiem galamērķiem. Kā iepriekš paziņots, lai vienkāršotu IP adrešu diapazona pārvaldību, mēs esam konsolidējuši Exchange Online Protection (EOP) IP adrešu diapazonus, kas tiek izmantoti, lai sūtītu un saņemtu e-pastu ārpus Microsoft 365. Mūsu analīze norāda, ka vienu vai vairākus ārējos e-pasta avotus vai adresātus, kas ir konfigurēti pasta plūsmas savienotājiem, neakceptē savienojumus no [šeit](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)parādītajiem IP adrešu diapazoniem.

Act pirms 26. oktobra, lai nodrošinātu, ka šie avoti un galamērķi pieņems savienojumus uz un no visām [publicētajām EOP IP adresēm](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Papildinformāciju par šīm izmaiņām skatiet rakstā ziņojumu centra ziņas [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)vai [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Piezīme**. Ja iepriekš izmantojāt IP vai vietrāža URL publicēšanu, izmantojot HTML, XML un RSS galapunktu atjauninājumus, jums jāmigrē arī uz jaunajiem tīmekļa pakalpojumiem, lai automatizētu šos atjauninājumu tipus. Lai iegūtu papildinformāciju, skatiet rakstu [microsoft 365 galapunkta kategorijas un Microsoft 365 IP adrese un URL tīmekļa pakalpojums](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
