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
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/25/2019
ms.locfileid: "36545179"
---
# <a name="issues-with-mfa"></a>Problēmas ar MFA
Ir dažas lietas, kas jāpārbauda, ja lietotāji nevar pieteikties, izmantojot vairāku faktoru autentifikāciju (MFA)

1. Ietekmēto lietotāju var bloķēt Azure Active Directory portālā. Šādā gadījumā automātiski tiek liegta autentifikācijas mēģinājumi šim konkrētam lietotājam. [Lūdzu, veiciet šajā rakstā aprakstītās darbības, lai atbloķētu tos.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ja atbloķēšanas lietotāja nepalīdzēja vai lietotājs nav bloķēts varat mēģināt atiestatīt MFA par lietotāju, un viņi iet caur reģistrēšanas procesu vēlreiz. [Lūdzu, veiciet šajā rakstā aprakstītās darbības.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ja šī ir pirmā reize, kad iespējojat MFA un lietotāji nevar pieteikties-pārlūkprogrammas klientiem, piemēram, Outlook, Skype utt, varbūt ADAL (Active Directory autentifikācijas bibliotēka) nav iespējots O365 abonements. Šajā gadījumā jums būs nepieciešams, lai izveidotu savienojumu ar Exchange Online PowerShell un palaist šo cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*