---
title: Kļūdas AttributeValueMustBeUnique
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
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709158"
---
# <a name="error-attributevaluemustbeunique"></a>Kļūda: AttributeValueMustBeUnique

Biežāk sastopamais AttributeValueMustBeUnique kļūdas iemesls ir divi objekti ar atšķirīgu SourceAnchor (immutableId) ir tāda pati vērtība attiecībā uz ProxyAddresses un/vai UserPrincipalName atribūtiem. Lai izlabotu AttributeValueMustBeUnique kļūdu:
  
1. Identificējiet dublēto proxyAddresses, userPrincipalName vai citu atribūta vērtību, kas izraisa kļūdu. Arī Identificējiet, kuri divi (vai vairāki) objekti ir iesaistīti konfliktā. Azure AD Connect Health sinhronizēšanai ģenerētā atskaite var palīdzēt noteikt divus objektus.
    
2. Identificējiet, kuram objektam jāturpina dublētā vērtība un kuru objektu nelietot.
    
3. Noņemiet dublēto vērtību no objekta, kuram nav šīs vērtības. Ņemiet vērā, ka ir jāveic izmaiņas direktorijā, no kuras ir avots objekts. Dažos gadījumos, iespējams, ir jādzēš viens no konfliktējošajiem objektiem.
    
4. Ja veicāt izmaiņas lokālajā REKLĀMā, ļaujiet pakalpojumam Azure AD Connect sinhronizēt izmaiņas kļūdas novēršanai.
    

