---
title: Clases para Internet de Win32
ms.date: 09/12/2018
f1_keywords:
- vc.classes.win32
helpviewer_keywords:
- Internet classes [MFC]
- WinInet classes [MFC], classes
- Win32 [MFC], Internet classes
- Windows API [MFC], Internet classes
ms.assetid: b49601d5-3025-4068-9408-316b54ee4375
ms.openlocfilehash: a655759e8e1ffdcfe422305cd39623b9d7a6ca4e
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/31/2018
ms.locfileid: "50486442"
---
# <a name="win32-internet-classes"></a>Clases para Internet de Win32

MFC encapsula la tecnología de ActiveX y de Internet Win32 (WinInet) para facilitar la programación para Internet.

>[!IMPORTANT]
> ActiveX es una tecnología heredada que no se recomienda para nuevo desarrollo. Para obtener más información acerca de las tecnologías modernas que sustituyen a ActiveX, vea [controles ActiveX](activex-controls.md).

[CInternetSession](../mfc/reference/cinternetsession-class.md)<br/>
Crea e Inicializa una sesión de Internet o varias sesiones simultáneas y, si es necesario, describe la conexión a un servidor proxy.

[CInternetConnection](../mfc/reference/cinternetconnection-class.md)<br/>
Administra la conexión a un servidor de Internet.

[CInternetFile](../mfc/reference/cinternetfile-class.md)<br/>
Esta clase y sus clases derivadas permiten el acceso a archivos en sistemas remotos que utilizan protocolos de Internet.

[CHttpConnection](../mfc/reference/chttpconnection-class.md)<br/>
Administra la conexión a un servidor HTTP.

[CHttpFile](../mfc/reference/chttpfile-class.md)<br/>
Proporciona la funcionalidad para buscar y leer archivos en un servidor HTTP.

[CGopherFile](../mfc/reference/cgopherfile-class.md)<br/>
Proporciona la funcionalidad para buscar y leer archivos en un servidor gopher.

[CFtpConnection](../mfc/reference/cftpconnection-class.md)<br/>
Administra la conexión a un servidor FTP.

[CGopherConnection](../mfc/reference/cgopherconnection-class.md)<br/>
Administra la conexión a un servidor gopher.

[CFileFind](../mfc/reference/cfilefind-class.md)<br/>
Realiza el local y búsquedas de archivos de Internet.

[CFtpFileFind](../mfc/reference/cftpfilefind-class.md)<br/>
Ayuda en las búsquedas del archivo de Internet de servidores FTP.

[CGopherFileFind](../mfc/reference/cgopherfilefind-class.md)<br/>
Ayuda en las búsquedas de archivos de Internet de servidores gopher.

[CGopherLocator](../mfc/reference/cgopherlocator-class.md)<br/>
Obtiene un "localizador" gopher de un servidor gopher, determina el tipo de localizador y pone el localizador a disposición de `CGopherFileFind`.

[CInternetException](../mfc/reference/cinternetexception-class.md)<br/>
Representa una condición de excepción relacionada con una operación de Internet.

## <a name="see-also"></a>Vea también

[Información general de clases](../mfc/class-library-overview.md)

