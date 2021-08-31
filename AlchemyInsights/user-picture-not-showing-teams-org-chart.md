---
title: User picture not showing in Microsoft Teams organization chart
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792758"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>User picture not showing in Microsoft Teams organization chart

Ja vienai vai vairākām personām jūsu organizācijā trūkst profila fotoattēla organizācijas diagrammā, iespējams, **ka iestatījums ShowInAddressLists** ir iestatīts uz **Aplams:**

1. Dodieties uz Microsoft 365 administrēšanas centrs > [**Aktīvie lietotāji**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)un atlasiet lietotāju, kurā trūkst fotoattēla. 
1. Atlasiet cilni **Pasts** un pārliecinieties, vai **iestatījums Rādīt globālajā adrešu** sarakstā ir **jā.** 

Ja **ShowInAddressLists iestatījums** **uz Jā** nedarbojas, pārbaudiet šādus iestatījumus:

- Iespējams, lietotājs ir paslēpts no adresātu saraksta programmā Exchange. Papildinformāciju skatiet rakstā [Adrešu sarakstu pārvaldība programmā Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Iespējams, lietotājs ir paslēpts no adrešu saraksta programmā Azure Active Directory. Papildinformāciju skatiet rakstā [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
