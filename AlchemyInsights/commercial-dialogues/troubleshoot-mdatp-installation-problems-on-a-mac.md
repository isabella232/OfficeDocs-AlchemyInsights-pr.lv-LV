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
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091052"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>MDATP instalēšanas problēmu novēršana Mac datorā

Ja manuāla instalēšana neizdodas, **instalēšanas** vedņa lapā Kopsavilkums tiek parādīts šāds kļūdas ziņojums:

"Instalēšanas laikā radās kļūda. Instalēšanas programmai radās kļūda, kas izraisīja instalācijas atteici. Lai saņemtu palīdzību, sazinieties ar programmatūras ražotāju."

MDM izvietojumiem lapā ir redzama arī vispārīga instalēšanas kļūme.

Lai gan lietotājiem netiek rādītas precīzas kļūdas, mēs paturam žurnālfailu ar instalēšanas norisi programmā **/Library/Logs/Microsoft/mdatp/install.log.** Katra instalācijas sesija tiek pievienota šim žurnālfailam. Lai izvadītu tikai pēdējo instalēšanas sesiju, izmantojiet `sed` .

Papildinformāciju skatiet rakstā [Microsoft Defender ATP operētājsistēmai Mac](https://go.microsoft.com/fwlink/?linkid=2144615)instalēšanas problēmu novēršana.
