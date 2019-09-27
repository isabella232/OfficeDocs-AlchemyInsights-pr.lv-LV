---
title: Datu atrašanās vieta
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207268"
---
# <a name="data-location"></a>Datu atrašanās vieta

Varat skatīt Office 365 nomnieka atrašanās vietu administrēšanas centrā vai, izveidojot savienojumu ar Exchange Online, izmantojot PowerShell.


**Administrēšanas centrs:**
1. Piesakieties [administrēšanas centrā](https://admin.microsoft.com/Adminportal/Home).
2. Atlasiet vienumu **Iestatījumi** > **organizācijas profils**.
3. Sadaļā **datu atrašanās vieta**atlasiet **Skatīt detalizētu informāciju**.


**Powershell:**
1. Izveidot savienojumu ar Exchange Online, izmantojot programmu Windows PowerShell.
2. Izpildīt [Get OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet, lai parādītu sarakstu ar nomnieka rekvizītus. 
3. Apskatiet rekvizītu OrganizationId.

Ja jums ir EXO un SPO datu atrašanās vieta, varat noteikt datu atrašanās vietu citiem pakalpojumiem, kurus jūs varat izmantot no vietas, [kur atrodas jūsu dati](https://products.office.com/where-is-your-data-located).