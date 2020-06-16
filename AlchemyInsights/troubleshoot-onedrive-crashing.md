---
title: Feilsøke OneDrive-krasj
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749163"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="98d11-102">Feilsøke OneDrive-krasj</span><span class="sxs-lookup"><span data-stu-id="98d11-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="98d11-103">Hvis OneDrive krasjer gjentatte ganger, kan du prøve disse feilsøkingstrinnene:</span><span class="sxs-lookup"><span data-stu-id="98d11-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="98d11-104">**Kontroller at registernøkler ikke er angitt:**</span><span class="sxs-lookup"><span data-stu-id="98d11-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="98d11-105">Bruk Registerredigering til å gå til HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="98d11-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="98d11-106">Hvis DisableFileSyncNGSC finnes og satt til 1, åpner du nøkkelen og endrer verdien til 0.</span><span class="sxs-lookup"><span data-stu-id="98d11-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="98d11-107">Start OneDrive manuelt ved å gå til Start</span><span class="sxs-lookup"><span data-stu-id="98d11-107">Manually launch OneDrive by going to Start</span></span> ![Trykk Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="98d11-109">, skriv inn OneDrive i søkeboksen, og klikk deretter på OneDrive-skrivebordsappen.</span><span class="sxs-lookup"><span data-stu-id="98d11-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="98d11-110">**Tilbakestill OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="98d11-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="98d11-111">Notater:</span><span class="sxs-lookup"><span data-stu-id="98d11-111">Notes:</span></span>

- <span data-ttu-id="98d11-112">Tilbakestilling av OneDrive kobler fra alle eksisterende synkroniseringstilkoblinger (inkludert din personlige OneDrive hvis konfigurert).</span><span class="sxs-lookup"><span data-stu-id="98d11-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="98d11-113">Du vil ikke miste filer eller data ved å tilbakestille OneDrive på datamaskinen.</span><span class="sxs-lookup"><span data-stu-id="98d11-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="98d11-114">**Slik tilbakestiller du OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="98d11-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="98d11-115">Åpne en Kjør-dialogboks ved å trykke Windows-tasten og R.</span><span class="sxs-lookup"><span data-stu-id="98d11-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="98d11-116">Skriv inn %localappdata%\Microsoft\OneDrive\onedrive.exe /reset, og trykk på OK.</span><span class="sxs-lookup"><span data-stu-id="98d11-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="98d11-117">Et kommandovindu kan vises kort.</span><span class="sxs-lookup"><span data-stu-id="98d11-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="98d11-118">Start OneDrive manuelt ved å gå til Start</span><span class="sxs-lookup"><span data-stu-id="98d11-118">Manually launch OneDrive by going to Start</span></span> ![Trykk Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="98d11-120">, skriv inn OneDrive i søkeboksen, og klikk deretter på OneDrive-skrivebordsappen.</span><span class="sxs-lookup"><span data-stu-id="98d11-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="98d11-121">Notater:</span><span class="sxs-lookup"><span data-stu-id="98d11-121">Notes:</span></span>

- <span data-ttu-id="98d11-122">Hvis du hadde valgt å synkronisere bare noen mapper før tilbakestillingen, må du gjøre det igjen når synkroniseringen er fullført.</span><span class="sxs-lookup"><span data-stu-id="98d11-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="98d11-123">Les [Velg hvilke OneDrive-mapper som skal synkroniseres med datamaskinen,](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   hvis du vil ha mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="98d11-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="98d11-124">Du må fullføre dette for din personlige OneDrive og OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="98d11-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>