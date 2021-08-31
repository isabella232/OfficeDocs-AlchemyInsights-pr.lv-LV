---
title: Problēmu Microsoft 365 Diemžēl mums ir īslaicīgu servera problēmu ziņojums
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 565f70d9a09c61bef84cdd1c23e9b0ed34bebe51
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744674"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Programmas Microsoft 365 "Diemžēl mums ir īslaicīgas servera problēmas"

Piezīme. Ja izmantojat vecāku Windows versiju (piemēram, Windows 7 SP1, Windows Server 2008 R2), izmantojiet [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) vienkāršo labojumu, lai iespējotu TLS 1.2 kā noklusējumu. Papildinformāciju skatiet rakstā Atjaunināšana, lai [iespējotu TLS 1.1 un TLS 1.2 kā noklusējuma drošos protokolus programmā WinHTTP Windows.](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Ja saņemat šādu ziņojumu, mēģiniet veikt šādas darbības:

1. Pārbaudiet savu ugunsmūri, pretvīrusu programmatūru un starpniekservera iestatījumus, lai pārliecinātos, vai tie nebloķē piekļuvi Microsoft 365 programmām. Skatiet [rakstu URL un IP adrešu diapazoni.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Dodieties **uz Start**  >  **Run** un pēc tam ierakstiet **services.msc**. Pārliecinieties, vai darbojas tālāk sniegtie pakalpojumi.
    - Tīkla savienoto ierīču automātiskā iestatīšana
    - Tīkla saraksta pakalpojums
    - Informētība par tīkla atrašanās vietu
    - Windows Notikumu žurnāls

Ja kāds no šiem pakalpojumiem nedarbojas, mēģiniet to startēt. Ja rodas problēma, startējot pakalpojumu, palaidiet tālāk norādīto komandu, atverot komandu uzvedni ar paaugstinātām atļaujām:

**sfc /scannow**

Kad šī komanda ir pabeigta, restartējiet datoru.

Detalizētu informāciju skatiet sadaļā ["Diemžēl nevaram izveidot savienojumu ar jūsu kontu. Lūdzu, vēlāk mēģiniet vēlreiz", kad aktivizējat.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)