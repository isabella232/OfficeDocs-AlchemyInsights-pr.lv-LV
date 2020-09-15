---
title: 1554 Winsock kļūda 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698869"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="e53ec-102">Winsock kļūda 10061</span><span class="sxs-lookup"><span data-stu-id="e53ec-102">Winsock error 10061</span></span>

<span data-ttu-id="e53ec-103">Šis kļūdas kods nozīmē, ka Microsoft nevar izveidot TCP ligzdu (savienojumu) ar mērķi resursdators.</span><span class="sxs-lookup"><span data-stu-id="e53ec-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="e53ec-104">Visticamāk, šīs kļūdas cēlonis ir problēmas ar ugunsmūra konfigurāciju.</span><span class="sxs-lookup"><span data-stu-id="e53ec-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="e53ec-105">Lai novērstu šo problēmu, pārbaudiet šos iestatījumus:</span><span class="sxs-lookup"><span data-stu-id="e53ec-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="e53ec-106">Ugunsmūra konfigurācijas pārbaudīšana, izmantojot informāciju [Microsoft 365 vietrāžus URL un IP adrešu diapazonos](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="e53ec-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="e53ec-107">Ja kļūda ir specifiska Exchange Online Protection (EOP), jums ir iepriekš jāziņo par izmaiņām [Exchange Online Protection IP adresēs](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="e53ec-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="e53ec-108">Pārbaudiet, vai jūsu interneta pakalpojumu sniedzējs (ISP) nebloķē portu.</span><span class="sxs-lookup"><span data-stu-id="e53ec-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="e53ec-109">Pārliecinieties, vai jūsu savienotājiem ir gudri resursdators un mērķserveri iestatījumi.</span><span class="sxs-lookup"><span data-stu-id="e53ec-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="e53ec-110">Ņemiet vērā, ka Microsoft 365 nebloķē *ienākošos* savienojumus šādā veidā.</span><span class="sxs-lookup"><span data-stu-id="e53ec-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
