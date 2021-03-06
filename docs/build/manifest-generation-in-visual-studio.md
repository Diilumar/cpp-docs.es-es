---
title: Generación de manifiestos en Visual Studio
ms.date: 11/04/2016
helpviewer_keywords:
- manifests [C++]
ms.assetid: 0af60aa9-d223-42cd-8426-b3fc543a2a81
ms.openlocfilehash: 75f8fcae2a51e4e8296f6f3c252888b6ca55ad20
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/31/2018
ms.locfileid: "50520359"
---
# <a name="manifest-generation-in-visual-studio"></a>Generación de manifiestos en Visual Studio

Se puede controlar la generación de un archivo de manifiesto para un proyecto concreto en el proyecto **páginas de propiedades** cuadro de diálogo. En el **propiedades de configuración** , haga clic **vinculador**, a continuación, **archivo de manifiesto de**, a continuación, **Generar manifiesto**. De forma predeterminada se establecen las propiedades del proyecto de nuevos proyectos para generar un archivo de manifiesto. Sin embargo es posible deshabilitar la generación del manifiesto para un proyecto mediante el **Generar manifiesto** propiedad del proyecto. Cuando esta propiedad se establece en **Sí**, se genera el manifiesto para este proyecto. En caso contrario, el vinculador omite la información de ensamblado al resolver dependencias del código de aplicación y no genera el manifiesto.

El sistema de compilación en Visual Studio permite que el manifiesto se incrusta en el archivo de aplicación binario final, o generado como un archivo externo. Este comportamiento se controla mediante el **incrustar manifiesto** opción el **las propiedades del proyecto** cuadro de diálogo. Para establecer esta propiedad, abra el **herramienta manifiesto** nodo, a continuación, seleccione **de entrada y salida**. Si no se incrusta el manifiesto, se genera como un archivo externo y guardado en el mismo directorio que el archivo binario final. Si el manifiesto está incrustado, Visual Studio incrusta los manifiestos finales mediante el proceso siguiente:

1. Una vez compilado el código fuente en los archivos objeto, el vinculador recopila información de ensamblado dependiente. Al vincular el archivo binario final, el vinculador genera un manifiesto intermedio que se utilizará posteriormente para generar el manifiesto final.

1. Una vez terminado el manifiesto intermedio y la vinculación, se ejecutará la herramienta de manifiesto para combinar un manifiesto final y guardarla como un archivo externo.

1. El proyecto de sistema de compilación, a continuación, detecta si el manifiesto generado por la herramienta de manifiesto contiene información diferente que el manifiesto incrustado ya en el archivo binario.

1. Si el manifiesto incrustado en el archivo binario es diferente del manifiesto generado por la herramienta manifiesto, o el archivo binario no contiene un manifiesto incrustado, Visual Studio llamará al vinculador una vez más para incrustar el archivo de manifiesto externo dentro del archivo binario como un recurso.

1. Si el manifiesto incrustado en el archivo binario es el mismo que el manifiesto generado por la herramienta manifiesto, la compilación seguirá los pasos de compilación.

El manifiesto está incrustado en el archivo binario final como un recurso de texto y se puede ver abriendo el archivo binario final como un archivo en Visual Studio. Para asegurarse de que el manifiesto señala a las bibliotecas correctas, siga los pasos descritos en [descripción de las dependencias de una aplicación de Visual C++](../ide/understanding-the-dependencies-of-a-visual-cpp-application.md) o siga las sugerencias que se describe en el [desolucióndeproblemas](../build/troubleshooting-c-cpp-isolated-applications-and-side-by-side-assemblies.md) sección.

## <a name="see-also"></a>Vea también

[Cómo: Incrustar un manifiesto en una aplicación de C/C++](../build/how-to-embed-a-manifest-inside-a-c-cpp-application.md)<br/>
[Acerca de los ensamblados privados](/windows/desktop/SbsCs/about-private-assemblies-)<br/>
[Herramienta manifiesto](/windows/desktop/SbsCs/mt-exe)<br/>
[Introducción a la generación de manifiestos para los programas de C/C++](../build/understanding-manifest-generation-for-c-cpp-programs.md)