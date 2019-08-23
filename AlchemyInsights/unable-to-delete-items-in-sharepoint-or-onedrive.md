---
title: Nevar izdzēst vienumus SharePoint vai OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: b25e6d144dcefcfed4258e78ad5cfd4089ba7d1e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558660"
---
# <a name="unable-to-delete-items"></a>Nevar izdzēst vienumus

Problēmas, dzēšot vienumus SharePoint?

- Vienmēr pārliecinieties, vai jums ir [atbilstošas atļaujas](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) dzēst vienumu vai [vietņu kolekcijas administrators](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) mēģinājums noņemt vienumu.

- Nodrošina to, ka nenotiek [saglabāšanas politiku](https://docs.microsoft.com/office365/securitycompliance/retention-policies) iestatīšana krājumam.

- Nodrošinātu, ka prece nav [paņēmis](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) cits lietotājs.

- Visbeidzot, administratori var izmantot [SharePoint modeļus un praksi](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) kas atrodas bibliotēka PowerShell komandu, kas ļauj jums veikt sarežģītas vadības rīcība, piemēram, piespiest spītīgs vienumu dzēšana.
- [Noņemt failu PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Noņemt mapi PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP saraksta vienuma noņemšana](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Noņemt PNP sarakstu](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Noņemt PNP laukā (kolonnā)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)