---
title: Apakšdomēnu pievienošana
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506484"
---
# <a name="adding-a-sub-domain"></a>Apakšdomēnu pievienošana

Apakšdomēnus var pievienot tam pašam vai citā nomniekā, nevis vecākdomēnu. Jebkurā gadījumā jums ir jāpārvalda savi DNS iestatījumi reģistrētāja tīmekļa vietnē. Ja ļaujat korporācijai Microsoft pārvaldīt jūsu DNS iestatījumus, izmantojot NS ierakstus, vai ja domēnu iegādājāties no Microsoft, apakšdomēnus nevarat pievienot, tos vispirms nemainot.

Vispirms pievienojiet vecākdomēnu un pēc tam pievienojiet apakšdomēnu. Ja apakšdomēns atrodas vienā nomniekā, nav nepieciešama papildu pārbaude. Ja apakšdomēnu pievienojat atsevišķam nomniekam, īpašumtiesību pārbaudei ir nepieciešams DNS txt ieraksts pirms domēna pievienošanas un papildu DNS ieraksti atlasītajiem pakalpojumiem.

- Lai pievienotu domēnu vai apakšdomēnu, izpildiet domēna pievienošanas vedni vai manuāli pievienojiet domēnu vai apakšdomēnu, dodoties uz [](https://admin.microsoft.com/Adminportal#/Domains/Wizard)   >  **Domains** Add  >  **domain iestatīšana**.

Ja nepieciešams:

- Lai mainītu, kurš pārvalda jūsu DNS iestatījumus esošam domēnam, dodieties **uz Iestatījumi**  >  [**Domains**](https://admin.microsoft.com/Adminportal/Home#/Domains), atzīmējiet izvēles rūtiņu blakus domēnam un pēc tam atlasiet **Pārvaldīt DNS**. Vednī atlasiet Pievienot **savus DNS ierakstus un** pabeidziet darbības vednī.
- Lai pievienotu apakšdomēnus Microsoft iegādātam domēnam, vispirms pārvirziet domēnu pie cita reģistrētāja un pēc tam veiciet iepriekš minētās izmaiņas, lai pārvaldītu savus DNS ierakstus. Norādījumus skatiet rakstā [Domēna pārvietošana no Microsoft uz citu resursdatoru.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
- Ja tiek parādīts kļūdas ziņojums, ka jūsu domēnu jau izmanto citi dalībnieki vai personas jūsu organizācijā, jums vispirms ir jāpārņem šis nepārvaldītais konts, pirms izmantojat domēnu. Norādījumus skatiet rakstā [Nepārvaldīta direktorija pārraudzīšanu kā administratoram pakalpojumā Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover).
