---
title: Starpniekservera adreses kļūda koplietojamas pastkastes izveides laikā
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568297"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="17526-102">Starpniekservera adreses kļūda, veidojot pastkasti vai citu e-pasta objektu</span><span class="sxs-lookup"><span data-stu-id="17526-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="17526-103">Ja mēģinājāt izveidot e-pasta objektu (pastkaste, koplietojama pastkaste utt.) un tiek parādīts kļūdas ziņojums "starpniekservera adrese" SMTP:alias@domain.com "jau tiek izmantota...", jūsu izvēlētajā e-pasta adresē jau ir cits e-pasta objekts jūsu organizācijā.</span><span class="sxs-lookup"><span data-stu-id="17526-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="17526-104">Jums ir jāatrod lietotāja, grupas, koplietojamas pastkastes vai publiskas mapes, kurā ir šī e-pasta adrese, vai jādzēš tā vai jāmaina tās e-pasta adrese.</span><span class="sxs-lookup"><span data-stu-id="17526-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="17526-105">Pēc tam varat izveidot jaunu e-pasta objektu ar atbrīvoto e-pasta adresi.</span><span class="sxs-lookup"><span data-stu-id="17526-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="17526-106">Lai to atrastu, sākumlapā izmantojiet meklēšanu.</span><span class="sxs-lookup"><span data-stu-id="17526-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="17526-107">Varat arī izmantot šādu komandu Exchange Online PowerShell, lai to meklētu:</span><span class="sxs-lookup"><span data-stu-id="17526-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="17526-108">Ja nevēlaties dzēst esošo e-pasta adresi, izvēlieties jaunu e-pasta adresi jaunajam objektam, ko veidojat.</span><span class="sxs-lookup"><span data-stu-id="17526-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  