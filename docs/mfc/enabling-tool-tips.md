---
title: Habilitar la información sobre herramientas
ms.date: 11/04/2016
helpviewer_keywords:
- initializing tool tips [MFC]
- enabling tool tips [MFC]
- tool tips [MFC], initializing
- tool tips [MFC], enabling
ms.assetid: 06b7c889-7722-4ce6-8b88-9efa50fe6369
ms.openlocfilehash: 270eb8bad03679cd6e605e3279c0e4ffc499a765
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/31/2018
ms.locfileid: "50571160"
---
# <a name="enabling-tool-tips"></a>Habilitar la información sobre herramientas

Puede habilitar la compatibilidad con la sugerencia de herramienta para los controles secundarios de una ventana (por ejemplo, los controles de un cuadro de diálogo o la vista de formulario).

### <a name="to-enable-tool-tips-for-the-child-controls-of-a-window"></a>Para habilitar la información sobre herramientas para los controles secundarios de una ventana

1. Llame a `EnableToolTips` para la ventana para el que desea proporcionar información sobre herramientas.

1. Proporcionar una cadena para cada control en su [la notificación TTN_NEEDTEXT](../mfc/handling-ttn-needtext-notification-for-tool-tips.md) controlador. El controlador está en el mapa de mensajes de la ventana que contiene los controles secundarios (por ejemplo, la clase de vista de formulario). Este controlador debe llamar a una función que identifica el control y establece **pszText** para especificar el texto utilizado por el control de información sobre herramientas.

## <a name="see-also"></a>Vea también

[Información sobre herramientas en ventanas no derivadas de CFrameWnd](../mfc/tool-tips-in-windows-not-derived-from-cframewnd.md)

