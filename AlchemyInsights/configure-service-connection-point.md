---
title: Pakalpojumu savienojuma punkta konfigurēšana (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036145"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="56155-102">Pakalpojumu savienojuma punkta konfigurēšana (SCP)</span><span class="sxs-lookup"><span data-stu-id="56155-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="56155-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="56155-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="56155-104">**Iemesls**: nevar nolasīt SCP objektu un iegūt Azure AD nomnieka informāciju</span><span class="sxs-lookup"><span data-stu-id="56155-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="56155-105">**Risinājums**: skatiet sadaļu [pakalpojumu savienojuma punkta konfigurēšana](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="56155-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="56155-106">**Darbību plāns**</span><span class="sxs-lookup"><span data-stu-id="56155-106">**Action plan**</span></span>

- <span data-ttu-id="56155-107">Pārbaudiet, vai ierīce ir saņēmusi kontrolētās validācijas GPO.</span><span class="sxs-lookup"><span data-stu-id="56155-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="56155-108">Pārliecinieties, vai GPO ir izveidojis reģistra atslēgas.</span><span class="sxs-lookup"><span data-stu-id="56155-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="56155-109">Pārliecinieties, vai jums ir 2 taustiņi, kas izveidoti ar jūsu direktorija ID un onmicrosoft domēnu.</span><span class="sxs-lookup"><span data-stu-id="56155-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="56155-110">**Klienta puses reģistra iestatījuma konfigurēšana SCP**</span><span class="sxs-lookup"><span data-stu-id="56155-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="56155-111">Izmantojiet tālāk norādīto piemēru, lai izveidotu grupas politikas objekta (GPO), lai izvietotu reģistra iestatījumu, kas konfigurē SCP ierakstu savu ierīču reģistrā.</span><span class="sxs-lookup"><span data-stu-id="56155-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="56155-112">Atveriet grupas politikas pārvaldības konsoli un izveidojiet jaunu GPO jūsu domēnā.</span><span class="sxs-lookup"><span data-stu-id="56155-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="56155-113">Nodrošiniet jaunizveidotā GPO nosaukumu (piemēram, ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="56155-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="56155-114">Rediģējiet GPO un atrodiet šādu ceļu: **datora konfigurācija > Preferences > Windows iestatījumi > reģistru**.</span><span class="sxs-lookup"><span data-stu-id="56155-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="56155-115">Ar peles labo pogu noklikšķiniet uz **reģistrs** un atlasiet **Jauns > reģistra vienumu**.</span><span class="sxs-lookup"><span data-stu-id="56155-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="56155-116">Cilnē **Vispārīgi** konfigurējiet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="56155-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="56155-117">**Darbība**: atjaunināšana</span><span class="sxs-lookup"><span data-stu-id="56155-117">**Action**: Update</span></span>
    
- <span data-ttu-id="56155-118">**Strops**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="56155-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="56155-119">**Atslēgas ceļš**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="56155-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="56155-120">**Vērtības nosaukums**: TenantId</span><span class="sxs-lookup"><span data-stu-id="56155-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="56155-121">**Vērtības tips**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="56155-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="56155-122">**Vērtību dati**: Azure AD instances GUID vai direktorija ID (šī vērtība var atrast **Azure portālā > azure Active Directory > REKVIZĪTIEM > direktorija ID**)</span><span class="sxs-lookup"><span data-stu-id="56155-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="56155-123">Noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="56155-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="56155-124">Ar peles labo pogu noklikšķiniet uz **reģistrs** un atlasiet **Jauns > reģistra vienumu**.</span><span class="sxs-lookup"><span data-stu-id="56155-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="56155-125">Cilnē **Vispārīgi** konfigurējiet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="56155-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="56155-126">**Darbība**: atjaunināšana</span><span class="sxs-lookup"><span data-stu-id="56155-126">**Action**: Update</span></span>
    
- <span data-ttu-id="56155-127">**Strops**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="56155-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="56155-128">**Atslēgas ceļš**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="56155-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="56155-129">**Vērtības nosaukums**: TenantName</span><span class="sxs-lookup"><span data-stu-id="56155-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="56155-130">**Vērtības tips**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="56155-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="56155-131">**Vērtības dati**: jūsu Verificētais domēna nosaukums, ja izmantojat Federatīvo vidi, piemēram, AD FS.</span><span class="sxs-lookup"><span data-stu-id="56155-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="56155-132">Jūsu Verificētais domēna nosaukums vai jūsu onmicrosoft.com domēna nosaukums (piemēram, contoso. onmicrosoft). com, ja izmantojat pārvaldītu vidi</span><span class="sxs-lookup"><span data-stu-id="56155-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="56155-133">Noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="56155-133">Click **OK**.</span></span>

7. <span data-ttu-id="56155-134">Jāslēdz jaunizveidotā GPO redaktors.</span><span class="sxs-lookup"><span data-stu-id="56155-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="56155-135">Saistiet jaunizveidoto GPO ar vēlamo OU, kas ietver domēnu, kas pieder jūsu kontrolētajiem izvēršanas iedzīvotājiem.</span><span class="sxs-lookup"><span data-stu-id="56155-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="56155-136">Lai iegūtu papildinformāciju, skatiet rakstu [Hibrīdā AZURE ad Join-AZURE ad savienojuma pārbaude | Microsoft dokumenti](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) un  [problēmu novēršanas Hibrīdā Azure Active Directory pievienotās ierīces | Microsoft dokumenti](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="56155-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









