---
title: Novērst problēmas ziņojumu piekļuve liegta
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: ee154a60d80472639371d44faef464eea8734dc9
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716653"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Problēmu novēršana darbā ar Sharepoint/OneDrive administrēšanas centrā ziņojumi Piekļuve liegta

<p><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Ja saņemat ziņojumu par liegtu piekļuvi, mēģinot meklēt Sharepoint/OneDrive Admin Center, lūdzu, pārliecinieties, ka jums <a href="https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One">piešķirt licenci lietotājam </a>. Ja lietotājam ir licence, jums vajadzētu arī pārliecināties tie ir <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/about-admin-roles?view=o365-worldwide">piešķirta administratora loma</a> , var piekļūt admin centriem.</span></p>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Šī problēma var arī rasties, ja lietotājs ir dzēsta un izveidota atkārtoti, izmantojot vienu un to pašu lietotāja pamatnosaukums (UPN). Jaunais konts ir izveidots, izmantojot citu PUID (pases unikālo ID) vērtību. Ja lietotājs mēģina piekļūt vietņu kolekcijā vai to OneDrive, lietotājam ir nepareiza PUID. Otrais scenārijs ietver directory sinhronizācija ar Active Directory organizācijas vienību (OU). Ja lietotāji jau pieslēdzās SharePoint, un tad ir pārvietots uz citu OU un resynced ar SharePoint, viņiem šī problēma var rasties.</span></span></p>  <ul style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;" type="disc">  <li style="line-height: normal; ; font-size: 11pt; font-style: normal; font-weight: 400;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Lai atrisinātu šo problēmu, vajadzētu atjaunot sākotnējo UPN ar rakstu, <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">atjaunot Office 365 lietotāja</a>darbības.</span></span></li>  </ul>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><strong><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;">Piezīme:</span></span></strong><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-fareast-font-family: 'Times New Roman'; mso-bidi-font-family: 'Times New Roman';"><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><em style="mso-bidi-font-style: normal;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">&nbsp;</span></em><em><span style="font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;font-style: normal; mso-bidi-font-style: italic;">Ja OneDrive vai SharePoint administrēšanas centru nav pieejams vairākiem lietotājiem, kas iepriekš bija pieejami, var būt pagaidu pakalpojumu jautājums.&nbsp; </span></span></em> <em><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;"> <a href="https://portal.office.com/adminportal/home#/servicehealth" target="_blank" rel="noopener"><span style="font-style: normal; mso-bidi-font-style: italic;">Pārbaudīt pakalpojumu veselības dashboard</span></a>.</span></em></span></span></p>


