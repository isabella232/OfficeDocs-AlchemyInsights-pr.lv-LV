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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891756"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Programma Outlook nevar izveidot savienojumu ar publiskajām mapēm

Ja piekļuve publiskajai mapei nedarbojas dažiem lietotājiem, mēģiniet veikt šādas darbības:

Izveidot savienojumu ar EXO PowerShell un konfigurēt parametru DefaultPublicFolderMailbox problēmu lietotāja kontu, lai atbilstu parametru darba lietotāja kontu.

Piemērs:

Iegūt pastkasti WorkingUser | FT DefaultPublicFolderMailbox Efektivepublicfoldermailbox

Set-pastkaste ProblemUser-DefaultPublicFolderMailbox \<vērtību no iepriekšējās komandas>

Uzgaidiet vismaz vienu stundu, lai izmaiņas stātos spēkā.

Ja problēma joprojām pastāv, lūdzu, veiciet [šīs darbības](https://aka.ms/pfcte) , lai novērstu publiskās mapes piekļuves problēmas, izmantojot programmu Outlook.