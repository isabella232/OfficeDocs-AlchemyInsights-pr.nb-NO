---
title: Feilsøke OneDrive-krasj
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665007"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="f8252-102">Feilsøke OneDrive-krasj</span><span class="sxs-lookup"><span data-stu-id="f8252-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="f8252-103">Hvis OneDrive krasjer gjentatte ganger, kan du prøve disse feil søkings trinnene:</span><span class="sxs-lookup"><span data-stu-id="f8252-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="f8252-104">**Kontroller at Register nøkler ikke er angitt:**</span><span class="sxs-lookup"><span data-stu-id="f8252-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="f8252-105">Bruk register redigering til å gå til HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="f8252-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="f8252-106">Hvis DisableFileSyncNGSC finnes og satt til 1, åpner du nøkkelen og endrer verdien til 0.</span><span class="sxs-lookup"><span data-stu-id="f8252-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="f8252-107">Start OneDrive manuelt ved å gå til Start</span><span class="sxs-lookup"><span data-stu-id="f8252-107">Manually launch OneDrive by going to Start</span></span> ![Trykk Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="f8252-109">, Skriv inn OneDrive i søke boksen, og klikk deretter på skrive bords programmet OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f8252-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="f8252-110">**Tilbakestill OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="f8252-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="f8252-111">Merknader</span><span class="sxs-lookup"><span data-stu-id="f8252-111">Notes:</span></span>

- <span data-ttu-id="f8252-112">Hvis du tilbakestiller OneDrive, kobles alle de eksisterende synkroniserings tilkoblingene fra (inkludert din personlige OneDrive hvis den er konfigurert).</span><span class="sxs-lookup"><span data-stu-id="f8252-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="f8252-113">Du mister ikke filer eller data ved å tilbakestille OneDrive på data maskinen.</span><span class="sxs-lookup"><span data-stu-id="f8252-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="f8252-114">**Slik tilbakestiller du OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="f8252-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="f8252-115">Åpne en Kjør-dialogboks ved å trykke Windows-tasten og R.</span><span class="sxs-lookup"><span data-stu-id="f8252-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="f8252-116">Skriv inn% localappdata% \Microsoft\OneDrive\onedrive.exe/reset, og trykk OK.</span><span class="sxs-lookup"><span data-stu-id="f8252-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="f8252-117">Et kommando vindu kan vises kort.</span><span class="sxs-lookup"><span data-stu-id="f8252-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="f8252-118">Start OneDrive manuelt ved å gå til Start</span><span class="sxs-lookup"><span data-stu-id="f8252-118">Manually launch OneDrive by going to Start</span></span> ![Trykk Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="f8252-120">, Skriv inn OneDrive i søke boksen, og klikk deretter på skrive bords programmet OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f8252-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="f8252-121">Merknader</span><span class="sxs-lookup"><span data-stu-id="f8252-121">Notes:</span></span>

- <span data-ttu-id="f8252-122">Hvis du har valgt å synkronisere bare enkelte mapper før du tilbakestiller, må du gjøre det på nytt når synkroniseringen er fullført.</span><span class="sxs-lookup"><span data-stu-id="f8252-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="f8252-123">Les [velge hvilke OneDrive-mapper som skal synkroniseres til data maskinen](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="f8252-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="f8252-124">Du må fullføre dette for din personlige OneDrive og OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="f8252-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>