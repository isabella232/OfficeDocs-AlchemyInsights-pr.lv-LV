---
title: Nemanāma vienotās pierakstīšanās (SSO) problēmu novēršana lokālajā vidē
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816206"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="95990-102">Nemanāma vienotās pierakstīšanās (SSO) problēmu novēršana lokālajā vidē</span><span class="sxs-lookup"><span data-stu-id="95990-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="95990-103">Lai atrisinātu neviendabīgas vienotās pierakstīšanās (SSO) problēmas, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="95990-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="95990-104">**Kā varu pāriet uz AZUREADSSO datora konta Kerberos atšifrēšanas atslēgu?**</span><span class="sxs-lookup"><span data-stu-id="95990-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="95990-105">Ļoti ieteicams pārritināt Kerberos atšifrēšanas atslēgu vismaz reizi 30 dienās.</span><span class="sxs-lookup"><span data-stu-id="95990-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="95990-106">Lai to izdarītu manuāli, skatiet rakstu [kā pāriet uz Kerberos atšifrēšanas atslēgām](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span><span class="sxs-lookup"><span data-stu-id="95990-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="95990-107">**Nemanāma SSO konfigurēšana**</span><span class="sxs-lookup"><span data-stu-id="95990-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="95990-108">Lai izvietotu viengabala SSO, izpildiet darbības [Azure Active Directory nemanāma vienotā pierakstīšanās: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span><span class="sxs-lookup"><span data-stu-id="95990-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="95990-109">**Padomdevēja**</span><span class="sxs-lookup"><span data-stu-id="95990-109">**Advisory**</span></span>

- <span data-ttu-id="95990-110">[Azure Active Directory vienotā pierakstīšanās: bieži uzdotie jautājumi](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) — šajā rakstā mēs adresējam bieži uzdotos jautājumus par Azure Active Directory nemanāmu atsevišķu Sign-On (viengabala SSO).</span><span class="sxs-lookup"><span data-stu-id="95990-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="95990-111">Atgriezieties pie jauna satura pārbaude.</span><span class="sxs-lookup"><span data-stu-id="95990-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="95990-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) -šajā rakstā ir sniegta informācija par to, kā veikt līdzekļu pieprasījumus vai uzdot tehniskus jautājumus par viengabala SSO.</span><span class="sxs-lookup"><span data-stu-id="95990-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="95990-113">**Problēmu novēršana**</span><span class="sxs-lookup"><span data-stu-id="95990-113">**Troubleshoot**</span></span>

<span data-ttu-id="95990-114">[Azure Active Directory vienotās pierakstīšanās problēmu novēršana](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) šajā rakstā palīdz atrast problēmu novēršanas informāciju par biežāk sastopamajām problēmām attiecībā uz Azure Active Directory (Azure AD) bezproblēmu Single Sign-On (viengabala SSO).</span><span class="sxs-lookup"><span data-stu-id="95990-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







