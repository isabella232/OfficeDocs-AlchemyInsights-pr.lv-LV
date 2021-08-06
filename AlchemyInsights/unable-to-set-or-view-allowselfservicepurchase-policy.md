---
title: Nevar iestatīt vai skatīt politiku AllowSelfServicePurchase
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
- "9001212"
- "3526"
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020199"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nevar iestatīt vai skatīt politiku AllowSelfServicePurchase

Mēģinot iestatīt vai skatīt politiku AllowSelfServicePurchase, tiek rādīts šāds kļūdas ziņojums:

*HandleError: Neizdevās izgūt produkta politiku ar PolicyId 'AllowSelfServicePurchase', ErrorMessage — pamatā esošais savienojums tika aizvērts: sūtīšanas laikā radās neparedzēta kļūda.*

Iemesls var būt vecāka transporta slāņa drošības (TLS) versija. Lai izveidotu savienojumu ar MSCommerce pakalpojumu, ir jāizmanto TLS 1.2 vai jaunāka versija.  

Mēģiniet veikt tālāk norādītās darbības, lai iespējotu/iestatītu TLS protokolu uz 1.2, pārbaudītu un mēģinātu vēlreiz.
 1. PowerShell komandu uzvednē (PS C: ievadiet šo komandu, lai \) iestatītu TLS protokolu uz versiju 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Pārbaudiet lietotos TLS protokolus ar šādu komandu:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Mēģiniet vēlreiz iegūt vai atjaunināt komandas pēc nepieciešamības.

