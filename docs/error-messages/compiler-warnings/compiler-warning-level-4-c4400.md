---
title: Advertencia del compilador (nivel 4) C4400
ms.date: 11/04/2016
f1_keywords:
- C4400
helpviewer_keywords:
- C4400
ms.assetid: f135fe98-4f92-4e07-9d71-2621b36ee755
ms.openlocfilehash: 61a6d3090355c9bda8aa11c041b302e4ec77ec8d
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/31/2018
ms.locfileid: "50557292"
---
# <a name="compiler-warning-level-4-c4400"></a>Advertencia del compilador (nivel 4) C4400

'type': no se admiten los calificadores const/volatile en este tipo

El [const](../../cpp/const-cpp.md)y [volátil](../../cpp/volatile-cpp.md)calificadores no funcionará con las variables de tipos common language runtime.

## <a name="example"></a>Ejemplo

El ejemplo siguiente genera C4400.

```
// C4400.cpp
// compile with: /clr /W4
// C4401 expected
using namespace System;
#pragma warning (disable : 4101)
int main() {
   const String^ str;   // C4400
   volatile String^ str2;   // C4400
}
```