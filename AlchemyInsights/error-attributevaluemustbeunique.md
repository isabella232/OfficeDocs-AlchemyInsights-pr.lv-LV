---
title: Kļūda AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/18/2019
ms.locfileid: "36527020"
---
# <a name="error-attributevaluemustbeunique"></a>Kļūda: AttributeValueMustBeUnique

Visbiežāk iemesls AttributeValueMustBeUnique kļūda ir divi objekti ar citu SourceAnchor (immutableId) ir tāda pati vērtība ProxyAddresses un/vai UserPrincipalName atribūtus. Lai labotu AttributeValueMustBeUnique kļūdu:
  
1. Identificējiet dublikātu proxyAddresses, userPrincipalName vai citu atribūta vērtība, kas izraisa kļūdu. Arī noteikt, kuri divi (vai vairāk) objekti ir iesaistīti konfliktā. Azure AD Connect veselības sinhronizācijas ģenerēts ziņojums var palīdzēt identificēt divus objektus.
    
2. Noteikt, kurš objekts ir jāturpina dublēt vērtību un kuru objektu nedrīkst.
    
3. Noņemiet dublēto vērtību no objekta, kuram nav šī vērtība. Ņemiet vērā, ka ir jāveic izmaiņas direktorijā, no kurienes tiek iegūts objekts. Dažos gadījumos, iespējams, būs jādzēš viens no konflikta objektiem.
    
4. Ja veicāt izmaiņas telpās AD, ļaujiet Azure AD savienojumu sinhronizēt izmaiņas kļūdas iegūt fiksētu.
    

