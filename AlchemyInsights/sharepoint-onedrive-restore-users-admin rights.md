---
title: Feilsøke tilgang nektet meldinger til OneDrive for Business-områder
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670625"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Feilsøke tilgang nektet meldinger til OneDrive for Business-områder

Dette problemet oppstår oftest når en bruker slettes og opprettes på nytt med samme brukerhovednavn (UPN). Den nye kontoen opprettes ved hjelp av en annen PUID-verdi (konto – unik ID). Når brukeren prøver å få tilgang til en område samling eller deres OneDrive, har brukeren feil PUID. Et annet scenario omfatter katalog synkronisering med en Active Directory-organisasjonsenhet (OU). Hvis brukerne allerede har logget seg på SharePoint, og deretter flyttes til en annen OU og synkroniseres med SharePoint, kan de oppleve dette problemet.

1. Hvis du vil løse dette problemet, må du gjenopprette den opprinnelige UPN-en med trinnene i artikkelen, [gjenopprette en bruker i Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Hvis du ikke kan gjenopprette den opprinnelige brukeren, må du fjerne den gamle brukeren fra OneDrive-nettstedet ved hjelp av disse trinnene, [fjerne en bruker fra bruker informasjons listen](). 
3. Når dette er gjort, kan du kontrollere at brukeren har administrator rettigheter til OneDrive-nettstedet ved å følge Fremgangs måten [for å legge til administrator for en brukers OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Hvis du vil ha mer informasjon om tillatelses nivåer, kan du se artikkelen [forstå tilgangs nivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
