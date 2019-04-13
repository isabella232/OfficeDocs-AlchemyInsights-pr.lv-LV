---
title: 761 veido savienojumu ar Exchange Online PowerShell MFA ir iespējota
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 4/26/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 761
ms.assetid: 9b0b89e3-d1d7-4e4d-93de-bb4cd00904d8
ms.openlocfilehash: d9c4195ba3079d35f7a556b91ea6d7318efb35cb
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859543"
---
# <a name="connect-to-exchange-online-powershell-when-mfa-is-enabled"></a><span data-ttu-id="63aa4-102">Izveidot savienojumu ar Exchange Online PowerShell MFA ir iespējota</span><span class="sxs-lookup"><span data-stu-id="63aa4-102">Connect to Exchange Online PowerShell when MFA is enabled</span></span>

<span data-ttu-id="63aa4-103">Ja jūsu kontam ir vairāku faktoru autentifikaciju (MFA) iespējota, jums nepieciešams ievērot šos norādījumus, lai izveidotu savienojumu ar Exchange Online PowerShell: [Exchange Online PowerShell savienojuma izveide, izmantojot vairāku faktoru autentifikaciju](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="63aa4-103">If your account has multi-factor authentication (MFA) enabled, you need to follow these instructions to connect to Exchange Online PowerShell: [Connect to Exchange Online PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell).</span></span>

<span data-ttu-id="63aa4-104">**Piezīme**: pat, ja jūs esat pieslēdzies Exchange Online PowerShell pagātnē, izmantojot [regulāras savienojuma instrukcijas](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell), jums vajadzēs izmantot MFA savienojuma instrukcijas, pēc tam, kad jūsu konts ir iespējots MFA.</span><span class="sxs-lookup"><span data-stu-id="63aa4-104">**Note**: Even if you've connected to Exchange Online PowerShell in the past using [the regular connection instructions](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell), you need to use the MFA connection instructions after MFA has been enabled for your account.</span></span>
