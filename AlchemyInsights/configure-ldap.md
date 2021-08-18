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
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090419"
---
# <a name="configure-ldap"></a>LDAP konfigurēšana

Lai konfigurētu LDAP, rīkojieties šādi:

1. Pārbaudiet sava domēna darbspēju [Azure portālā.](https://aka.ms/aadds-health)
1. Pārliecinieties, vai ir pieejams derīgs Azure AD abonements un iespējoti Azure AD domēna pakalpojumi.
1. Sertifikāts, kas nepieciešams, lai iespējotu drošu LDAP, ir jāiegūst no uzticamas publiskās sertificēšanas iestādes vai arī jābūt pašparakstītam sertifikātam.
1. Pārliecinieties, vai sertifikāts atbilst nepieciešamajām [vadlīnijām.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Nederīgs sertifikāts**
1. Lai atjaunotu sertifikātu, izpildiet norādījumus, lai izveidotu jaunu sertifikātu un atkārtoti ielādētu: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Lai novērstu zināmo problēmu ar Secure LDAP brīdinājumiem Azure Active Directory domēnu [pakalpojumos, skatiet sadaļu LDAP brīdinājumu atrise.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
