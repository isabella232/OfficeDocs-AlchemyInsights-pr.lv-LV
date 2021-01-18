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
# <a name="configure-ldap"></a><span data-ttu-id="f5b74-102">LDAP konfigurēšana</span><span class="sxs-lookup"><span data-stu-id="f5b74-102">Configure LDAP</span></span>

<span data-ttu-id="f5b74-103">Lai konfigurētu LDAP, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="f5b74-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="f5b74-104">Pārbaudiet sava domēna darbspējas [Azure portālā](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="f5b74-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="f5b74-105">Nodrošiniet, lai būtu pieejams derīgs Azure AD abonements un iespējots Azure AD Domain Services.</span><span class="sxs-lookup"><span data-stu-id="f5b74-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="f5b74-106">Sertifikāts, kas nepieciešams, lai iespējotu drošu LDAP, ir jāiegūst no uzticamas publiskās sertificēšanas iestādes vai jābūt pašparakstītam sertifikātam.</span><span class="sxs-lookup"><span data-stu-id="f5b74-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="f5b74-107">Pārliecinieties, vai sertifikāts atbilst nepieciešamajām [vadlīnijām](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span><span class="sxs-lookup"><span data-stu-id="f5b74-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="f5b74-108">**Nederīgs sertifikāts**</span><span class="sxs-lookup"><span data-stu-id="f5b74-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="f5b74-109">Lai atjaunotu sertifikātu, veiciet norādītās darbības, lai izveidotu jaunu sertifikātu un atkārtoti augšupielādētu: [LDAP konfigurēšana](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="f5b74-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="f5b74-110">Lai atrisinātu zināmo problēmu ar drošo LDAP brīdinājumiem Azure Active Directory domēnu pakalpojumos, skatiet sadaļu [LDAP brīdinājumu atrisināšana](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="f5b74-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
