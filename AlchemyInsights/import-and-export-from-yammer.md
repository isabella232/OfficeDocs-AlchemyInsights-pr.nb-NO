---
title: Importere og eksportere fra Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036120"
---
# <a name="import-and-export-from-yammer"></a>Importere og eksportere fra Yammer

**Importer**

Alternativene for brukerimport varierer avhengig av om Yammer-nettverket er i [opprinnelig modus for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)eller ikke.

- **Ikke-opprinnelig modus:** Brukere kan importeres til grupper ved hjelp av Legg til fra adresseboken (grense til 100 brukere) i gruppeinnstillinger, eller til nettverket ved hjelp av masseoppdatering i Nettverksadministrator. [](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) [](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users)
- **Opprinnelig modus:** Operasjoner for gruppemedlemskap og nettverksmedlemskap bør utføres fra administrasjonsportalen for [Microsoft 365,](https://docs.microsoft.com/microsoft-365/admin/add-users) [Azure AD-portalen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)eller ved hjelp av et annet Azure AD-alternativ. Nettverk i opprinnelig modus har ikke lenger tilgang til masseoppdatering og andre eldre funksjoner.

> [!IMPORTANT]
> Yammer støttet aldri import av innhold fra nettverksadministratoren selv når dataeksportfunksjonen ble brukt i et annet nettverk. Innhold kan publiseres på nytt av partnerløsninger eller YAMMER REST API-er.

**Eksporter**

[Eksporter nettverksdata i Nettverksadministrator](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) tillater eksport av innhold fra Yammer-nettverk, inkludert meldinger og filer. Vedlegg kan være svært store, og det vil føre til at eksporten tar betydelig tid å fullføre. Vi anbefaler at aktive nettverk eksporteres ved hjelp av [dataeksport-API-en](https://developer.yammer.com/docs/data-export-api) i biter etter dag eller uke. Microsoft Kundestøtte tilbyr ikke egendefinerte skript til dette formålet.

Det finnes [en egen GDPR-eksport](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) for å eksportere innhold for en enkeltbruker.