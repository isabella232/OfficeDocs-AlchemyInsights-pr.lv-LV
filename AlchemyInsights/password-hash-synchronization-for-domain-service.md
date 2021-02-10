---
title: Paroļu jaukšanas sinhronizācija domēna pakalpojumam
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177487"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="68a86-102">Paroļu jaukšanas sinhronizācija domēna pakalpojumam</span><span class="sxs-lookup"><span data-stu-id="68a86-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="68a86-103">**Ja jūsu Azure AD DS instance piedāvā iespējot paroļu jaukšanas sinhronizāciju**</span><span class="sxs-lookup"><span data-stu-id="68a86-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="68a86-104">Tiek parādīts scenārijs, kurā tiek palaista Hibrīdā vide ar lietotājiem, kas tiek sinhronizēti no lokālā Azure Active Directory domēna pakalpojumu (AD DS) vides.</span><span class="sxs-lookup"><span data-stu-id="68a86-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="68a86-105">Šis scenārijs ir sastopams, ja jums ir paroļu jaukšanas sinhronizācija no lokālā AD DS uz jūsu Azure AD nomnieku.</span><span class="sxs-lookup"><span data-stu-id="68a86-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="68a86-106">**Izraisīt**</span><span class="sxs-lookup"><span data-stu-id="68a86-106">**Cause**</span></span>

<span data-ttu-id="68a86-107">Tas notiek tāpēc, ka Azure AD Connect pēc noklusējuma nesinhronizē mantoto jauno tehnoloģiju LAN Manager (NTLM) un Kerberos paroļu hashes, kas nepieciešamas Azure AD DS lietošanai.</span><span class="sxs-lookup"><span data-stu-id="68a86-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="68a86-108">**Risinājums**</span><span class="sxs-lookup"><span data-stu-id="68a86-108">**Workaround**</span></span> 

<span data-ttu-id="68a86-109">Lai sinhronizētu šīs paroļu hashes, kas nepieciešami NTLM un Kerberos autentifikācijai, ir jākonfigurē Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="68a86-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="68a86-110">Pēc Azure AD Connect konfigurēšanas, lokālā konta izveides vai paroles maiņas notikums arī pēc tam sinhronizē mantotās paroļu jaucējvirknes uz Azure AD.</span><span class="sxs-lookup"><span data-stu-id="68a86-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="68a86-111">Lai iegūtu papildinformāciju par šo problēmu, skatiet [šeit](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) un norādījumus par to, kā iespējot paroļu SINHRONIZĀCIJU AZURE AD DS hibrīdās vidēs.</span><span class="sxs-lookup"><span data-stu-id="68a86-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>