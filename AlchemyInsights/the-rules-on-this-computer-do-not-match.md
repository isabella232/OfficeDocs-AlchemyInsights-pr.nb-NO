---
title: 'Feil: Reglene på denne datamaskinen samsvarer ikke'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664255"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="ddbf7-102">Feil: Reglene på denne datamaskinen samsvarer ikke</span><span class="sxs-lookup"><span data-stu-id="ddbf7-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="ddbf7-103">Hvis du vil se oppdatert status for dette kjente problemet, kan du se [Reglene på denne datamaskinen samsvarer ikke med reglene for Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="ddbf7-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="ddbf7-104">Outlook-teamet har implementert en løsning i Build 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="ddbf7-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="ddbf7-105">Løsningen er allerede på Insider Fast og vil gå til Månedlig kanal i slutten av juni 2020.</span><span class="sxs-lookup"><span data-stu-id="ddbf7-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="ddbf7-106">Når du har den faste builden, kan du få meldingen "Hvilke regler vil du beholde" en siste gang.</span><span class="sxs-lookup"><span data-stu-id="ddbf7-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="ddbf7-107">Velg Server når du blir bedt om det, og gå deretter tilbake i Outlook og aktivere alle regler som ble deaktivert på nytt.</span><span class="sxs-lookup"><span data-stu-id="ddbf7-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="ddbf7-108">Til hurtigreparasjonen er tilgjengelig, bruk følgende løsning:</span><span class="sxs-lookup"><span data-stu-id="ddbf7-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="ddbf7-109">**Løsning**: Det har oppstått problemet for de som bare har opprettet klientregler i Outlook-skrivebordet i nylige rapporter.</span><span class="sxs-lookup"><span data-stu-id="ddbf7-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="ddbf7-110">Hvis du fortsatt støter på problemet, kan du vurdere å slette reglene og deretter opprette og redigere regler bare i OWA (Outlook Web App) til problemet er løst.</span><span class="sxs-lookup"><span data-stu-id="ddbf7-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="ddbf7-111">Hvis du ikke kan slette reglene manuelt, kan du kjøre en Outlook-kommando når du starter Outlook ved å kjøre Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="ddbf7-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="ddbf7-112">Dette sletter både klient- og serverreglene.</span><span class="sxs-lookup"><span data-stu-id="ddbf7-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="ddbf7-113">Det vil slette alle reglene for alle kontoene i Outlook-profilen.</span><span class="sxs-lookup"><span data-stu-id="ddbf7-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="ddbf7-114">Denne kommandoen er ytterligere dokumentert i command-line brytere artikkelen.</span><span class="sxs-lookup"><span data-stu-id="ddbf7-114">This command is further documented in the Command-line switches article.</span></span>

