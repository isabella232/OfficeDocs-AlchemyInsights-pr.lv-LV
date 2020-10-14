---
title: Intune Win32 lietojumprogrammu izvietošana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461872"
---
# <a name="intune-win32-app-deployment"></a>Intune Win32 lietojumprogrammu izvietošana

Microsoft Intune atļauj Win32 lietojumprogrammas, ieskaitot, bet neaprobežojoties ar MSI. EXE ir jāizvieto Windows 10 ierīcēs. Izmantotajam izvietošanas mehānismam ir nepieciešams, lai Intune pārvaldības paplašinājums (IME) būtu atrodams Target ierīcē. Pēc PowerShell skripta vai Win32 lietojumprogrammas izvietošanas uz lietotāju/ierīci tiek automātiski instalēts IME.

Pastāv arī priekšnosacījumu kopa, kas ir jāizpilda, lai izvietotu Win32 lietojumprogrammas, kas ietver:

- Atbalstītās platformas: Windows 10 versija 1607 vai jaunāka (Enterprise, Pro un Education versijas).
- Atbalstītā arhitektūra: x86 un x64.
- Ierīču pārvaldība: AAD ir pievienojies un automātiski reģistrējušies (ieskaitot hibrīdo domēnu un grupas politiku, kas tiek automātiski reģistrēta).
- Lietojumprogrammas pakotnes formāts: **intunewin**  failu, ko sagatavojis [Microsoft Win32 satura sagatavošanas rīks](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Ierobežojumi
    - Maksimālais lielums: 8GB.
    - Neatbalstītā arhitektūra: ieroči.

Lai skatītu informāciju, kas saistīta ar šīm darbībām, recenzējiet dokumentu "[pievienot, piešķirt un pārraudzīt Win32 lietojumprogrammu pakalpojumā Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)".

Detalizētu informāciju par problēmu novēršanu lietojumprogrammas izvietojumā sistēmā Windows, tostarp Win32 lietojumprogrammas, var pārskatīt šādos dokumentos

- [Lietojumprogrammas instalēšanas problēmu novēršana](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Win32 lietojumprogrammu problēmu novēršana](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)