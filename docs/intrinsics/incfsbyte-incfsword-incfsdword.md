---
title: __incfsbyte, __incfsword, __incfsdword
ms.date: 11/04/2016
f1_keywords:
- __incfsword
- __incfsbyte_cpp
- __incfsbyte
- __incfsdword
- __incfsword_cpp
- __incfsdword_cpp
helpviewer_keywords:
- __incfsword intrinsic
- __incfsdword intrinsic
- __incfsbyte intrinsic
ms.assetid: 820457fb-e35e-42d3-bcb6-725da3281c64
ms.openlocfilehash: f9f0bef89b32e1901c2f6b173baa90153b25a71d
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/31/2018
ms.locfileid: "50577912"
---
# <a name="incfsbyte-incfsword-incfsdword"></a>__incfsbyte, __incfsword, __incfsdword

**Específicos de Microsoft**

Agregue uno para el valor en una ubicación de memoria especificada por un desplazamiento relativo al principio de la `FS` segmento.

## <a name="syntax"></a>Sintaxis

```
void __incfsbyte(
   unsigned long Offset
);
void __incfsword(
   unsigned long Offset
);
void __incfsdword(
   unsigned long Offset
);
```

#### <a name="parameters"></a>Parámetros

*Desplazamiento*<br/>
[in] El desplazamiento desde el principio del `FS`.

## <a name="requirements"></a>Requisitos

|Función intrínseca|Arquitectura|
|---------------|------------------|
|`__incfsbyte`|x86|
|`__incfsword`|x86|
|`__incfsdword`|x86|

## <a name="remarks"></a>Comentarios

Estas funciones intrínsecas solo están disponibles en modo kernel, y las rutinas solo están disponibles como intrínsecos.

**FIN de Específicos de Microsoft**

## <a name="see-also"></a>Vea también

[__addfsbyte, \__addfsword, \__addfsdword](../intrinsics/addfsbyte-addfsword-addfsdword.md)<br/>
[__readfsbyte, \__readfsdword, \__readfsqword, \__readfsword](../intrinsics/readfsbyte-readfsdword-readfsqword-readfsword.md)<br/>
[__writefsbyte, \__writefsdword, \__writefsqword, \__writefsword](../intrinsics/writefsbyte-writefsdword-writefsqword-writefsword.md)<br/>
[Intrínsecos del controlador](../intrinsics/compiler-intrinsics.md)