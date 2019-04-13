---
title: 1065 EOP izslēgšanas izejošo IP adresi rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 17beb1722142d94ea05b67ce5ed1f20f8b11375c
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858103"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>EOP izejošo IP adresi diapazoni izslēgšanas

Mēs esam atklāti potenciālu problēmu ar savu organizāciju, kas (ja netiek laboti ar oktobrī 26, 2018) nepārtrūks pasta plūsma uz lokālajiem vai ārējiem mērķiem. Kā iepriekš paziņota, vienkāršot IP adrešu diapazona vadību, mēs konsolidēšana Exchange Online aizsardzība (EOP) IP adrese diapazonus, ko izmanto, lai nosūtītu un saņemtu e-pastu ārpus biroja 365. Mūsu analīze liecina, ka vienai vai vairākām no ārējiem e-pasta avotu vai galamērķiem, pasta plūsmas savienotāji konfigurētajā nav akceptēt savienojumus no IP adrešu diapazonu parādīts [šeit](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Darboties pirms oktobris 26, lai nodrošinātu šos avotus un galamērķiem tiks akceptēšanai un no visiem [publicēts EOP IP adreses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Plašāku informāciju par šo izmaiņu, lūdzu, skatiet ziņojumu centra amatu, [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)vai [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Piezīme**: ja iepriekš izmantojāt IP vai URL publicēšana, izmantojot HTML, XML un RSS galapunkta atjauninājumus, jums arī vajadzētu pāriet uz jaunajos web pakalpojumos, automatizējot šo atjauninājumu tipiem. Lai iegūtu papildinformāciju, skatiet [Office 365 IP adrese un biroja 365 galapunkta kategorijām un URL web pakalpojums](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
