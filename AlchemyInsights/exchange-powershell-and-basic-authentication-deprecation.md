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
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell un pamata autentifikācijas novecošana

Lai iegūtu jaunāko informāciju par to, kā izveidot savienojumu ar Exchange Online PowerShell, neizmantojot pamata autentifikāciju, [lūdzu, dodieties šeit](https://aka.ms/psbasicauth).

Ņemiet vērā, ka pamata autentifikācija joprojām ir jāiespējo klienta datorā.
Jaunais PowerShell V2 modulis izmanto moderno autentifikāciju, lai izveidotu savienojumu visu REST V2 cmdlet iespējošanai. Papildus V2 cmdlet tas arī sniedz iespēju piekļūt vecākām Remote PowerShell (RPS) cmdlet, kam ir nepieciešams izveidot Remote PowerShell sesiju. Lai izveidotu RPS sesiju Windows datorā, klienta datorā ir jāiespējo WinRM BasicAuth, lai gan modulis izmanto moderno autentifikācijas mehānismu, lai autentificētu pakalpojumā. WinRM pamata autentifikācijas kanāls tiek lietots modernās autentifikācijas žetonu transportēšanai. Ja WinRM pamata autentifikācija ir atspējota klienta datorā, jaunās V2 cmdlet turpinās darboties (taču vecākās RPS cmdlet nē).
