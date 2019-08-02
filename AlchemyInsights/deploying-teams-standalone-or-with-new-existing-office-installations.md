---
title: Distribusjon av grupper som frittstående eller med nye eller eksisterende Office-installasjoner
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054239"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Distribusjon av grupper som frittstående eller med nye eller eksisterende Office-installasjoner

Microsoft-Teams er nå inkludert som en del av ***nye installasjoner*** av Office 365 ProPlus Office 365 Business og Office for Mac. Hvis du vil ha mer informasjon, se [når Microsoft Teams starter som følger med nye installasjoner av Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

I tillegg vil starter med versjon 1906 i månedlig kanal, Team bli ***lagt til i eksisterende installasjoner*** av Office 365 ProPlus (og Office 365 Business) på enheter som kjører Windows, når du oppdaterer den eksisterende installasjonen til den nyeste versjonen. Hvis du vil ha mer informasjon, se [Hva med eksisterende installasjoner av Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Hvis du ikke vil vente til denne tidsplanen for distribusjonen, kan du distribuere team som frittstående for brukerne ved å [følge disse instruksjonene](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) eller du kan la brukerne installere Team for seg selv fra [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Hvis organisasjonen ikke er klar til å distribuere team, har vi trinnene du kan gjøre for å ***utelate Team*** fra [Ny](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) eller [eksisterende](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installasjoner av Office. Hvis du vil at grupper kan installeres, men ikke vil bruke grupper til å starte automatisk for brukeren når den er installert, kan du se [At Microsoft Team starter automatisk etter installasjonen](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

***Avinstallere grupper*** fra en enhet som kjører Windows, kan du se [Avinstallere Microsoft Team](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). For opprydding Microsoft Teams fra flere målmaskiner eller brukere, kan du se [Microsoft Team distribusjon opprydding](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Hvis du bruker delte datamaskiner, Remote Desktop Services (RDS) eller virtuelle skrivebordet infrastruktur (VDI), kan du se [delt datamaskin og VDI miljøer med Microsoft Team](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Hvis du bruker Office for Mac, kan du se [Microsoft Team installasjoner på en Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Når Team er installert, er det [automatisk oppdatert](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) omtrent annenhver uke med nye funksjoner og oppdateringer for kvalitet. 