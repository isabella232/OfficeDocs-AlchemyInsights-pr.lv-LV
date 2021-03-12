---
title: Biežāk sastopamo problēmu novēršana saistībā ar DKIM ieraksta formatēšanu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746832"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Biežāk sastopamo problēmu novēršana saistībā ar DKIM ieraksta formatēšanu

Lielākā daļa DKIM iestatīšanas problēmu ir saistītas ar nepareiziem DNS ierakstiem.

Lai izlabotu DKIM iestatīšanas problēmas, pārbaudiet, vai DKIM CNAME ieraksts (**nevis** txt ieraksts) ir pareizi formatēts. Papildinformāciju skatiet rakstā kas jādara, [lai manuāli IESTATĪTU DKIM pakalpojumā Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Ja vēlaties saņemt palīdzību par DNS ierakstiem vispār, skatiet rakstu [DNS ierakstu izveide pie jebkura DNS viesošanas pakalpojumu sniedzēja pakalpojumā Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> Pēc tam, kad esat izveidojis vai atjauninājis savus DKIM DNS ierakstus pie sava domēna DNS viesošanas pakalpojuma, būs jāgaida, līdz tiek izplatīti DNS ieraksti.
