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
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7b98b68fabff6c048f1bab6cf506355114d18658
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916531"
---
# <a name="error-attributevaluemustbeunique"></a>Kļūda: AttributeValueMustBeUnique

AttributeValueMustBeUnique kļūdas visbiežāk iemesls ir divi objekti ar dažādu SourceAnchor (immutableId) ir tāda pati vērtība atribūtu ProxyAddresses un/vai UserPrincipalName. Lai izlabotu kļūdu AttributeValueMustBeUnique:
  
1. Identificētu dublicētās proxyAddresses, userPrincipalName vai citus atribūta vērtībai, kas izraisa kļūdu. Arī noteikt, kādi divas (vai vairāk) objekti ir iesaistītas konfliktā. Atskaiti, kas rada veselības Azure AD savienotu sinhronizācijai var palīdzēt identificēt divus objektus.
    
2. Noteikt, kuru objektu turpmāk vajadzētu būt dublicētās vērtības un kuru objektu nevajadzētu būt.
    
3. Noņemiet objektu, kuram nav jābūt šo vērtību dublicētās vērtības. Ņemiet vērā, ka direktoriju, kurā objekts tiek iegūts no būtu jāveic izmaiņas. Dažos gadījumos, var rasties nepieciešamība dzēst kādu no objektiem konfliktā.
    
4. Ja veicāt izmaiņas par AD telpās, ļaujiet Azure AD pievienot sinhronizācijas kļūdu saņemt fiksētu izmaiņu.
    

