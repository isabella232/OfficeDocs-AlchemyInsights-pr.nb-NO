---
title: Feilsøking av tilgang nektet meldinger til OneDrive for Business-områder
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051614"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Feilsøking av tilgang nektet meldinger til OneDrive for Business-områder

Dette problemet oppstår hyppigst når en bruker slettes og opprettes på nytt med samme hovednavn for bruker (UPN). Den nye kontoen opprettes ved hjelp av en annen verdi for PUID (Passport Unique ID). Når brukeren prøver å få tilgang til en områdesamling eller deres OneDrive, har brukeren en feil PUID. Et annet scenario omfatter katalogsynkronisering med en organisasjonsenhet for Active Directory (OU). Hvis brukere allerede har logget på SharePoint, og deretter flyttes til en annen ORGANISASJONSENHET og resynced med SharePoint, kan de oppleve dette problemet.

1. Hvis du vil løse dette problemet, bør du gjenopprette den opprinnelige UPN med trinnene i artikkelen, [gjenopprette en bruker i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Hvis du ikke kan gjenopprette den opprinnelige brukeren, bør du fjerne den gamle brukeren fra OneDrive-området ved hjelp av disse trinnene, [fjerne en bruker fra listen over bruker informasjon](). 
3. Når dette er gjort, kan du kontrollere at brukeren har admin rettigheter til OneDrive-området ved å følge fremgangsmåten for å [legge til admin for en brukers OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Hvis du vil ha mer informasjon om tillatelsesnivåer, kan du se artikkelen [forstå tillatelsesnivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
