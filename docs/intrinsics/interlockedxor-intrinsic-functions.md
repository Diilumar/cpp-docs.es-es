---
title: Funciones intrínsecas _InterlockedXor
ms.date: 12/17/2018
f1_keywords:
- _InterlockedXor_nf
- _InterlockedXor_np
- _InterlockedXor64_HLERelease
- _InterlockedXor8_acq
- _InterlockedXor64_acq
- _InterlockedXor64_rel
- _InterlockedXor64_nf
- _InterlockedXor_acq
- _InterlockedXor16
- _InterlockedXor64_np
- _InterlockedXor64
- _InterlockedXor_HLEAcquire
- _InterlockedXor_HLERelease
- _InterlockedXor_cpp
- _InterlockedXor16_rel
- _InterlockedXor8_rel
- _InterlockedXor8
- _InterlockedXor64_HLEAcquire
- _InterlockedXor16_nf
- _InterlockedXor16_acq
- _InterlockedXor16_np
- _InterlockedXor8_fn
- _InterlockedXor8_np
- _InterlockedXor64_cpp
- _InterlockedXor_rel
- _InterlockedXor
helpviewer_keywords:
- InterlockedXor intrinsic
- _InterlockedXor64 intrinsic
- InterlockedXor64 intrinsic
- _InterlockedXor intrinsic
ms.assetid: faef1796-cb5a-4430-b1e2-9d5eaf9b4a91
ms.openlocfilehash: 8410420564ae641ff5e624cc5a1ddb0f260672e6
ms.sourcegitcommit: ff3cbe4235b6c316edcc7677f79f70c3e784ad76
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/19/2018
ms.locfileid: "53627382"
---
# <a name="interlockedxor-intrinsic-functions"></a>Funciones intrínsecas _InterlockedXor

**Específicos de Microsoft**

Realiza una operación OR exclusiva (XOR) bit a bit atómica en una variable compartida por varios subprocesos.

## <a name="syntax"></a>Sintaxis

```
long _InterlockedXor(
   long volatile * Value,
   long Mask
);
long _InterlockedXor_acq(
   long volatile * Value,
   long Mask
);
long _InterlockedXor_HLEAcquire(
   long volatile * Value,
   long Mask
);
long _InterlockedXor_HLERelease(
   long volatile * Value,
   long Mask
);
long _InterlockedXor_nf(
   long volatile * Value,
   long Mask
);
long _InterlockedXor_np(
   long volatile * Value,
   long Mask
);
long _InterlockedXor_rel(
   long volatile * Value,
   long Mask
);
char _InterlockedXor8(
   char volatile * Value,
   char Mask
);
char _InterlockedXor8_acq(
   char volatile * Value,
   char Mask
);
char _InterlockedXor8_nf(
   char volatile * Value,
   char Mask
);
char _InterlockedXor8_np(
   char volatile * Value,
   char Mask
);
char _InterlockedXor8_rel(
   char volatile * Value,
   char Mask
);
short _InterlockedXor16(
   short volatile * Value,
   short Mask
);
short _InterlockedXor16_acq(
   short volatile * Value,
   short Mask
);
short _InterlockedXor16_nf (
   short volatile * Value,
   short Mask
);
short _InterlockedXor16_np (
   short volatile * Value,
   short Mask
);
short _InterlockedXor16_rel(
   short volatile * Value,
   short Mask
);
__int64 _InterlockedXor64(
   __int64 volatile * Value,
   __int64 Mask
);
__int64 _InterlockedXor64_acq(
   __int64 volatile * Value,
   __int64 Mask
);
__int64 _InterlockedXor64_HLEAcquire(
   __int64 volatile * Value,
   __int64 Mask
);
__int64 _InterlockedXor64_HLERelease(
   __int64 volatile * Value,
   __int64 Mask
);
__int64 _InterlockedXor64_nf(
   __int64 volatile * Value,
   __int64 Mask
);
__int64 _InterlockedXor64_np(
   __int64 volatile * Value,
   __int64 Mask
);
__int64 _InterlockedXor64_rel(
   __int64 volatile * Value,
   __int64 Mask
);
```

#### <a name="parameters"></a>Parámetros

*Valor*<br/>
[in, out] Un puntero al primer operando, sean reemplazadas por el resultado.

*Máscara*<br/>
[in] El segundo operando.

## <a name="return-value"></a>Valor devuelto

El valor original del primer operando.

## <a name="requirements"></a>Requisitos

|Función intrínseca|Arquitectura|Encabezado|
|---------------|------------------|------------|
|`_InterlockedXor`, `_InterlockedXor8`, `_InterlockedXor16`, `_InterlockedXor64`|x86, ARM, x64|\<INTRIN.h >|
|`_InterlockedXor_acq`, `_InterlockedXor_nf`, `_InterlockedXor_rel`, `_InterlockedXor8_acq`, `_InterlockedXor8_nf`, `_InterlockedXor8_rel`, `_InterlockedXor16_acq`, `_InterlockedXor16_nf`, `_InterlockedXor16_rel`, `_InterlockedXor64_acq`, `_InterlockedXor64_nf`, `_InterlockedXor64_rel`,|ARM|\<INTRIN.h >|
|`_InterlockedXor_np`, `_InterlockedXor8_np`, `_InterlockedXor16_np`, `_InterlockedXor64_np`|x64|\<INTRIN.h >|
|`_InterlockedXor_HLEAcquire`, `_InterlockedXor_HLERelease`, `_InterlockedXor64_HLEAcquire`, `_InterlockedXor64_HLERelease`|x86, x64|\<immintrin.h >|

## <a name="remarks"></a>Comentarios

El número en el nombre de cada función especifica el tamaño en bits de los argumentos.

En plataformas ARM, utilice los intrínsecos con sufijos `_acq` y `_rel` si necesita adquirir y liberar semántica, como al principio y al final de una sección crítica. Los intrínsecos ARM con un sufijo `_nf` ("sin límite") no actúan como una barrera de memoria.

Los intrínsecos con un sufijo `_np` ("sin captura previa") impiden que el compilador inserte una posible operación de captura previa.

En las plataformas de Intel que admiten instrucciones de Elisión de bloqueo de Hardware (HLE), los intrínsecos con sufijos `_HLEAcquire` y `_HLERelease` incluyen una sugerencia para el procesador que puede acelerar el rendimiento mediante la eliminación de un paso de escritura de bloqueo en el hardware. Si se llama a estos intrínsecos en plataformas que no son compatibles con HLE, se omite la sugerencia.

## <a name="example"></a>Ejemplo

```
// _InterLockedXor.cpp
#include <stdio.h>
#include <intrin.h>

#pragma intrinsic(_InterlockedXor)

int main()
{
        long data1 = 0xFF00FF00;
        long data2 = 0x00FFFF00;
        long retval;
        retval = _InterlockedXor(&data1, data2);
        printf_s("0x%x 0x%x 0x%x", data1, data2, retval);
}
```

```Output
0xffff0000 0xffff00 0xff00ff00
```

**FIN de Específicos de Microsoft**

## <a name="see-also"></a>Vea también

[Intrínsecos del controlador](../intrinsics/compiler-intrinsics.md)<br/>
[Conflictos con el compilador de x86](../build/x64-software-conventions.md#conflicts-with-the-x86-compiler)