---
title: Exchange PowerShell un pamata autentifikācijas novecošana
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813479"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="5bb99-102">Exchange PowerShell un pamata autentifikācijas novecošana</span><span class="sxs-lookup"><span data-stu-id="5bb99-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="5bb99-103">Lai iegūtu jaunāko informāciju par to, kā izveidot savienojumu ar Exchange Online PowerShell, neizmantojot pamata autentifikāciju, [lūdzu, dodieties šeit](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="5bb99-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="5bb99-104">PowerShell V2 modulis neizmanto pamata autentifikāciju.</span><span class="sxs-lookup"><span data-stu-id="5bb99-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="5bb99-105">Ņemiet vērā, ka pamata autentifikācija joprojām ir jāiespējo klienta datorā.</span><span class="sxs-lookup"><span data-stu-id="5bb99-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="5bb99-106">Jaunais PowerShell V2 modulis izmanto moderno autentifikāciju, lai izveidotu savienojumu visu REST V2 cmdlet iespējošanai.</span><span class="sxs-lookup"><span data-stu-id="5bb99-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="5bb99-107">Papildus V2 cmdlet tas arī sniedz iespēju piekļūt vecākām Remote PowerShell (RPS) cmdlet, kam ir nepieciešams izveidot Remote PowerShell sesiju.</span><span class="sxs-lookup"><span data-stu-id="5bb99-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="5bb99-108">Lai izveidotu RPS sesiju Windows datorā, klienta datorā ir jāiespējo WinRM BasicAuth, lai gan modulis izmanto moderno autentifikācijas mehānismu, lai autentificētu pakalpojumā.</span><span class="sxs-lookup"><span data-stu-id="5bb99-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="5bb99-109">WinRM pamata autentifikācijas kanāls tiek lietots modernās autentifikācijas žetonu transportēšanai.</span><span class="sxs-lookup"><span data-stu-id="5bb99-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="5bb99-110">Ja WinRM pamata autentifikācija ir atspējota klienta datorā, jaunās V2 cmdlet turpinās darboties (taču vecākās RPS cmdlet nē).</span><span class="sxs-lookup"><span data-stu-id="5bb99-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
