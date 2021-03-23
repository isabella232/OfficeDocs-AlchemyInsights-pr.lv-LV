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
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="0df70-102">Azure AD autentifikācijas un autorizācijas (AADSTS) kļūdu kodu problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="0df70-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="0df70-103">Lai atrisinātu AAD autentifikāciju un autorizācijas kļūdu kodus (AADSTS), veiciet tālāk norādītās ieteicamās darbības.</span><span class="sxs-lookup"><span data-stu-id="0df70-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="0df70-104">**Kļūdu kodu apstrāde lietojumprogrammā**</span><span class="sxs-lookup"><span data-stu-id="0df70-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="0df70-105">Ar **OAuth 2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2 sniedz norādījumus par to, kā apstrādāt kļūdas, veicot autentifikāciju, izmantojot kļūdu atbildes kļūdas daļu.</span><span class="sxs-lookup"><span data-stu-id="0df70-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="0df70-106">**kļūda**: kļūdas koda virkne, ko var izmantot, lai klasificētu kļūdu tipus, kas rodas, un ir jāizmanto, lai reaģētu uz kļūdām.</span><span class="sxs-lookup"><span data-stu-id="0df70-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="0df70-107">**Kļūdas** laukam ir vairākas iespējamās vērtības — pārskatiet protokola dokumentācijas saites un OAuth 2,0 specs, lai iegūtu papildinformāciju par konkrētām kļūdām un to, kā tās reaģēt.</span><span class="sxs-lookup"><span data-stu-id="0df70-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="0df70-108">Šeit redzama kļūdas atbilde piemērs:</span><span class="sxs-lookup"><span data-stu-id="0df70-108">Here is a sample error response:</span></span>
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
2. <span data-ttu-id="0df70-109">**Uzmeklēšanas pašreizējā kļūdas koda informācija**</span><span class="sxs-lookup"><span data-stu-id="0df70-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="0df70-110">Kļūdu kodi un ziņojumi var tikt mainīti.</span><span class="sxs-lookup"><span data-stu-id="0df70-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="0df70-111">Jaunāko informāciju skatiet https://login.microsoftonline.com/error lapā, lai atrastu AADSTS kļūdu aprakstus, labojumus un dažus ieteicamos risinājumus.</span><span class="sxs-lookup"><span data-stu-id="0df70-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="0df70-112">Varat arī meklēt un novērst [AADSTS kļūdu kodus](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) , kas norādīti rakstā [Azure AD autentifikācijas un autorizācijas kļūdu kodi](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span><span class="sxs-lookup"><span data-stu-id="0df70-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="0df70-113">**Palīdzības saņemšana**</span><span class="sxs-lookup"><span data-stu-id="0df70-113">**Get Help**</span></span>

- <span data-ttu-id="0df70-114">[Atbalsta un palīdzības opcijas izstrādātājiem](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) — ja jums ir nepieciešams atbildēt uz jautājumu vai palīdzēt atrisināt problēmu, kas nav iekļauta mūsu dokumentācijā, iespējams, ir pienācis laiks sazināties ar ekspertiem, lai saņemtu palīdzību.</span><span class="sxs-lookup"><span data-stu-id="0df70-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="0df70-115">Šajā rakstā ir sniegti vairāki ieteikumi, kā saņemt atbildes uz jautājumiem par to, kā izveidot lietojumprogrammas, kas ir integrētas ar Microsoft identitātes platformu.</span><span class="sxs-lookup"><span data-stu-id="0df70-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








