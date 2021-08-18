---
title: Ierīces writeback
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: c069d0b4588e53250d6cc1f3a66c744ea5c12ae4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320093"
---
# <a name="device-writeback"></a>Ierīces writeback

Ierīces writeback tiek izmantots šādos scenārijos:

- Windows Hello [darbam iespējošana, izmantojot hibrīdo sertifikātu uzticamības izvietošanu](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Nosacījum piekļuves iespējošana, pamatojoties uz ierīcēm, ar ADFS (2012 R2 vai jaunāku versiju) aizsargātām lietojumprogrammām (uzticamās pušu uzticamības)

    **Piezīme.** Lai ierīcē rakstītu, ir Premium Azure AD abonements.

Tādējādi tiek nodrošināta papildu drošība un drošība, ka piekļuve lietojumprogrammām tiek piešķirta tikai uzticamām ierīcēm. Papildinformāciju par nosacījum piekļuvi skatiet [rakstā](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) Riska pārvaldība ar nosacījuma piekļuvi un Lokālās nosacījum piekļuves iestatīšana, izmantojot Azure Active Directory [ierīces reģistrāciju.](https://docs.microsoft.com/azure/active-directory/devices/overview)

Papildinformāciju par ierīces Writeback iespējošanu ierīcēm skatiet rakstā [Ierīces writeback iespējošana.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)
