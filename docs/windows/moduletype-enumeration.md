---
title: "ModuleType (enumeración) | Documentos de Microsoft"
ms.custom: 
ms.date: 11/04/2016
ms.reviewer: 
ms.suite: 
ms.technology: cpp-windows
ms.tgt_pltfrm: 
ms.topic: reference
f1_keywords: module/Microsoft::WRL::ModuleType
dev_langs: C++
helpviewer_keywords: ModuleType enumeration
ms.assetid: 61a763af-a5a4-451d-8b40-815af507fcde
caps.latest.revision: "5"
author: mikeblome
ms.author: mblome
manager: ghogen
ms.workload:
- cplusplus
- uwp
ms.openlocfilehash: dd68d911a3734510bfb35db4b3ee0c4b8e46a4a0
ms.sourcegitcommit: 8fa8fdf0fbb4f57950f1e8f4f9b81b4d39ec7d7a
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/21/2017
---
# <a name="moduletype-enumeration"></a>ModuleType (enumeración)
Especifica si un módulo debe admitir un servidor en proceso o un servidor fuera de proceso.  
  
## <a name="syntax"></a>Sintaxis  
  
```  
enum ModuleType;  
```  
  
## <a name="members"></a>Miembros  
  
### <a name="values"></a>Valores  
  
|Nombre|Descripción|  
|----------|-----------------|  
|`InProc`|Un servidor en proceso.|  
|`OutOfProc`|Un servidor fuera de proceso.|  
|`DisableCaching`|Deshabilitar el mecanismo de almacenamiento en caché en el módulo.|  
|`InProcDisableCaching`|Combinación de `InProc` y `DisableCaching`.|  
|`OutOfProcDisableCaching`|Combinación de `OutOfProc` y `DisableCaching`.|  
  
## <a name="requirements"></a>Requisitos  
 **Encabezado:** module.h  
  
 **Espacio de nombres:** Microsoft::WRL  
  
## <a name="see-also"></a>Vea también  
 [Microsoft::WRL (espacio de nombres)](../windows/microsoft-wrl-namespace.md)