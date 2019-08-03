---
title: Problēmas ar MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250172"
---
# <a name="issues-with-mfa"></a>Problēmas ar MFA
Ir pāris lietas, lai pārbaudītu, ja lietotāji nevar reģistrēties sistēmā, izmantojot vairāku faktoru autentifikaciju (MFA)

1. Skarto lietotāju var tikt bloķēta Azure Active Directory portālā. Ja tas tā ir gadījumā, autentifikācijas mēģinājumus, ka konkrētu lietotāju būs automātiski noraidīja. [Lūdzu izpildiet šajā pantā atbloķēt tos.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ja atbloķēšanas lietotājam nepalīdzēja vai nav bloķēts lietotājs jūs varat mēģināt atiestatīt lietotāja MFA un viņi iet cauri procesam enroll atkal. [Lūdzu, izpildiet šajā rakstā aprakstītie soļi.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ja šī ir pirmā reize, kad ļāva MFA un lietotāji nevarat ieiet bez pārlūkprogrammas klientiem, piemēram, Outlook, Skype u.c., varbūt ADAL (aktīvajā direktorijā autentifikācijas bibliotēka) nav iespējota O365 abonementu. Šajā gadījumā jums būs nepieciešams pieslēgties Exchange Online Powershell un palaist šo cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*