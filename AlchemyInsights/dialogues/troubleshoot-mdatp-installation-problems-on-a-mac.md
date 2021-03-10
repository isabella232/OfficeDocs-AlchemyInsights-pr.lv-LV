---
title: MDATP instalēšanas problēmu novēršana Mac datorā
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694281"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>MDATP instalēšanas problēmu novēršana Mac datorā

Ja manuāla instalēšana neizdevās, instalēšanas vedņa **kopsavilkuma** lapā tiek rādīta šāda kļūda:

"Instalēšanas laikā radās kļūda. Instalēšanas programma atklāja kļūdu, kuras dēļ instalēšana neizdevās. Lai saņemtu palīdzību, sazinieties ar programmatūras ražotāju.

MDM izvietojumiem lapā tiek rādīta arī vispārīga instalēšanas kļūme.

Lai gan nerāda precīzas kļūdas lietotājiem, mēs pabeidzam reģistrēt failu ar instalēšanas norisi programmā **/Library/logs/Microsoft/mdatp/Install.log**. Katra instalācijas sesija pievieno šo žurnālfailu. Lai izvadītu tikai pēdējo instalēšanas sesiju, izmantojiet `sed` .

Lai uzzinātu vairāk, skatiet rakstu [problēmu novēršana saistībā ar Microsoft Defender ATP darbam ar Mac instalēšanas problēmām](https://go.microsoft.com/fwlink/?linkid=2144615).
