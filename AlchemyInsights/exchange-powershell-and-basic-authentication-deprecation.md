---
title: Exchange PowerShell un pamata autentifikācijas novecošana
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015696"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="eb283-102">Exchange PowerShell un pamata autentifikācijas novecošana</span><span class="sxs-lookup"><span data-stu-id="eb283-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="eb283-103">Lai iegūtu jaunāko informāciju par to, kā izveidot savienojumu ar Exchange Online PowerShell, neizmantojot pamata autentifikāciju, [lūdzu, dodieties šeit](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="eb283-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="eb283-104">Ņemiet vērā, ka pamata autentifikācija joprojām ir jāiespējo klienta datorā.</span><span class="sxs-lookup"><span data-stu-id="eb283-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="eb283-105">Jaunais PowerShell V2 modulis izmanto moderno autentifikāciju, lai izveidotu savienojumu visu REST V2 cmdlet iespējošanai.</span><span class="sxs-lookup"><span data-stu-id="eb283-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="eb283-106">Papildus V2 cmdlet tas arī sniedz iespēju piekļūt vecākām Remote PowerShell (RPS) cmdlet, kam ir nepieciešams izveidot Remote PowerShell sesiju.</span><span class="sxs-lookup"><span data-stu-id="eb283-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="eb283-107">Lai izveidotu RPS sesiju Windows datorā, klienta datorā ir jāiespējo WinRM BasicAuth, lai gan modulis izmanto moderno autentifikācijas mehānismu, lai autentificētu pakalpojumā.</span><span class="sxs-lookup"><span data-stu-id="eb283-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="eb283-108">WinRM pamata autentifikācijas kanāls tiek lietots modernās autentifikācijas žetonu transportēšanai.</span><span class="sxs-lookup"><span data-stu-id="eb283-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="eb283-109">Ja WinRM pamata autentifikācija ir atspējota klienta datorā, jaunās V2 cmdlet turpinās darboties (taču vecākās RPS cmdlet nē).</span><span class="sxs-lookup"><span data-stu-id="eb283-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
