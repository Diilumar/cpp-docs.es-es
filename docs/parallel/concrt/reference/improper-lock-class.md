---
title: improper_lock (Clase)
ms.date: 11/04/2016
f1_keywords:
- improper_lock
- CONCRT/concurrency::improper_lock
- CONCRT/concurrency::improper_lock::improper_lock
helpviewer_keywords:
- improper_lock class
ms.assetid: 8f494942-7748-4a2a-8de2-23414bfe6346
ms.openlocfilehash: de7393c9186a1572040acd18854b5b3046b239f2
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/31/2018
ms.locfileid: "50552794"
---
# <a name="improperlock-class"></a>improper_lock (Clase)

Esta clase describe una excepción que se produce cuando se realiza un bloqueo de forma incorrecta.

## <a name="syntax"></a>Sintaxis

```
class improper_lock : public std::exception;
```

## <a name="members"></a>Miembros

### <a name="public-constructors"></a>Constructores públicos

|Name|Descripción|
|----------|-----------------|
|[improper_lock)](#ctor)|Sobrecargado. Construye un objeto `improper_lock exception`.|

## <a name="remarks"></a>Comentarios

Normalmente, esta excepción se produce cuando se intenta adquirir un bloqueo no reentrante de forma recursiva en el mismo contexto.

## <a name="inheritance-hierarchy"></a>Jerarquía de herencia

`exception`

`improper_lock`

## <a name="requirements"></a>Requisitos

**Encabezado:** concrt.h

**Espacio de nombres:** simultaneidad

##  <a name="ctor"></a> improper_lock)

Construye un objeto `improper_lock exception`.

```
explicit _CRTIMP improper_lock(_In_z_ const char* _Message) throw();

improper_lock() throw();
```

### <a name="parameters"></a>Parámetros

*_Cuerpo*<br/>
Mensaje descriptivo del error.

## <a name="see-also"></a>Vea también

[concurrency (espacio de nombres)](concurrency-namespace.md)<br/>
[critical_section (clase)](critical-section-class.md)<br/>
[reader_writer_lock (clase)](reader-writer-lock-class.md)
