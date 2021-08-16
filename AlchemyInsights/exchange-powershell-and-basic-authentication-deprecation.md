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
ms.openlocfilehash: 7b5acf4dd3061c7d9ed23d52a8355865592b9a1d743025fc9300dcda5a18831a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069251"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell un pamata autentifikācijas novecošana

Lai iegūtu jaunāko informāciju par to, kā izveidot savienojumu ar Exchange Online PowerShell, neizmantojot pamata autentifikāciju, [lūdzu, dodieties šeit](https://aka.ms/exops-docs). PowerShell V2 modulis neizmanto pamata autentifikāciju.

Ņemiet vērā, ka pamata autentifikācija joprojām ir jāiespējo klienta datorā.
Jaunais PowerShell V2 modulis izmanto moderno autentifikāciju, lai izveidotu savienojumu visu REST V2 cmdlet iespējošanai. Papildus V2 cmdlet tas arī sniedz iespēju piekļūt vecākām Remote PowerShell (RPS) cmdlet, kam ir nepieciešams izveidot Remote PowerShell sesiju. Lai izveidotu RPS sesiju Windows datorā, klienta datorā ir jāiespējo WinRM BasicAuth, lai gan modulis izmanto moderno autentifikācijas mehānismu, lai autentificētu pakalpojumā. WinRM pamata autentifikācijas kanāls tiek lietots modernās autentifikācijas žetonu transportēšanai. Ja WinRM pamata autentifikācija ir atspējota klienta datorā, jaunās V2 cmdlet turpinās darboties (taču vecākās RPS cmdlet nē).
