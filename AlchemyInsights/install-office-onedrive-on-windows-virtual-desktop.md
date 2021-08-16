---
title: Installer Office og OneDrive på Windows virtuelt skrivebord
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 226bd24a955f6165969102c8cf00cf45da537ee05a5363c74f1dfd055d922e1d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028625"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Installer Office og OneDrive på Windows virtuelt skrivebord

1. [Klargjøre og tilpasse et hovedbilde av VHD](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). Opprett en virtuell maskin (VM) hvis den ikke allerede er opprettet.

1. [Installer Office i modus for aktivering av delt datamaskin](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode). Aktivering av delt datamaskin gir flere brukere tilgang til Office.

1. [Installer OneDrive i maskinmodus](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode). Vanligvis er OneDrive installert per bruker, men her bør den installeres per maskin.