---
title: _local_unwind2
ms.date: 11/04/2016
apiname:
- _local_unwind2
apilocation:
- msvcr110_clr0400.dll
- msvcrt.dll
- msvcr100.dll
- msvcr110.dll
- msvcr80.dll
- msvcr90.dll
- msvcr120.dll
apitype: DLLExport
f1_keywords:
- _local_unwind2
- local_unwind2
helpviewer_keywords:
- _local_unwind2 function
- local_unwind2 function
ms.assetid: 44f1fa82-e01e-490f-a6e6-18fc6811c28c
ms.openlocfilehash: 8ae5c3937c9dedc54f0a936b91963419d59f79cc
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/31/2018
ms.locfileid: "50535413"
---
# <a name="localunwind2"></a>_local_unwind2

Función de CRT interna. Ejecuta todos los controladores de finalización que figuran en la tabla de ámbito indicada.

## <a name="syntax"></a>Sintaxis

```
void _local_unwind2(
   PEXCEPTION_REGISTRATION xr,
   int stop
);
```

#### <a name="parameters"></a>Parámetros

*xr*<br/>
[in] Registro asociado a una tabla de ámbito.

*stop*<br/>
[in] Nivel léxico que señala dónde debe detenerse `_local_unwind2`.

## <a name="remarks"></a>Comentarios

Este método solo se usa en el entorno en tiempo de ejecución. No llame a este método en su código.

Cuando este método ejecuta controladores de finalización, comienza en el nivel léxico actual y realiza su recorrido hacia niveles léxicos superiores hasta que alcanza el nivel indicado por `stop`. No ejecuta controladores de finalización situados en el nivel indicado por `stop`.

## <a name="see-also"></a>Vea también

[Referencia alfabética de funciones](../c-runtime-library/reference/crt-alphabetical-function-reference.md)