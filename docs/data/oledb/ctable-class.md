---
title: CTable (Clase)
ms.date: 11/04/2016
f1_keywords:
- ATL::CTable
- ATL.CTable
- CTable
- ATL.CTable.Open
- ATL::CTable::Open
- CTable::Open
- CTable.Open
helpviewer_keywords:
- CTable class
- Open method
ms.assetid: f13fdaa3-e198-4557-977d-54b0bbc3454d
ms.openlocfilehash: 7605d78a140a0f5353a16b9e22d5d618d29ff327
ms.sourcegitcommit: c40469825b6101baac87d43e5f4aed6df6b078f5
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/12/2018
ms.locfileid: "51556691"
---
# <a name="ctable-class"></a>CTable (Clase)

Proporciona un medio para tener acceso directamente a un conjunto de filas sencillo (uno sin parámetros).

## <a name="syntax"></a>Sintaxis

```cpp
template <class TAccessor = CNoAccessor,
            template <typename T> class TRowset = CRowset>
class CTable :
   public CAccessorRowset <TAccessor, TRowset>
```

### <a name="parameters"></a>Parámetros

*TAccessor*<br/>
Una clase de descriptor de acceso.

*TRowset*<br/>
Una clase de conjunto de filas.

## <a name="requirements"></a>Requisitos

**Encabezado:** atldbcli.h

## <a name="members"></a>Miembros

### <a name="methods"></a>Métodos

|||
|-|-|
|[Abrir](#open)|Se abre en la tabla.|

## <a name="remarks"></a>Comentarios

Consulte [CCommand](../../data/oledb/ccommand-class.md) para obtener información sobre cómo ejecutar un comando para obtener acceso a un conjunto de filas.

## <a name="open"></a> CTable:: Open

Se abre en la tabla.

### <a name="syntax"></a>Sintaxis

```cpp
HRESULT Open(const CSession& session,
   LPCWSTR wszTableName,
   DBPROPSET* pPropSet = NULL,
   ULONG ulPropSets = 0) throw ();

HRESULT Open(const CSession& session,
   LPCSTR szTableName,
   DBPROPSET* pPropSet = NULL,
   ULONG ulPropSets = 0) throw ();

HRESULT Open(const CSession& session,
   DBID& dbid,
   DBPROPSET* pPropSet = NULL,
   ULONG ulPropSets = 0) throw ();
```

#### <a name="parameters"></a>Parámetros

*Sesión*<br/>
[in] La sesión para el que se abre en la tabla.

*wszTableName*<br/>
[in] El nombre de la tabla para poder abrirlos, se pasa como una cadena Unicode.

*szTableName*<br/>
[in] El nombre de la tabla para poder abrirlos, se pasa como una cadena ANSI.

*dbid*<br/>
[in] El `DBID` de la tabla que desea abrir.

*pPropSet*<br/>
[in] Un puntero a una matriz de [DBPROPSET](https://docs.microsoft.com/previous-versions/windows/desktop/ms714367(v=vs.85)) estructuras que contienen las propiedades y valores que desea establecer. Consulte [conjuntos de propiedades y grupos de propiedades](https://docs.microsoft.com/previous-versions/windows/desktop/ms713696(v=vs.85)) en el *referencia del programador OLE DB* en el SDK de Windows. El valor predeterminado es null, especifica ninguna propiedad.

*ulPropSets*<br/>
[in] El número de [DBPROPSET](https://docs.microsoft.com/previous-versions/windows/desktop/ms714367(v=vs.85)) pasan las estructuras en el *pPropSet* argumento.

### <a name="return-value"></a>Valor devuelto

Un HRESULT estándar.

### <a name="remarks"></a>Comentarios

Para obtener más información, consulte [IOpenRowset:: OpenRowset](https://docs.microsoft.com/previous-versions/windows/desktop/ms716724(v=vs.85)) en el *referencia del programador de OLE DB*.

## <a name="see-also"></a>Vea también

[Plantillas de consumidor OLE DB](../../data/oledb/ole-db-consumer-templates-cpp.md)<br/>
[Referencia de plantillas de consumidor OLE DB](../../data/oledb/ole-db-consumer-templates-reference.md)