---
title: PowerShell izmantošana politiku koplietošanai un organizācijas attiecībām.
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 9c52b876160f9577e6cefe7644c29d6fdf3b23fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826062"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>PowerShell izmantošana politiku koplietošanai un organizācijas attiecībām.


Attiecībā uz organizācijas attiecībām, lūdzu, pārskatiet detalizētu sintaksi un parametru informāciju par: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  UN  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Lai izveidotu koplietošanas politiku, izmantojiet [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Lai  [lietotu koplietošanas politiku pastkastei vai lietotājam](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  jāizmanto  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) un [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) kombinācija ar jaunizveidoto politiku. Lai  [modificētu, atspējotu vai noņemtu koplietošanas politiku](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  ir jāizmanto  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) un [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Lai pilnībā izprastu šo tēmu, lūdzu, izlasiet:**

[Koplietošana pakalpojumā Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)