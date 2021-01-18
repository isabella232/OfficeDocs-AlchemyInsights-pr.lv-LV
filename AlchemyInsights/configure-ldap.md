---
title: LDAP konfigurēšana
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885164"
---
# <a name="configure-ldap"></a>LDAP konfigurēšana

Lai konfigurētu LDAP, veiciet tālāk norādītās darbības.

1. Pārbaudiet sava domēna darbspējas [Azure portālā](https://aka.ms/aadds-health).
1. Nodrošiniet, lai būtu pieejams derīgs Azure AD abonements un iespējots Azure AD Domain Services.
1. Sertifikāts, kas nepieciešams, lai iespējotu drošu LDAP, ir jāiegūst no uzticamas publiskās sertificēšanas iestādes vai jābūt pašparakstītam sertifikātam.
1. Pārliecinieties, vai sertifikāts atbilst nepieciešamajām [vadlīnijām](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Nederīgs sertifikāts**
1. Lai atjaunotu sertifikātu, veiciet norādītās darbības, lai izveidotu jaunu sertifikātu un atkārtoti augšupielādētu: [LDAP konfigurēšana](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Lai atrisinātu zināmo problēmu ar drošo LDAP brīdinājumiem Azure Active Directory domēnu pakalpojumos, skatiet sadaļu [LDAP brīdinājumu atrisināšana](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
