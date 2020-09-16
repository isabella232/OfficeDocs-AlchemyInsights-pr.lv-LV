---
title: Sava domēna pārbaude
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734313"
---
# <a name="verify-your-domain"></a><span data-ttu-id="52beb-102">Sava domēna pārbaude</span><span class="sxs-lookup"><span data-stu-id="52beb-102">Verify your domain</span></span>

 <span data-ttu-id="52beb-103">**Ieraksts, iespējams, nav atjaunināts internetā.**</span><span class="sxs-lookup"><span data-stu-id="52beb-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="52beb-104">Parasti ir nepieciešamas tikai dažas minūtes, lai mēs varētu redzēt jauno ierakstu, taču reizēm tas var aizņemt vairākas stundas.</span><span class="sxs-lookup"><span data-stu-id="52beb-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="52beb-105">Ja jau ilgi gaidījāt, ka esat to izdarījis, vēlreiz pārbaudiet, vai esat nokopējis un ielīmējis precīzu vērtību TXT verifikācijas ierakstā pie sava DNS viesošanas pakalpojumu sniedzēja.</span><span class="sxs-lookup"><span data-stu-id="52beb-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="52beb-106">Viens no bieži sastopamajiem jautājumiem neiekļauj ieraksta daļu "MS =".</span><span class="sxs-lookup"><span data-stu-id="52beb-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="52beb-107">Arī mums tas ir jādara!</span><span class="sxs-lookup"><span data-stu-id="52beb-107">We need that too!</span></span>

- <span data-ttu-id="52beb-108">Dažos DNS resursdatoros ir jāveic papildu darbības, lai saglabātu zonas failu (kurā ir saglabāts DNS ieraksts) un tas tiks atjaunināts visā internetā.</span><span class="sxs-lookup"><span data-stu-id="52beb-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="52beb-109">Pārliecinieties, vai esat saglabājis izmaiņas, lai Microsoft varētu redzēt un verificēt ierakstu.</span><span class="sxs-lookup"><span data-stu-id="52beb-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
