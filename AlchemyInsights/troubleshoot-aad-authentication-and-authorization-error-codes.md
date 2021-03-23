---
title: Azure AD autentifikācijas un autorizācijas (AADSTS) kļūdu kodu problēmu novēršana
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036509"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Azure AD autentifikācijas un autorizācijas (AADSTS) kļūdu kodu problēmu novēršana

Lai atrisinātu AAD autentifikāciju un autorizācijas kļūdu kodus (AADSTS), veiciet tālāk norādītās ieteicamās darbības.

1. **Kļūdu kodu apstrāde lietojumprogrammā**

- Ar **OAuth 2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2 sniedz norādījumus par to, kā apstrādāt kļūdas, veicot autentifikāciju, izmantojot kļūdu atbildes kļūdas daļu.

    - **kļūda**: kļūdas koda virkne, ko var izmantot, lai klasificētu kļūdu tipus, kas rodas, un ir jāizmanto, lai reaģētu uz kļūdām.
    - **Kļūdas** laukam ir vairākas iespējamās vērtības — pārskatiet protokola dokumentācijas saites un OAuth 2,0 specs, lai iegūtu papildinformāciju par konkrētām kļūdām un to, kā tās reaģēt.

- Šeit redzama kļūdas atbilde piemērs:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Uzmeklēšanas pašreizējā kļūdas koda informācija**

- Kļūdu kodi un ziņojumi var tikt mainīti. Jaunāko informāciju skatiet https://login.microsoftonline.com/error lapā, lai atrastu AADSTS kļūdu aprakstus, labojumus un dažus ieteicamos risinājumus.
- Varat arī meklēt un novērst [AADSTS kļūdu kodus](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) , kas norādīti rakstā [Azure AD autentifikācijas un autorizācijas kļūdu kodi](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).

3. **Palīdzības saņemšana**

- [Atbalsta un palīdzības opcijas izstrādātājiem](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) — ja jums ir nepieciešams atbildēt uz jautājumu vai palīdzēt atrisināt problēmu, kas nav iekļauta mūsu dokumentācijā, iespējams, ir pienācis laiks sazināties ar ekspertiem, lai saņemtu palīdzību. Šajā rakstā ir sniegti vairāki ieteikumi, kā saņemt atbildes uz jautājumiem par to, kā izveidot lietojumprogrammas, kas ir integrētas ar Microsoft identitātes platformu.








