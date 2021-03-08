---
title: ClientAccessServerEnabled iestatīšana uz patiess
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
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525969"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="c9efa-102">ClientAccessServerEnabled iestatīšana uz patiess</span><span class="sxs-lookup"><span data-stu-id="c9efa-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="c9efa-103">Ja nevarat atvērt šifrētu e-pasta ziņojumu un tā vietā skatīt **rpmsg** pielikumu, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="c9efa-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="c9efa-104">Savienojuma izveide ar Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c9efa-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="c9efa-105">Lai izveidotu savienojumu ar Exchange Online PowerShell, jums ir jāpierakstās, izmantojot globālo administratoru vai Exchange administratora kontu.</span><span class="sxs-lookup"><span data-stu-id="c9efa-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="c9efa-106">izveide.</span><span class="sxs-lookup"><span data-stu-id="c9efa-106">a.</span></span> <span data-ttu-id="c9efa-107">Atveriet programmu Windows PowerShell un pēc tam izpildiet šādu komandu: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="c9efa-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="c9efa-108">b.</span><span class="sxs-lookup"><span data-stu-id="c9efa-108">b.</span></span> <span data-ttu-id="c9efa-109">Dialoglodziņā **Windows PowerShell akreditācijas datu pieprasījums** ievadiet savu darba vai mācību iestādes kontu un paroli c.</span><span class="sxs-lookup"><span data-stu-id="c9efa-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="c9efa-110">Noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="c9efa-110">Click **OK**.</span></span> 

2. <span data-ttu-id="c9efa-111">Lai izveidotu jaunu sesiju, izpildiet šādu komandu:</span><span class="sxs-lookup"><span data-stu-id="c9efa-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="c9efa-112">izveide.</span><span class="sxs-lookup"><span data-stu-id="c9efa-112">a.</span></span> <span data-ttu-id="c9efa-113">Palaidiet šādu komandu:</span><span class="sxs-lookup"><span data-stu-id="c9efa-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="c9efa-114">`Get-IRMConfiguration`Komanda Palaist.</span><span class="sxs-lookup"><span data-stu-id="c9efa-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="c9efa-115">Pārbaudiet iestatījumu **ClientAccessServerEnabled** .</span><span class="sxs-lookup"><span data-stu-id="c9efa-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="c9efa-116">izveide.</span><span class="sxs-lookup"><span data-stu-id="c9efa-116">a.</span></span> <span data-ttu-id="c9efa-117">Ja **ClientAccessServerEnabled** iestatījums ir **FALSE**, izpildiet šo cmdlet komandu: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="c9efa-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="c9efa-118">Vienmēr izvērsiet PowerShell sesiju ar šādu komandu: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="c9efa-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="c9efa-119">Papildinformāciju skatiet rakstā [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="c9efa-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

