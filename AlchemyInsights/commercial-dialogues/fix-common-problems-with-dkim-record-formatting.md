---
title: Bieži sastopamo problēmu ar DKIM ierakstu formatējumu novēršana
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
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930068"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Bieži sastopamo problēmu ar DKIM ierakstu formatējumu novēršana

Lielākā daļa DKIM iestatīšanas problēmu ir saistītas ar nepareiziem DNS ierakstiem.

Lai novērstu DKIM iestatīšanas problēmas, pārliecinieties, vai DKIM CNAME ieraksts **(nevis** TXT ieraksts) ir pareizi formatēts. Papildinformāciju skatiet [rakstā Kas jādara, lai manuāli iestatītu DKIM programmā Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Ja jums ir nepieciešama palīdzība saistībā ar DNS ierakstiem kopumā, skatiet rakstu DNS ierakstu izveide pie jebkura [DNS viesošanas pakalpojumu sniedzēja, kas paredzēts Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

> [!NOTE]
> Pēc tam, kad izveidosit vai atjaunināsit DKIM DNS ierakstus jūsu domēna DNS viesošanas pakalpojumā, būs jāgaida, līdz DNS ieraksti tiks izplatīti.
