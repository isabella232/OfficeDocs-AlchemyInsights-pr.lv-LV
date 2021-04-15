---
title: Domēna pārbaude
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770998"
---
# <a name="verify-your-domain"></a><span data-ttu-id="dbee8-102">Domēna pārbaude</span><span class="sxs-lookup"><span data-stu-id="dbee8-102">Verify your domain</span></span>

 <span data-ttu-id="dbee8-103">**Iespējams, ka ieraksts nav atjaunināts internetā.**</span><span class="sxs-lookup"><span data-stu-id="dbee8-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="dbee8-104">Parasti nepieciešamas dažas minūtes, lai redzētu jauno ierakstu, taču dažreiz var būt nepieciešamas dažas stundas.</span><span class="sxs-lookup"><span data-stu-id="dbee8-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="dbee8-105">Ja esat gaidījis tik ilgi, vēlreiz pārbaudiet, vai esat nokopjis un ielīmējis precīzu vērtību TXT verifikācijas ierakstā sava DNS viesošanas pakalpojumuā.</span><span class="sxs-lookup"><span data-stu-id="dbee8-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="dbee8-106">Bieži izplatīta problēma ir ieraksta daļas "MS=" neiekšana.</span><span class="sxs-lookup"><span data-stu-id="dbee8-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="dbee8-107">Arī šī ir nepieciešama!</span><span class="sxs-lookup"><span data-stu-id="dbee8-107">We need that too!</span></span>

- <span data-ttu-id="dbee8-108">Dažu DNS viesošanas pakalpojumu serveru vietnēs ir jāveic papildu darbība, lai saglabātu zonas failu (kur tiek glabāts DNS ieraksts), un tas tiek atjaunināts internetā.</span><span class="sxs-lookup"><span data-stu-id="dbee8-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="dbee8-109">Pārliecinieties, vai esat saglabājis izmaiņas, lai Microsoft varētu skatīt un verificēt ierakstu.</span><span class="sxs-lookup"><span data-stu-id="dbee8-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
