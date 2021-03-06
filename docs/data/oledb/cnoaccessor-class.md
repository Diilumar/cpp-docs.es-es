---
title: CNoAccessor (Clase)
ms.date: 11/04/2016
f1_keywords:
- ATL::CNoAccessor
- CNoAccessor
- ATL.CNoAccessor
helpviewer_keywords:
- CNoAccessor class
ms.assetid: eb669ae5-0a56-49a3-9646-c4ae6239da31
ms.openlocfilehash: d6eb5aaa9a66f46335b0a364e6c6e79abc297d64
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/31/2018
ms.locfileid: "50647903"
---
# <a name="cnoaccessor-class"></a>CNoAccessor (Clase)

Se puede usar como un argumento de plantilla (`TAccessor`) para las clases de plantilla, como `CCommand` y `CTable`, que requieren un argumento de la clase de descriptor de acceso.

## <a name="syntax"></a>Sintaxis

```cpp
class CNoAccessor
```

## <a name="remarks"></a>Comentarios

Use `CNoAccessor` como argumento de plantilla cuando no desea que la clase para admitir parámetros o columnas de salida.

`CNoAccessor` implementa los siguientes métodos de código auxiliar, cada uno de los cuales corresponde a otros métodos de clase de descriptor de acceso:

- `BindColumns` -Enlaza las columnas a los descriptores de acceso.

- `BindParameters` -Enlaza los parámetros creados para las columnas.

- `Bind` : Crea los enlaces.

- `Close` -Cierra el descriptor de acceso.

- `ReleaseAccessors` -Libera los descriptores de acceso creados por la clase.

- `FreeRecordMemory` -Libera las columnas en el registro actual que necesitan ser liberados.

- `GetColumnInfo` -Obtiene información de columna del conjunto de filas abierto.

- `GetNumAccessors` -Recupera el número de descriptores de acceso creado por la clase.

- `IsAutoAccessor` -Devuelve true si se recuperan automáticamente los datos para el descriptor de acceso durante una operación de movimiento.

- `GetHAccessor` -Recupera el identificador de descriptor de acceso de un descriptor de acceso especificada.

- `GetBuffer` -Recupera el puntero al búfer del marcador.

- `NoBindOnNullRowset` -Impide que el enlace de datos en conjuntos de filas vacío.

## <a name="requirements"></a>Requisitos

**Encabezado:** atldbcli.h

## <a name="see-also"></a>Vea también

[Plantillas de consumidor OLE DB](../../data/oledb/ole-db-consumer-templates-cpp.md)<br/>
[Referencia de plantillas de consumidor OLE DB](../../data/oledb/ole-db-consumer-templates-reference.md)