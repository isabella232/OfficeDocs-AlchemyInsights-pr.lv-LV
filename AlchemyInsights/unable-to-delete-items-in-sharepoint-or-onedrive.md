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
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049524"
---
# <a name="unable-to-delete-items"></a>Nevar izdzēst objektus

Radušās problēmas, dzēšot SharePoint vienumus?

- Vienmēr pārliecinieties, vai jums ir [atbilstošās atļaujas](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) dzēst vienumu vai [vietņu kolekcijas administratora](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) mēģinājums noņemt vienumu.

- Pārliecinieties, vai krājumam nav [saglabāšanas politikas](https://docs.microsoft.com/office365/securitycompliance/retention-policies) iestatījuma.

- Pārliecinieties, vai vienums nav [paņemts](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) citam lietotājam.

- Visbeidzot, administratori var izmantot [SharePoint modeļus un praksi](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP), kurā ir PowerShell komandu bibliotēka, kas ļauj veikt sarežģītas pārvaldības darbības, piemēram, Force dzēšot spītīgs vienumus.
- [PNP faila noņemšana](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Noņemt PNP mapi](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Noņemt PNP saraksta vienumu](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Noņemt PNP sarakstu](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Noņemt PNP lauku (kolonna)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)