---
title: PowerShell izmantošana politiku koplietošanai un organizācijas attiecībām.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709473"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="806a4-102">PowerShell izmantošana politiku koplietošanai un organizācijas attiecībām.</span><span class="sxs-lookup"><span data-stu-id="806a4-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="806a4-103">Attiecībā uz organizācijas attiecībām, lūdzu, pārskatiet detalizētu sintaksi un parametru informāciju par: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  UN  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="806a4-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="806a4-104">Lai izveidotu koplietošanas politiku, izmantojiet [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="806a4-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="806a4-105">Lai  [lietotu koplietošanas politiku pastkastei vai lietotājam](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  jāizmanto  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) un [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) kombinācija ar jaunizveidoto politiku.</span><span class="sxs-lookup"><span data-stu-id="806a4-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="806a4-106">Lai  [modificētu, atspējotu vai noņemtu koplietošanas politiku](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  ir jāizmanto  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) un [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="806a4-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="806a4-107">**Lai pilnībā izprastu šo tēmu, lūdzu, izlasiet:**</span><span class="sxs-lookup"><span data-stu-id="806a4-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="806a4-108">Koplietošana pakalpojumā Exchange Online</span><span class="sxs-lookup"><span data-stu-id="806a4-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)