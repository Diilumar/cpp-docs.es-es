---
title: Interfaces del objeto de comando
ms.date: 10/24/2018
helpviewer_keywords:
- command object interfaces [C++]
- command objects [OLE DB]
- OLE DB [C++], command object interfaces
ms.assetid: dacff5ae-252c-4f20-9ad7-4e602cc48536
ms.openlocfilehash: d9f663d4e857d300e5c0f5783b86445ce824ea8e
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/31/2018
ms.locfileid: "50598879"
---
# <a name="command-object-interfaces"></a>Interfaces del objeto de comando

El objeto de comando utiliza el `IAccessor` interfaz para especificar enlaces de parámetros. El consumidor llama a `IAccessor::CreateAccessor`, pasa una matriz de `DBBINDING` estructuras. `DBBINDING` contiene información acerca de los enlaces de columna (por ejemplo, tipo y longitud). El proveedor recibe las estructuras y determina cómo se deben transferir los datos y si las conversiones son necesarias.

El `ICommandText` interfaz proporciona una manera de especificar un comando de texto. El `ICommandProperties` interfaz controla todas las propiedades de comando.

## <a name="see-also"></a>Vea también

[Arquitectura de plantillas de proveedores OLE DB](../../data/oledb/ole-db-provider-template-architecture.md)<br/>
