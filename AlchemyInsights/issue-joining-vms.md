---
title: Problēma, kas savieno VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885656"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="b10ed-102">Problēma, kas savieno VMs</span><span class="sxs-lookup"><span data-stu-id="b10ed-102">Issue joining VMs</span></span>

<span data-ttu-id="b10ed-103">Lai atrisinātu problēmas, kas rodas, mēģinot pievienoties VMs, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="b10ed-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="b10ed-104">Mēģiniet pierakstīties, izmantojot **UPN** formātu (piemēram, "joeuser@contoso.com"), nevis **SAMAccountName** formātu (' CONTOSO\joeuser ').</span><span class="sxs-lookup"><span data-stu-id="b10ed-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="b10ed-105">Pārliecinieties, vai esat iespējojis paroļu sinhronizāciju atbilstoši *darba sākšanas* rokasgrāmatā izklāstītajām darbībām.</span><span class="sxs-lookup"><span data-stu-id="b10ed-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="b10ed-106">Nodrošiniet, lai attiecīgais lietotāja konts nav ārējs konts Azure AD nomniekā.</span><span class="sxs-lookup"><span data-stu-id="b10ed-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="b10ed-107">Ārējie lietotāji nevar pierakstīties pārvaldītajā domēnā, jo Azure AD domēna pakalpojumos nav šādu lietotāju kontu akreditācijas datu.</span><span class="sxs-lookup"><span data-stu-id="b10ed-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="b10ed-108">Ja attiecīgais lietotāja konts ir tikai Cloud lietotāja konts, pārliecinieties, vai lietotāji ir mainījuši savu paroli pēc Azure AD Domain Services iespējošanas.</span><span class="sxs-lookup"><span data-stu-id="b10ed-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="b10ed-109">Veicot šo darbību, tiek izraisīti, lai varētu ģenerēt Azure AD domēna pakalpojumu vajadzībām nepieciešamos akreditācijas datus.</span><span class="sxs-lookup"><span data-stu-id="b10ed-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="b10ed-110">Ja ietekmētie lietotāju konti tiek sinhronizēti no lokālā direktorija, pārbaudiet, vai Azure AD Connect ieteicamais laidiens ir konfigurēts, lai veiktu pilnu sinhronizāciju.</span><span class="sxs-lookup"><span data-stu-id="b10ed-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="b10ed-111">Ja pēc 4. darbības apstiprināšanas problēma ir novērsta, izpildiet tālāk minētās komandas no sinhronizācijas datora.</span><span class="sxs-lookup"><span data-stu-id="b10ed-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="b10ed-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="b10ed-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>