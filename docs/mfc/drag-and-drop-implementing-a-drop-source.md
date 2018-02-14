---
title: "Arrastrar y colocar: implementar un origen de colocación | Documentos de Microsoft"
ms.custom: 
ms.date: 11/04/2016
ms.reviewer: 
ms.suite: 
ms.technology: cpp-windows
ms.tgt_pltfrm: 
ms.topic: article
dev_langs: C++
helpviewer_keywords:
- OLE drag and drop [MFC], initiating drag operations
- drag and drop [MFC], calling DoDragDrop
- OLE drag and drop [MFC], drop source
- OLE drag and drop [MFC], calling DoDragDrop
- drag and drop [MFC], initiating drag operations
- drag and drop [MFC], drop source
ms.assetid: 0ed2fda0-63fa-4b1e-b398-f1f142f40035
caps.latest.revision: "10"
author: mikeblome
ms.author: mblome
manager: ghogen
ms.workload: cplusplus
ms.openlocfilehash: 301980f7f5a901aa4e2cba40357b18311eef581e
ms.sourcegitcommit: 8fa8fdf0fbb4f57950f1e8f4f9b81b4d39ec7d7a
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/21/2017
---
# <a name="drag-and-drop-implementing-a-drop-source"></a>Arrastrar y colocar: Implementar un origen de colocación
En este artículo se explica cómo obtener la aplicación para proporcionar datos a una operación de arrastrar y colocar.  
  
 Implementación básica de un origen de colocación es relativamente sencilla. El primer paso es determinar qué eventos inician una operación de arrastre. Recomienda directrices de interfaz de usuario definen el principio de una operación de arrastre como la selección de datos y un `WM_LBUTTONDOWN` eventos que se producen en un punto dentro de los datos seleccionados. Los ejemplos de MFC OLE [OCLIENT](../visual-cpp-samples.md) y [HIERSVR](../visual-cpp-samples.md) siga estas instrucciones.  
  
 Si la aplicación es un contenedor y los datos seleccionados están vinculado o un objeto incrustado de tipo `COleClientItem`, llame a su `DoDragDrop` función miembro. En caso contrario, construir un `COleDataSource` objeto, inicialícelo con la selección y llamar al objeto de origen de datos `DoDragDrop` función miembro. Si la aplicación es un servidor, use `COleServerItem::DoDragDrop`. Para obtener información acerca de cómo personalizar el comportamiento estándar de arrastrar y colocar, vea el artículo [arrastrar y colocar: personalización](../mfc/drag-and-drop-customizing.md).  
  
 Si `DoDragDrop` devuelve `DROPEFFECT_MOVE`, eliminar inmediatamente los datos de origen del documento de origen. Ningún otro tipo de valor devuelto de `DoDragDrop` no tiene ningún efecto en un origen de colocación.  
  
 Para obtener más información, consulte:  
  
-   [Implementar un destino de colocación](../mfc/drag-and-drop-implementing-a-drop-target.md)  
  
-   [Personalización de arrastrar y colocar](../mfc/drag-and-drop-customizing.md)  
  
-   [Crear y destruir objetos de datos OLE y orígenes de datos](../mfc/data-objects-and-data-sources-creation-and-destruction.md)  
  
-   [Manipular objetos de datos OLE y orígenes de datos](../mfc/data-objects-and-data-sources-manipulation.md)  
  
## <a name="see-also"></a>Vea también  
 [Arrastrar y colocar (OLE)](../mfc/drag-and-drop-ole.md)   
 [COleDataSource:: DoDragDrop](../mfc/reference/coledatasource-class.md#dodragdrop)   
 [COleClientItem::DoDragDrop](../mfc/reference/coleclientitem-class.md#dodragdrop)   
 [CView::OnDragLeave](../mfc/reference/cview-class.md#ondragleave)
