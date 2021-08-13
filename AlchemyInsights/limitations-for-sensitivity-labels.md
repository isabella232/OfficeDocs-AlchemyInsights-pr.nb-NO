---
title: Begrensninger for følsomhetsetiketter for Office filer i SharePoint og OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813161"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Begrensninger for følsomhetsetiketter for Office filer i SharePoint og OneDrive

Når du aktiverer følsomhetsetiketter for Office filer i SharePoint og OneDrive, må du være oppmerksom på krav og begrensninger, som omfatter:

- SharePoint og OneDrive kan ikke behandle noen filer merket og kryptert fra Office-skrivebordsprogrammer når filene inneholder PowerQuery-data, data som er lagret av egendefinerte tillegg eller egendefinerte XML-deler.
- SharePoint og OneDrive ikke bruker følsomhetsetiketter automatisk på eksisterende filer du allerede har kryptert ved hjelp av Azure Information Protection (AIP)-etiketter. Slik bruker du følsomhetsetiketter på krypterte filer: 
    - Kontroller at AIP-etiketter er overført og publisert til samsvarssenteret Microsoft 365.
    - Last ned de merkede filene, og last dem deretter opp til den opprinnelige SharePoint eller OneDrive plasseringen.
- Utskrift støttes ikke for krypterte dokumenter.

Hvis du vil ha mer informasjon om begrensninger, kan du se Aktivere følsomhetsetiketter for Office [filer i SharePoint og OneDrive](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations).
