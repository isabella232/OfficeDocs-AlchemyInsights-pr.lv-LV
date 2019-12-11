---
title: Nevar piekļūt publiskajām mapēm
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959501"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Programma Outlook nevar izveidot savienojumu ar publiskajām mapēm

Ja publiskās mapes piekļuve nedarbojas tikai dažiem lietotājiem, mēģiniet veikt šādas darbības:

Izveidot savienojumu ar EXO PowerShell un konfigurēt DefaultPublicFolderMailbox problēmu lietotāja kontu, lai saskaņotu vienu darba lietotāja kontu.

Piemērs:

Iegūt pastkasti WorkingUser | FT DefaultPublicFolderMailbox Efektivepublicfoldermailbox

Set-pastkaste ProblemUser-DefaultPublicFolderMailbox \<vērtību no iepriekšējās komandas>

Uzgaidiet vismaz vienu stundu, lai izmaiņas stātos spēkā.