---
title: 1554 Winsock kļūda 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7651effc43cb0c4bc2fbbe5349bb72303943f493
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859147"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="9d6d7-102">Winsock kļūda 10061</span><span class="sxs-lookup"><span data-stu-id="9d6d7-102">Winsock error 10061</span></span>

<span data-ttu-id="9d6d7-103">Šo kļūdas kodu, nozīmē, ka Office 365 nevarētu izveidot TCP ligzda (savienojums) ar mērķa resursdatoru.</span><span class="sxs-lookup"><span data-stu-id="9d6d7-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="9d6d7-104">Visdrīzāk, ka cēlonis šīs kļūdas ir ar ugunsmūra konfigurāciju saistīta problēma.</span><span class="sxs-lookup"><span data-stu-id="9d6d7-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="9d6d7-105">Lai novērstu problēmu, pārbaudiet šos iestatījumus:</span><span class="sxs-lookup"><span data-stu-id="9d6d7-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="9d6d7-106">Pārbaudiet, vai jūsu ugunsmūra konfigurēšanu ar informāciju, kas atrodas [Office 365 URL un IP adrešu diapazons](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="9d6d7-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="9d6d7-107">Ja kļūda ir specifiski uz Exchange Online aizsardzība (EOP), jums vajadzētu ir iepriekš paziņots [Exchange Online aizsardzība IP adreses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)maiņa.</span><span class="sxs-lookup"><span data-stu-id="9d6d7-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="9d6d7-108">Pārliecinieties, ka jūsu interneta pakalpojumu sniedzēja (ISP) nav bloķē portu.</span><span class="sxs-lookup"><span data-stu-id="9d6d7-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="9d6d7-109">Pārbaudiet, vai gudrs uzņēmējas un mērķa servera uzstādījumus jūsu savienotāji.</span><span class="sxs-lookup"><span data-stu-id="9d6d7-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="9d6d7-110">Ievērojiet, ka Office 365 nav bloķēt *ienākošos* savienojumus šādā veidā.</span><span class="sxs-lookup"><span data-stu-id="9d6d7-110">Note that Office 365 doesn't block *incoming* connections in this manner.</span></span>
