---
title: Error de las herramientas del vinculador LNK1241
ms.date: 11/04/2016
f1_keywords:
- LNK1241
helpviewer_keywords:
- LNK1241
ms.assetid: 7b8b52eb-0231-4521-b52a-2bce8d3e8956
ms.openlocfilehash: 87f73680d7ed40b9b2db9f40f9140976d552ab6b
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/31/2018
ms.locfileid: "50584553"
---
# <a name="linker-tools-error-lnk1241"></a>Error de las herramientas del vinculador LNK1241

archivo de recursos ' resource' ya se especificó

Este error se genera si ejecuta **cvtres** manualmente desde la línea de comandos y si, a continuación, pase el archivo .obj resultante del archivo al vinculador además a otros archivos. res.

Para especificar varios archivos. res, pase todo al vinculador como archivos, no desde los archivos .obj crean por **cvtres**.