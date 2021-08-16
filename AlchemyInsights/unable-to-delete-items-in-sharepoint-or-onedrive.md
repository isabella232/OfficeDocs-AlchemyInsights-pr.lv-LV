---
title: Nevar izdzēst vienumus programmā SharePoint vai OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038524"
---
# <a name="unable-to-delete-items"></a>Nevar izdzēst vienumus

- Saglabāšanas politiku dēļ var rasties šāda problēma: atspējojiet vai izslēdziet attiecīgo aizturēšanu, kas izraisa šo problēmu. Pēc saglabāšanas politikas vai aizturēšanas noņemšanas var paiet līdz pat 24 stundām, līdz izmaiņas stājas spēkā. Pārliecinieties, vai [vienumam nav saglabāšanas](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) politikas iestatījuma.

- Vietne, iespējams, ir pārsniegusi krātuves ierobežojumu, palielina [vietnes kvotu](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) un izdzēš vienumu.

- Pārliecinieties, vai [vienums nav paņemts](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) citam lietotājam.

- Visbeidzot administratori var izmantot [SharePoint patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), kas satur PowerShell komandu bibliotēku, kas sniedz iespēju veikt sarežģītas pārvaldības darbības, piemēram, likt izdzēst pasaknis vienumus.
- [PNP faila noņemšana](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP mapes noņemšana](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP saraksta elementa noņemšana](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP saraksta noņemšana](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP lauka noņemšana (kolonna)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)