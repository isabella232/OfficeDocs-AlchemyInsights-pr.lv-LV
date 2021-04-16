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
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810491"
---
# <a name="issues-with-azure-mfa"></a>Problēmas ar Azure MFA
Ir dažas lietas, kas jāpārbauda, vai lietotāji nevar pieteikties, izmantojot daudz faktoru autentificēšanu (MFA)

1. Ietekmēto lietotāju var bloķēt Azure Active Directory portālā. Šādā gadījumā konkrētam lietotājam autentifikācijas mēģinājumi tiks automātiski noraidīti. [Izpildiet šajā rakstā minētās darbības, lai tās atbloķētu.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ja lietotāja atbloķēšana nepalīdzēja vai lietotājs nav bloķēts, varat mēģināt atiestatīt lietotāja MFA un viņš vēlreiz veiks reģistrācijas procesu. [Izpildiet šajā rakstā norādītās darbības.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ja šī ir pirmā reize, kad iespējojat MFA un jūsu lietotāji nevar pieteikties klientiem, kas nav pārlūkprogrammas, piemēram, Outlook, Skype un citiem, iespējams, ADAL (Active Directory Authentication Library — Active Directory autentifikācijas bibliotēka) jūsu O365 abonementā nav iespējota. Šajā gadījumā būs jāizveido savienojums ar Exchange Online Powershell un jāpalaiž šis cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*