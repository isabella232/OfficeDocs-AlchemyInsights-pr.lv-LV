---
title: Pamatā esošais savienojums tika slēgts SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 1b4f336f389eb6fd81ac2ca40e6047184cc4c1bf
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317703"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Kļūdas ziņojums "Pamatā esošais savienojums tika aizvērts" SharePoint

Ja saņemat kļūdas ziņojumu "Pamatā esošais savienojums tika aizvērts" programmā SharePoint tas, iespējams, ir saistīts ar TLS 1.0/1.1 novecošanu. Papildinformāciju skatiet šajos rakstos:

- [Gatavošanās TLS 1.2 Office 365 Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Autentifikācijas kļūdas rodas, ja klientam nav TLS 1.2 atbalsta](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Atjauniniet, lai iespējotu TLS 1.1 un TLS 1.2 kā noklusējuma drošo protokolu winhttp programmā Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Ja lietotāji izmanto 7 Windows, pārliecinieties, vai viņi [pārbauda TLS cipher Suite in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).