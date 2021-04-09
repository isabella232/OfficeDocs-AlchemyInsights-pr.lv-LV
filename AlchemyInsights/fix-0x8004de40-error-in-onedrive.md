---
title: Pakalpojuma 0x8004de40 labošana pakalpojumā OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649755"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Pakalpojuma 0x8004de40 labošana pakalpojumā OneDrive

Ja jūsu datorā darbojas sistēma Windows 7 un tiek parādīta šī kļūda, atjauniniet, lai iespējotu [TLS 1.1 un TLS 1.2 kā noklusējuma drošos protokolus sistēmā WinHTTP sistēmā Windows.](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Ja datorā darbojas operētājsistēma Windows 10 un saņemat kļūdas 0x8004de40 saistībā ar OneDrive:

- Restartējiet ietekmēto datoru, kamēr ir izveidots savienojums ar pakalpojuma Acitve direktorija domēnu.
- Ja atkārtota palaišana nenovērš problēmu, atkārtoti pievienojiet ierīci no Azure AD. 

**Piezīme.** Jums ir jābūt korporatīvajā tīklā, veicot šīs darbības. Neveiciet šīs darbības, ja neesat izveidojis savienojumu ar savu korporatīvo infrastruktūru (piemēram, atrodoties braucot). 

1. Atveriet priviliģētu komandu uzvedni, atlasot **Sākums**, ar peles labo **pogu** noklikšķiniet uz Komandu uzvedne un pēc tam atlasiet Palaist **kā administratoram.**

1. Ierakstiet *dsregcmd /leave un* nospiediet taustiņu **Enter.**

1. Kad tas ir pabeigts, *ierakstiet dsregcmd /join un* nospiediet taustiņu **Enter.**

1. Kad esat pabeidzis, aizveriet komandu uzvedni.

1. Restartējiet datoru un piesakieties pakalpojumā OneDrive.