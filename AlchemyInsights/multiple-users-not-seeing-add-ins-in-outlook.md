---
title: Flere brukere ser ikke tillegg i Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197980"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Flere brukere ser ikke tillegg i Outlook

Hvis du tester Outlook-tillegg og ingen vises, bruker du cmdleten **Get-OrganizationConfig** PowerShell til å spørre _parameteren AppsForOfficeEnabled_ som første feilsøking. Hvis spørringen returnerer en verdi av **Usann**, setter du denne parameteren til **True** ved hjelp av cmdleten **Set-OrganizationConfig,** slik at tillegg vises som forventet.

Vi anbefaler ikke at _parameteren AppsForOfficeEnabled_ er satt til **False**. Verdien **False** overstyrer alle de ovennevnte administrative og brukerrolleinnstillingene og hindrer at nye apper aktiveres av en bruker i organisasjonen.

Hvis du vil ha mer informasjon, kan du se [Angi administratorer og brukere som kan installere og administrere tillegg for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).