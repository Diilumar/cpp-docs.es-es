---
title: Compilador advertencia (nivel 1) C4183
ms.date: 11/04/2016
f1_keywords:
- C4183
helpviewer_keywords:
- C4183
ms.assetid: dc48312c-4b34-44dd-80ff-eb5f11d5ca47
ms.openlocfilehash: 0d947a0f6d777a5ed3191d6d232a604028be2003
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/31/2018
ms.locfileid: "50477459"
---
# <a name="compiler-warning-level-1-c4183"></a>Compilador advertencia (nivel 1) C4183

'identifier': falta el tipo de valor devuelto; supone que una función miembro devuelve 'int'

La definición en línea de una función miembro en una clase o una estructura no tiene un tipo de valor devuelto. Esta función miembro se supone que tiene un valor predeterminado a tipo de valor devuelto `int`.

El ejemplo siguiente genera C4183:

```
// C4183.cpp
// compile with: /W1 /c
#pragma warning(disable : 4430)
class MyClass1;
class MyClass2 {
   MyClass1() {};   // C4183
};
```