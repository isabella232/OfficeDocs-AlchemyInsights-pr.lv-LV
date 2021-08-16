---
title: Error AttributeValueMustBeUnique
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
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002127"
---
# <a name="error-attributevaluemustbeunique"></a>Kļūda: AttributeValueMustBeUnique

Izplatītākais kļūdas AttributeValueMustBeUnique iemesls ir divi objekti ar atšķirīgu SourceAnchor (immutableId), kuriem ir vienāda ProxyAddresses un/vai UserPrincipalName atribūtu vērtība. Lai novērstu kļūdu AttributeValueMustBeUnique:
  
1. Identificējiet dublētās proxyAddresses, userPrincipalName vai citas atribūta vērtību, kas izraisa kļūdu. Norādiet arī to, kuri divi (vai vairāki) objekti ir iesaistīti konfliktā. Azure AD Savienošana sinhronizācijas darbspējas atskaite var palīdzēt noteikt abus objektus.
    
2. Identificējiet, kuram objektam arī turpmāk jābūt dublētās vērtības vērtībai, bet kuram objektam tā nevajadzētu būt.
    
3. Noņemiet dublēto vērtību no objekta, kam NEVAJADZĒTU būt vērtībai. Ņemiet vērā, ka ir jāveic izmaiņas direktorijā, no kura tiek iegūts objekts. Dažos gadījumos, iespējams, būs jāizdzēš kāds no objektiem, kas konfliktē.
    
4. Ja veicāt izmaiņas lokālajā AD, ļaujiet Azure AD Savienošana sinhronizēt kļūdas izmaiņas, lai tās būtu novērstas.
    

