---
title: Utstede åpning eller nedlasting av filer i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148335"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Utstede åpning eller nedlasting av filer i Yammer

Classic Yammer støtter flere alternativer for filopplastinger til meldinger og grupper. Avhengig av nettverkskonfigurasjon, filer som er standard til lagring i SharePoint.

Filvelgeren i nye Yammer støtter ennå ikke alle alternativene som er tilgjengelige i klassisk Yammer. En fremtidig oppdatering vil legge til flere funksjoner. Hvis du vil ha mer informasjon, kan du se [Legge ved en fil eller et bilde i et Yammer-samtaleinnlegg](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Kan ikke åpne eller laste ned en fil**  

En fil kan laste opp til Yammer, men også koble til en fil i SharePoint Online. Hvis du vil feilsøke, må du først bestemme plasseringen av filen. Hvis filen er lastet opp til Yammer, vil den ha en *.yammer.com URL-adresse. Kontroller at nødvendige URL-adresser og IP-adresser er blokkert. Hvis du vil ha mer informasjon, kan du se blogginnlegget [Ved hjelp av hardkodede IP-adresser for Yammer anbefales ikke](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Kontroller om en bruker som også er en global administrator, kan laste ned filen. Hvis filen er privat, må du kanskje bruke modus for privat innhold. Hvis du vil ha mer informasjon, kan du se [Overvåke privat innhold i Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Yammer-gjester og -filer på nettverksnivå i SharePoint Online**  

[Gjester på nettverksnivå i Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) bruker ikke Azure AD B2B og er interne for Yammer-tjenesten, slik at de ikke får tilgang til Yammer-filer som er lagret i SharePoint. Opprett en ekstern AAD B2B-bruker som har tilgang til dokumentbiblioteker i SharePoint Online ved hjelp av denne identiteten. Hvis du vil ha informasjon om fremtidig kundestøtte for Azure AD B2B-gjester i Yammer, kan du se [Kundestøtte for Business-to-business (B2B) i Yammer Preview – Kundevilkår og vanlige spørsmål](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).