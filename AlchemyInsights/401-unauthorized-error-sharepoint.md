---
title: 401 Nesankcionēta SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 04f56dfc7ebe7de91bc64a5e6d2b480b07741c6e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314355"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Nesankcionēta SharePoint

Ja saņemat kļūdas ziņojumu "(401) Neautorizēta" programmā SharePoint tā, iespējams, ir saistīta ar TLS 1.0/1.1 novecošanu. Papildinformāciju skatiet rakstā:

- [Gatavošanās TLS 1.2 Office 365 Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Autentifikācijas kļūdas rodas, ja klientam nav TLS 1.2 atbalsta](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Atjauniniet, lai iespējotu TLS 1.1 un TLS 1.2 kā noklusējuma drošo protokolu winhttp programmā Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Ja lietotāji izmanto 7 Windows, pārliecinieties, vai viņi [pārbauda TLS cipher Suite in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).