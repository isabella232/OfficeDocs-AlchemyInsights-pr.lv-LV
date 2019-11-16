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
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768844"
---
# <a name="issues-with-azure-mfa"></a>Problēmas ar Azure MFA
Ir dažas lietas, lai pārbaudītu, ja lietotāji nevar pieteikties, izmantojot vairāku faktoru autentifikācijas (MFA)

1. Ietekmēto lietotāju var bloķēt Azure Active Directory portālā. Šādā gadījumā automātiski tiek liegta autentifikācijas mēģinājumi šim konkrētam lietotājam. [Lūdzu, veiciet šajā rakstā aprakstītās darbības, lai atbloķētu tos.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ja atbloķēšanas lietotāja nepalīdzēja vai lietotājs nav bloķēts varat mēģināt atiestatīt MFA par lietotāju, un viņi iet caur reģistrēšanas procesu vēlreiz. [Lūdzu, veiciet šajā rakstā aprakstītās darbības.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ja šī ir pirmā reize, kad iespējojat MFA un lietotāji nevar pieteikties-pārlūkprogrammas klientiem, piemēram, Outlook, Skype utt, varbūt ADAL (Active Directory autentifikācijas bibliotēka) nav iespējots O365 abonements. Šajā gadījumā jums būs nepieciešams, lai izveidotu savienojumu ar Exchange Online PowerShell un palaist šo cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*