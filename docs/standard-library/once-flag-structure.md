---
title: once_flag (Estructura) | Microsoft Docs
ms.custom: 
ms.date: 11/04/2016
ms.reviewer: 
ms.suite: 
ms.technology: cpp-standard-libraries
ms.tgt_pltfrm: 
ms.topic: article
f1_keywords: mutex/std::once_flag
dev_langs: C++
ms.assetid: 71bfb88d-ca8c-4082-a6e1-ff52151e8629
caps.latest.revision: "13"
author: corob-msft
ms.author: corob
manager: ghogen
ms.workload: cplusplus
ms.openlocfilehash: fc66f322490bc728ab6d25e185f6b8d4ce0f0179
ms.sourcegitcommit: 8fa8fdf0fbb4f57950f1e8f4f9b81b4d39ec7d7a
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/21/2017
---
# <a name="onceflag-structure"></a>once_flag (Estructura)
Representa un `struct` que se usa con la función de plantilla [call_once](../standard-library/mutex-functions.md#call_once) para asegurarse de que solo se llame una vez al código de inicialización, incluso ante la presencia de varios subprocesos de ejecución.  
  
## <a name="syntax"></a>Sintaxis  
  
struct once_flag { constexpr once_flag() noexcept; once_flag(const once_flag&); once_flag& operator=(const once_flag&); };  
  
## <a name="remarks"></a>Comentarios  
 El `once_flag` `struct` tiene solo un constructor predeterminado.  
  
 Los objetos de tipo `once_flag` pueden crearse, pero no pueden copiarse.  
  
## <a name="requirements"></a>Requisitos  
 **Encabezado:** \<mutex >  
  
 **Espacio de nombres:** std  
  
## <a name="see-also"></a>Vea también  
 [Referencia de archivos de encabezado](../standard-library/cpp-standard-library-header-files.md)   
 [\<mutex>](../standard-library/mutex.md)


