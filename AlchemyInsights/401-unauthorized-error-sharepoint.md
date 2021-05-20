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
ms.openlocfilehash: ac2fe27a8e7b277bfaf18303bf5b792410a1ea6a
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539939"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Nesankcionēta SharePoint

Ja saņemat kļūdas ziņojumu "(401) Neautorizēta" programmā SharePoint tā, iespējams, ir saistīta ar TLS 1.0/1.1 novecošanu. Papildinformāciju skatiet rakstā:

- [Gatavošanās TLS 1.2 Office 365 Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Autentifikācijas kļūdas rodas, ja klientam nav TLS 1.2 atbalsta](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Atjauniniet, lai iespējotu TLS 1.1 un TLS 1.2 kā noklusējuma drošo protokolu winhttp Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Ja lietotāji izmanto 7 Windows, pārliecinieties, vai viņi [pārbauda TLS cipher Suite in Windows 7.](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)