---
title: Error grave de NMAKE U1073
ms.date: 11/04/2016
f1_keywords:
- U1073
helpviewer_keywords:
- U1073
ms.assetid: d46bf2dd-400a-4802-9db2-f832e1c97f02
ms.openlocfilehash: 2aa02fd86906bd545373a313fa5e6e409ffb3cf9
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/31/2018
ms.locfileid: "50582278"
---
# <a name="nmake-fatal-error-u1073"></a>Error grave de NMAKE U1073

no sabe cómo hacer 'nombrededestino'

El destino especificado no existe y no hay ningún comando para ejecutar o reglas de inferencia se aplican.

### <a name="to-fix-by-using-the-following-possible-solutions"></a>Use las soluciones posibles siguientes para corregirlo

1. Compruebe la ortografía del nombre de destino.

1. Si *targetname* es un pseudodestino, especifíquelo como un destino en otro bloque de descripción.

1. Si *targetname* es una llamada de macro, asegúrese de que no se expande a una cadena nula.