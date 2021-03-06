---
title: 'Contenedores de controles ActiveX: Insertar un control en una aplicación de contenedor de controles'
ms.date: 11/04/2016
helpviewer_keywords:
- ActiveX control containers [MFC], inserting controls
- ActiveX controls [MFC], adding to projects
ms.assetid: bbb617ff-872f-43d8-b4d6-c49adb16b148
ms.openlocfilehash: 2ca503119df955e8b76f6f8c131421f3e2d85652
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/31/2018
ms.locfileid: "50541380"
---
# <a name="activex-control-containers-inserting-a-control-into-a-control-container-application"></a>Contenedores de controles ActiveX: Insertar un control en una aplicación de contenedor de controles

Antes de que puede tener acceso a un control ActiveX desde una aplicación de contenedor de controles ActiveX, debe agregar el control ActiveX a la aplicación de contenedor mediante el [insertar ActiveX Control](../windows/insert-activex-control-dialog-box.md) cuadro de diálogo.

Para agregar un control ActiveX para el proyecto de contenedor de controles ActiveX, vea [ver y agregar controles ActiveX a un cuadro de diálogo](../windows/viewing-and-adding-activex-controls-to-a-dialog-box.md).

Una vez que agregue el control, deberá agregar una variable miembro (del tipo de control ActiveX) a la clase de cuadro de diálogo. Para obtener más información sobre este procedimiento, consulte [agregar una Variable miembro](../ide/adding-a-member-variable-visual-cpp.md).

Cuando haya agregado la variable miembro una clase, que se conoce como una clase contenedora, se genera automáticamente y se agrega al proyecto. Esta clase se utiliza como una interfaz entre el contenedor del control y el control incrustado.

## <a name="see-also"></a>Vea también

[Contenedores de controles ActiveX](../mfc/activex-control-containers.md)

