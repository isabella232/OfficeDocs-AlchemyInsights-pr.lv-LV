---
title: Lietotāja attēls joprojām tiek Microsoft Teams organizācijas diagrammā
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422250"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Lietotāja attēls joprojām tiek Microsoft Teams organizācijas diagrammā

Ja viena vai vairākas personas jūsu organizācijā ir atspējotas vai noņemtas, un viņu profila fotoattēls joprojām tiek rādīts organizācijas diagrammā, iespējams, **ka ShowInAddressLists iestatījums** ir Aplams: 

1. Dodieties uz Microsoft 365 administrēšanas centrs > [Aktīvie](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) lietotāji un atlasiet lietotāju, kura fotoattēls joprojām tiek rādīts. 
1. Atlasiet cilni **Pasts** un pārliecinieties, vai **iestatījums Rādīt globālajā adrešu sarakstā** ir **nē**.

Ja **showInAddressLists iestatījums** **uz Nē** nedarbojas, pārbaudiet šādus iestatījumus: 

- Lietotājs, iespējams, tiek parādīts no adresātu saraksta Exchange. Papildinformāciju skatiet rakstā [Adrešu sarakstu pārvaldība programmā Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Lietotājs, iespējams, tiek parādīts no adrešu saraksta programmā Azure Active Directory. Papildinformāciju skatiet rakstā [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 