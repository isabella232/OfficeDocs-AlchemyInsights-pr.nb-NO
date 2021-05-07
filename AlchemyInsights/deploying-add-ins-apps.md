---
title: Distribuere tillegg for Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233543"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Distribuere tillegg for Microsoft 365 Apps

Sentralisert distribusjon er den anbefalte måten å distribuere Office tillegg til brukere og grupper i organisasjonen på. Følg fremgangsmåten nedenfor for å distribuere tillegg:

**Obs!** Hvis du vil installere tillegg for Office som en [enkeltbruker,](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)kan du se Vise, administrere og installere tillegg i Office programmer . Kontroller også at individuelle Office Store tillegg er aktivert. Hvis du vil ha mer informasjon, kan du se Forhindre tilleggsnedlastinger ved å slå av Office Store på tvers av alle klienter [(unntatt Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)

1. Kontroller at miljøet oppfyller kravene for distribusjon av tillegg ved hjelp av sentralisert distribusjon. Hvis du vil ha mer informasjon, kan du se [Krav](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Gå til **Innstillinger**  >  **Integrerte apper** Hent apper i Microsoft 365  >   administrasjonssenteret for å distribuere tillegg. 

Merknader: 

- Integrerte apper krever at administratoren har global administrator eller Exchange administratortillatelser.

- Når du distribuerer tillegg til flere brukere, anbefaler vi å gjøre oppgaver ved hjelp av grupper i stedet for enkeltbrukere. Hvis du vil ha mer informasjon, kan du se Vurderinger når du [tilordner](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)et tillegg til brukere og grupper .

- Sentralisert distribusjon støtter ikke brukere i nestede grupper eller grupper som har overordnede grupper. Hvis du vil ha mer informasjon, [kan du se Bruker- og gruppetilordninger](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).

- Kontroller at Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') er aktivert for brukere å logge på. Hvis du vil ha mer informasjon, [kan du se Konfigurere appegenskaper](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).

- Hvis du opplever problemer med distribusjon av tillegg ved hjelp av integrerte apper, kan du prøve å distribuere ved hjelp [av tillegg](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).

Hvis du vil ha mer informasjon, kan du se:

[Distribuere tillegg i administrasjonssenteret](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Administrere tillegg i administrasjonssenteret](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Bruke PowerShell-cmdleter](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) for sentralisert distribusjon til å administrere tillegg 
 Publisere Office ved hjelp av sentralisert distribusjon via Microsoft 365 [administrasjonssenteret](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Feilsøke: Brukeren ser ikke tillegg](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Feilsøke brukerfeil med Office tillegg](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)