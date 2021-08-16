---
title: Problēmas ar MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098609"
---
# <a name="issues-with-azure-mfa"></a>Problēmas ar Azure MFA
Ir dažas lietas, kas jāpārbauda, vai lietotāji nevar pieteikties, izmantojot daudz faktoru autentificēšanu (MFA)

1. Ietekmētais lietotājs, iespējams, ir bloķēts Azure Active Directory portālā. Šādā gadījumā konkrētam lietotājam autentifikācijas mēģinājumi tiks automātiski noraidīti. [Izpildiet šajā rakstā minētās darbības, lai tās atbloķētu.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ja lietotāja atbloķēšana nepalīdzēja vai lietotājs nav bloķēts, varat mēģināt atiestatīt lietotāja MFA un viņš vēlreiz veiks reģistrācijas procesu. [Izpildiet šajā rakstā norādītās darbības.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ja šī ir pirmā reize, kad iespējojat MFA un jūsu lietotāji nevar pieteikties klientiem, kas nav pārlūkprogrammas, piemēram, Outlook, Skype utt., iespējams, ADAL (Active Directory Authentication Library — Active Directory autentifikācijas bibliotēka) jūsu O365 abonementam nav iespējota. Šajā gadījumā būs jāizveido savienojums ar Exchange Online Powershell un jāpalaiž šis cmdlet: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*