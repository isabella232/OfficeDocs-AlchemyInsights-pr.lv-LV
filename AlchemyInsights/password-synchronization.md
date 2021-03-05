---
title: Paroles sinhronizācija
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482038"
---
# <a name="password-synchronization"></a><span data-ttu-id="f1afd-102">Paroles sinhronizācija</span><span class="sxs-lookup"><span data-stu-id="f1afd-102">Password synchronization</span></span>

<span data-ttu-id="f1afd-103">**Paroļu jaukšanas sinhronizācija vispār nedarbojas**</span><span class="sxs-lookup"><span data-stu-id="f1afd-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="f1afd-104">Biežāk sastopamās problēmas, kas rodas klientiem, ja nedarbojas paroļu jaukšanas sinhronizācija, ir šādas:</span><span class="sxs-lookup"><span data-stu-id="f1afd-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="f1afd-105">Active Directory konts, ko izmanto Azure AD Connect, lai sazinātos ar lokālo pakalpojumu Active Directory, nepiešķir **replicēšanas direktorija izmaiņas** un **replicē direktorija izmaiņas** , kas nepieciešamas paroļu sinhronizēšanai, un jums tas ir jānovērš, piešķirot šīs atļaujas Active Directory kontam.</span><span class="sxs-lookup"><span data-stu-id="f1afd-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="f1afd-106">Paroļu jaukšanas sinhronizācija ir atspējota pēc tam, kad administrators ir mainījis lietotāja Sign-In metodi no **paroļu sinhronizēšanas** uz citu opciju, piemēram, **FEDERĀCIJU ar AD FS** Azure AD Connect vednī — to var izlabot, atkārtoti iespējojot **paroļu jaukšanas sinhronizācijas** līdzekli Azure AD Connect vednī.</span><span class="sxs-lookup"><span data-stu-id="f1afd-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="f1afd-107">Savienojamības problēma ar lokālo Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f1afd-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="f1afd-108">Piemēram, dažiem domēnu kontrolleriem nevar piekļūt, izmantojot Azure AD Connect, vai [nepieciešamos portus](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) ir bloķējis ugunsmūris — tas ir jānovērš, nodrošinot, ka savienojamība starp Azure AD Connect serveri un lokālo Active Directory darbojas pareizi.</span><span class="sxs-lookup"><span data-stu-id="f1afd-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="f1afd-109">Azure AD Connect serveris pašlaik tiek atvērts sagatavošanas režīmā, un tas rezultātā serveris nevarēs izmantot paroļu jaukšanas iespējas — lai novērstu šo problēmu, izpildiet rakstā norādītās darbības: [paroļu sinhronizēšana ar AZURE ad Connect sinhronizāciju — nav paroļu](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="f1afd-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="f1afd-110">**Dažu lietotāju paroļu jaukšanas sinhronizācija nedarbojas**</span><span class="sxs-lookup"><span data-stu-id="f1afd-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="f1afd-111">Ja esat pamanījis, ka parole hash netiek sinhronizēta lietotājam, izmantojiet **problēmu novēršanas** uzdevumu Azure AD Connect, lai izpētītu un atrisinātu problēmu.</span><span class="sxs-lookup"><span data-stu-id="f1afd-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="f1afd-112">Veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="f1afd-112">Perform the following tasks:</span></span>

    <span data-ttu-id="f1afd-113">izveide.</span><span class="sxs-lookup"><span data-stu-id="f1afd-113">a.</span></span> [<span data-ttu-id="f1afd-114">Vedņa problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="f1afd-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="f1afd-115">b.</span><span class="sxs-lookup"><span data-stu-id="f1afd-115">b.</span></span> [<span data-ttu-id="f1afd-116">Problēmu novēršanas cmdlet izmantošana, lai izpētītu paroļu jaukšanas problēmu saistībā ar konkrētu lietošanu</span><span class="sxs-lookup"><span data-stu-id="f1afd-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="f1afd-117">Lokālā Active Directory lietotāja objekts ir iespējots **lietotājam ir jāmaina parole blakus pieteikšanās** opcijai.</span><span class="sxs-lookup"><span data-stu-id="f1afd-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="f1afd-118">Ja šī opcija ir iespējota, lietotājam tiek piešķirta pagaidu parole, un tiks prasīts mainīt paroli nākamajā pieteikšanās reizē.</span><span class="sxs-lookup"><span data-stu-id="f1afd-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="f1afd-119">Azure AD Connect nesinhronizē pagaidu paroles pakalpojumam Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1afd-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="f1afd-120">Lai atrisinātu šo problēmu, veiciet kādu no tālāk norādītajiem uzdevumiem.</span><span class="sxs-lookup"><span data-stu-id="f1afd-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="f1afd-121">Lūdziet lietotājam pierakstīties lokālajā lietojumprogrammā (piemēram, Windows datorā) un mainīt paroli.</span><span class="sxs-lookup"><span data-stu-id="f1afd-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="f1afd-122">Jaunā parole tiks sinhronizēta ar Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1afd-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="f1afd-123">Administratoram ir jāatjaunina lietotāja parole, neiespējojot opciju **lietotājam nākamajā pieteikšanās reizē ir jāmaina parole** un jākopīgo jaunā parole ar lietotāju.</span><span class="sxs-lookup"><span data-stu-id="f1afd-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="f1afd-124">Lokālā Active Directory lietotāja objekts nav **pareizi konfigurēts** objektu sinhronizācijai vai paroļu sinhronizēšanai.</span><span class="sxs-lookup"><span data-stu-id="f1afd-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="f1afd-125">Lai novērstu šo problēmu, izpildiet darbības, kas aprakstītas rakstā [paroļu jaukšanas sinhronizācijas problēmu novēršana, izmantojot AZURE ad Connect sinhronizāciju](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="f1afd-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







