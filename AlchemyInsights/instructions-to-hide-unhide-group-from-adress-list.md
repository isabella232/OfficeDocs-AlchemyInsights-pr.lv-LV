---
title: Norādījumi par to, kā paslēpt/Parādīt paslēpto grupu no adrešu saraksta
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663016"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="ada78-102">Paslēpt Microsoft 365 grupu no adrešu saraksta (GAL)</span><span class="sxs-lookup"><span data-stu-id="ada78-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="ada78-103">Lai paslēptu Microsoft 365 grupu no adrešu sarakstiem (GAL) no Exchange klientiem (piemēram, Outlook vai OWA), izmantojiet šādu komandu EXO čaulā:</span><span class="sxs-lookup"><span data-stu-id="ada78-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="ada78-104">Lai paslēptu Microsoft 365 grupu, kas ir redzama Exchange klientiem, izmantojiet šādu komandu EXO čaulā:</span><span class="sxs-lookup"><span data-stu-id="ada78-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

