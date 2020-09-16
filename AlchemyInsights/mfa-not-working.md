---
title: Problēmas ar MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755138"
---
# <a name="issues-with-azure-mfa"></a>Problēmas ar Azure MFA
Ir daži ieteikumi, kā pārbaudīt, vai lietotāji nevar pieteikties, izmantojot daudzfaktoru autentifikāciju (MFA)

1. Ietekmētais lietotājs var tikt bloķēts Azure Active Directory portālā. Ja tā ir, šī konkrētā lietotāja autentifikācijas mēģinājumi tiks automātiski noraidīti. [Lūdzu, veiciet šajā rakstā norādītās darbības, lai tās atbloķētu.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ja atbloķēšanas lietotājs nepalīdzēja vai lietotājs nav bloķēts, varat mēģināt atiestatīt MFA lietotājam, un tie tiks pārskaitīti no jauna reģistrēšanās procesam. [Lūdzu, veiciet šajā rakstā norādītās darbības.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ja šī ir pirmā reize, kad iespējojat MFA, un jūsu lietotāji nevar pieteikties pārlūkprogrammās, kas nav pārlūkprogrammu klienti, piemēram, Outlook, Skype utt., iespējams, ADAL (Active Directory Authentication Library) nav iespējots jūsu O365 abonementā. Šajā gadījumā vajadzēs izveidot savienojumu ar Exchange Online PowerShell un palaist šo cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*