---
title: Feilsøking i forbindelse med tilgang nektes meldinger til OneDrive for forretningsområder
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 42a56b17e41649d979cf442909e8357eb262cf9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35354806"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Feilsøking i forbindelse med tilgang nektes meldinger til OneDrive for forretningsområder

Dette skjer oftest når en bruker slettes og opprettes på nytt med samme brukerhovednavnet (UPN). Den nye kontoen er opprettet ved hjelp av en annen verdi for PUID (unik ID for Passport). Når brukeren prøver å få tilgang til en områdesamling eller sin OneDrive, har brukeren en feil PUID. Andre scenariet omfatter directory-synkronisering med en Active Directory-organisasjonsenhet (OU). Hvis brukere har allerede logget på SharePoint, er flyttet til en annen Organisasjonsenhet og resynced med SharePoint, kan de oppleve dette problemet.

Hvis du vil løse dette problemet, bør du gjenopprette den opprinnelige UPN med trinnene i artikkelen,[gjenopprette en brukers i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Når dette er gjort, kan du kontrollere at brukeren har admin rettigheter til OneDrive området ved å følge fremgangsmåten for å [legge til admin er for en brukers OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Hvis du vil ha mer informasjon om nivåer for tillatelser, kan du se artikkelen, [Forstå tillatelsesnivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
