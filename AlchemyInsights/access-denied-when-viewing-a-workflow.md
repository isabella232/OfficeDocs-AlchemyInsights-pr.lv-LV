---
title: Piekļuve liegta, skatot darbplūsmu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955208"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Piekļuve liegta, skatot darbplūsmu

SharePoint 2013 darbplūsmas, kas mēģina nosūtīt e-pasta ziņojumu SharePoint grupai, var neizdoties ar kļūdas ziņojumu "Piekļuve liegta", ja SharePoint grupas dalība nav iestatīta kā Ikviens.
  
 **Lai novērstu šo problēmu, veiciet tālāk norādītās darbības.**
  
 1. Atļaujiet visiem skatīt grupas SharePoint dalībniekus.
  
 2. Noņemiet SharePoint e-pasta ziņojuma rindiņā Kam vai Kopija.
  
 3. Tieši pievienojiet lietotājus rindiņā Kam vai Kopija, ja dalības redzamību nevar mainīt SharePoint grupai.
  
Lai skatītu papildinformāciju, skatiet sadaļu HTTP nepilnvarots [uz /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  