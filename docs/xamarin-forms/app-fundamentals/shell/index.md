---
title: Xamarin.Forms-Shell
description: Dieser Leitfaden erklärt, wie die Xamarin.Forms-Shell verwendet wird, und wie sich die Komplexität von Xamarin.Forms-Anwendungen reduzieren lässt, indem sie die grundlegenden Funktionen bereitstellt, die die meisten Anwendungen benötigen.
ms.prod: xamarin
ms.assetid: 85B322AA-808F-41B6-953A-5877264AE643
ms.technology: xamarin-forms
author: davidbritch
ms.author: dabritch
ms.date: 05/06/2019
ms.openlocfilehash: 7699b39a6df6c64ae9a481d9171f23dc6a8eba57
ms.sourcegitcommit: 9d90a26cbe13ebd106f55ba4a5445f28d9c18a1a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/06/2019
ms.locfileid: "65054190"
---
# <a name="xamarinforms-shell"></a>Xamarin.Forms-Shell

![](~/media/shared/preview.png "Diese API ist derzeit als Vorabversion erhältlich")

## <a name="introductionintroductionmd"></a>[Introduction (Einführung)](introduction.md)

Die Xamarin.Forms-Shell reduziert die Komplexität der Entwicklung mobiler Anwendungen, indem es die grundlegenden Features bereitstellt, die die meisten mobilen Anwendungen benötigen. Dazu gehören eine gemeinsame Navigationsbenutzerumgebung, ein URI-basiertes Navigationsschema und ein integrierter Suchhandler.

## <a name="flyoutflyoutmd"></a>[Flyout](flyout.md)

Das Flyout ist das Hauptmenü für eine Shell-Anwendung, und der Zugriff erfolgt über ein Symbol oder durch Wischen von einer Seite des Bildschirms. Das Flyout besteht aus einem optionalen Header, Flyout-Elementen und optionalen Menüelementen.

## <a name="tabstabsmd"></a>[Registerkarten](tabs.md)

Nach einem Flyout ist die nächste Navigationsebene in einer Shell-Anwendung die untere Registerkartenleiste. Wenn eine Registerkarte mehrere Seiten enthält, sind die Seiten über Register am oberen Rand navigierbar.

## <a name="navigationnavigationmd"></a>[Navigation](navigation.md)

Shell-Anwendungen können ein URI-basiertes Navigationsschema nutzen, das Routen verwendet, um zu einer beliebigen Seite in der Anwendung zu navigieren, ohne einer festen Navigationshierarchie folgen zu müssen.

## <a name="searchsearchmd"></a>[Suchen](search.md)

Shell-Anwendungen können integrierte Suchfunktionalität über ein Suchfeld nutzen, das oben auf jeder Seite hinzugefügt werden kann.

## <a name="custom-rendererscustomrenderersmd"></a>[Benutzerdefinierte Renderer](customrenderers.md)

Shell-Anwendungen sind über die von den verschiedenen Shell-Klassen bereitgestellten Eigenschaften und Methoden äußerst anpassbar. Allerdings ist es auch möglich, einen benutzerdefinierten Shell-Renderer zu erstellen, wenn komplexere plattformspezifische Anpassungen erforderlich sind.