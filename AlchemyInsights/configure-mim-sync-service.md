---
title: Konfigurere MIM-synkroniseringstjenesten
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481869"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="0dff4-102">Konfigurere MIM-synkroniseringstjenesten</span><span class="sxs-lookup"><span data-stu-id="0dff4-102">Configure MIM Sync service</span></span>

<span data-ttu-id="0dff4-103">Synkroniseringstjenesten for Microsoft Identity Manager (MIM) er en komponent i MIM.</span><span class="sxs-lookup"><span data-stu-id="0dff4-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="0dff4-104">Det er en sentralisert lokal tjeneste som lagrer og integrerer informasjon for organisasjoner som har flere lokale kataloger og databaser.</span><span class="sxs-lookup"><span data-stu-id="0dff4-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="0dff4-105">Du kan kanskje løse problemet med MIM-synkronisering hvis problemet ble løst i en nylig oppdatering til MIM eller er et av de andre problemene som nevnes i avsnittet nedenfor.</span><span class="sxs-lookup"><span data-stu-id="0dff4-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="0dff4-106">**Anbefalte trinn**</span><span class="sxs-lookup"><span data-stu-id="0dff4-106">**Recommended steps**</span></span>

1. <span data-ttu-id="0dff4-107">Kontroller at du bruker en nylig oppdatering av MIM-synkronisering, og se produktmerknene for [MIM-synkronisering](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) for å finne ut om problemet er løst i en oppdatering.</span><span class="sxs-lookup"><span data-stu-id="0dff4-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="0dff4-108">Hvis problemet ligger i koblingene Generic LDAP, Generic SQL, Lotus Domino eller Web Services, må du kontrollere at du bruker en nylig oppdatering av de [generiske koblingene.](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)</span><span class="sxs-lookup"><span data-stu-id="0dff4-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="0dff4-109">Hvis en MIM-synkroniseringskjøring stopper med en [](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) feil, kan du se i feiltabellen for å finne potensielle årsaker.</span><span class="sxs-lookup"><span data-stu-id="0dff4-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="0dff4-110">Hvis kjøringen stopper med **extension-dll-exception,** klikker du på disse ordene for å åpne vinduet for egenskaper for koblingsområdeobjektet, og klikker på **Stack Trace...** for å se mer informasjon om den underliggende årsaken, som beskrevet i [Extension-DLL-Exception.](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx) </span><span class="sxs-lookup"><span data-stu-id="0dff4-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="0dff4-111">Hvis PCNS-komponenten (Password Change Notification Service) rapporterer feil **6025** i hendelsesloggen under passordsynkronisering, kan du se i veiledningen for feilsøking av [PCNS-rapportfeil 6025.](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)</span><span class="sxs-lookup"><span data-stu-id="0dff4-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="0dff4-112">Hvis full synkronisering med FIM Service Management  Agent er treg, kontrollerer du innstillingen for automatisk vekst for TempDB, som beskrevet i Feilsøking av treg eller [hengende full synkronisering.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)</span><span class="sxs-lookup"><span data-stu-id="0dff4-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="0dff4-113">Hvis det oppstår en feil med server som har blitt stoppet, med mislykket oppretting via nettjenester ved hjelp av FIM Service Management Agent, kan du se [Støtteinformasjon: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for å få en oversikt over årsaker.</span><span class="sxs-lookup"><span data-stu-id="0dff4-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

