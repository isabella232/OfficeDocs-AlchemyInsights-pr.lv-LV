---
title: Šifrēšana ar transportēšanas kārtulu palīdzību
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915173"
---
# <a name="encryption-with-transport-rules"></a>Šifrēšana ar transportēšanas kārtulu palīdzību

[Exchange administrēšanas centrā](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) savās pasta plūsmas kārtulās jūs varat izmantot Office ziņojumu šifrēšanas (OME) iespējas, lai veiktu ziņojumu šifrēšanu. Izvēlieties opciju **Pielietot Office 365 ziņojumu šifrēšanu un tiesību aizsardzību** transportēšanas kārtulas nosacījumam.

- Lai uzzinātu vairāk, lasiet [Šifrēšanas pasta plūsmas kārtulas definēšana](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Pakalpojumā PowerShell noklikšķiniet uz komandlietotnes[New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) un iestatiet parametru *ApplyOME* parametru kā $true.
