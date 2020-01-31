---
title: Nevar dzēst vienumus SharePoint vai OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571272"
---
# <a name="unable-to-delete-items"></a>Nevar izdzēst objektus

Saglabāšanas politikas var izraisīt šo, jums ir atspējota vai izslēgt attiecīgo aizturēšanu, kas izraisa šo problēmu. Pēc saglabāšanas politika vai aizturēšana ir noņemta, var ilgt līdz 24 stundām izmaiņas stātos spēkā. Pārliecinieties, vai krājumam nav [saglabāšanas politikas](https://docs.microsoft.com/office365/securitycompliance/retention-policies) iestatījuma.

Iespējams, ka vietne ir pārsniegusi krātuves ierobežojumu, palielina [vietnes kvotu](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) un dzēš vienumu.

Pārliecinieties, vai vienums nav [paņemts](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) citam lietotājam.

Visbeidzot, administratori var izmantot [SharePoint modeļus un praksi](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP), kurā ir PowerShell komandu bibliotēka, kas ļauj veikt sarežģītas pārvaldības darbības, piemēram, Force dzēšot spītīgs vienumus.
- [PNP faila noņemšana](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Noņemt PNP mapi](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Noņemt PNP saraksta vienumu](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Noņemt PNP sarakstu](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Noņemt PNP lauku (kolonna)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)