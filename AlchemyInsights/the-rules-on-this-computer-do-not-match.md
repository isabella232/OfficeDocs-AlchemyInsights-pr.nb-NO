---
title: 'Feil: reglene på denne data maskinen Sams varer ikke'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690972"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="b4522-102">Feil: reglene på denne data maskinen Sams varer ikke</span><span class="sxs-lookup"><span data-stu-id="b4522-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="b4522-103">Hvis du vil se oppdatert status for dette kjente problemet, kan du se [reglene på denne data maskinen Sams varer ikke med reglene for Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="b4522-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="b4522-104">Outlook-teamet har implementert en løsning i bygg 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="b4522-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="b4522-105">Løsningen er allerede på Insider fast, og vil gå til måneds kanal i den seneste juni 2020.</span><span class="sxs-lookup"><span data-stu-id="b4522-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="b4522-106">Når du har den faste versjonen, kan du få spørsmål om at du vil beholde "hvilke regler vil du ha" en siste gang.</span><span class="sxs-lookup"><span data-stu-id="b4522-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="b4522-107">Velg server når du blir bedt om det, og gå deretter tilbake i Outlook, og Aktiver eventuelle regler som ble deaktivert, på nytt.</span><span class="sxs-lookup"><span data-stu-id="b4522-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="b4522-108">Følg denne midlertidige løsningen til løsningen er tilgjengelig:</span><span class="sxs-lookup"><span data-stu-id="b4522-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="b4522-109">**Løsning**: i nylig brukte rapporter har det oppstått et problem for de som bare har opprettet klient regler i skrive bords versjonen av Outlook.</span><span class="sxs-lookup"><span data-stu-id="b4522-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="b4522-110">Hvis du fortsetter å kjøre i problemet, bør du vurdere å slette reglene og deretter opprette og redigere regler bare i OWA (Outlook Web App) til problemet er løst.</span><span class="sxs-lookup"><span data-stu-id="b4522-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="b4522-111">Hvis du ikke kan slette reglene manuelt, kan du kjøre en Outlook-kommando når du starter Outlook ved å kjøre Outlook.exe/Cleanrules.</span><span class="sxs-lookup"><span data-stu-id="b4522-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="b4522-112">Dette vil slette både klient-og server reglene.</span><span class="sxs-lookup"><span data-stu-id="b4522-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="b4522-113">Det vil slette alle reglene for alle kontoene i Outlook-profilen.</span><span class="sxs-lookup"><span data-stu-id="b4522-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="b4522-114">Denne kommandoen er mer dokumentert i artikkelen bytter mellom kommando linjen.</span><span class="sxs-lookup"><span data-stu-id="b4522-114">This command is further documented in the Command-line switches article.</span></span>

