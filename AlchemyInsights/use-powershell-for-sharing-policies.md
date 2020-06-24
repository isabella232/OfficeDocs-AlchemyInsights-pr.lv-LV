---
title: PowerShell izmantošana politiku un organizācijas attiecību koplietošanai
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862090"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>PowerShell izmantošana politiku un organizācijas attiecību koplietošanai


Attiecībā uz organizācijas attiecībām, lūdzu, pārskatiet detalizētu sintaksi un parametru informāciju: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) and [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Lai izveidotu koplietošanas politiku , [izmantojiet New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Lai [lietotu koplietošanas politiku pastkastei vai lietotājam,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) ir jāizmanto [set-mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) un [Get-Mailbox kombinācija](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) ar jaunizveidoto politiku. Lai [modificētu, atspējotu vai noņemtu koplietošanas politiku,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) jāizmanto [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) un [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Lai iegūtu pilnīgu izpratni par šo tēmu, lūdzu, izlasiet:**

[Koplietošana pakalpojumā Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)