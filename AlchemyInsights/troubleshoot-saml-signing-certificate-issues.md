---
title: Problēmu novēršana saistībā ar sertifikātu SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693425"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Problēmu novēršana saistībā ar sertifikātu SAML

Lai atrisinātu SAML pierakstīšanās sertifikāta problēmu, veiciet tālāk norādītās darbības.

1. Kad pievienojat uzņēmuma lietojumprogrammu, kas atbalsta SSO, Azure ģenerēs sertifikātu, ko dēvē par [SAML parakstīšanas sertifikātu](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications). Šī sertifikāta derīguma termiņš ir 3 gadi. Lai mainītu sertifikāta derīguma termiņu, skatiet rakstu [Federācijas sertifikāta derīguma termiņa pielāgošana un pāriešana uz jaunu sertifikātu](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. Azure izmantos šo sertifikātu, lai parakstītu SAML marķierus, kurus pieprasījusi lietojumprogramma, un nosūtītu to uz lietojumprogrammas izraudzīto SSO. Lai šo pabeigtu, lejupielādējiet sertifikātu no Azure portāla un nosūtiet to lietojumprogrammas piedāvātājam, lai pabeigtu SSO procesu.

Pēc tam, kad šī procesa pabeigšana lietojumprogramma uzticēs šo sertifikātu un visas šajā sertifikātā parakstītās SAML marķierierīces tiks akceptētas.

3. Ja šī sertifikāta derīgums beidzas, izveidojiet jaunu sertifikātu, atjauniniet to lietojumprogrammas pārdevējam un pēc tam aktivizējiet to pakalpojumā Azure Side. Papildinformāciju skatiet rakstā [tā sertifikāta atjaunošana, kura derīguma termiņš drīz beigsies](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

> [!NOTE]
> Ja sertifikāta derīgums beidzas, lietotājs netiks bloķēts.

4. [Pievienojiet e-pasta adresi paziņojumiem](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) , kas tiks saņemti pirms pašreizējā sertifikāta derīguma perioda beigām.

> [!NOTE]
> Step-4 nav obligāts.

5. Mainiet lietojumprogrammas SAML sertifikāta parakstīšanas opcijas un sertifikāta parakstīšanas algoritmu. Papildinformāciju skatiet rakstā [sertifikāta parakstīšanas opciju un paraksta algoritma maiņa](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

