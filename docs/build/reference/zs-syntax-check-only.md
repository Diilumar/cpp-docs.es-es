---
title: /Zs (Solamente comprobación de sintaxis)
ms.date: 11/04/2016
f1_keywords:
- /zs
helpviewer_keywords:
- -Zs compiler option [C++]
- Syntax Check Only compiler option
- Zs compiler option
- /Zs compiler option [C++]
ms.assetid: b4b41e6a-3f41-4d09-9cb6-fde5aa2cfecf
ms.openlocfilehash: 5cdd52ba6c221cbfa1526c19f3d6cfaf26a96e51
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/31/2018
ms.locfileid: "50429801"
---
# <a name="zs-syntax-check-only"></a>/Zs (Solamente comprobación de sintaxis)

Indica al compilador para comprobar solo la sintaxis de los archivos de origen en la línea de comandos.

## <a name="syntax"></a>Sintaxis

```
/Zs
```

## <a name="remarks"></a>Comentarios

Cuando se usa esta opción, se crea ningún archivo de salida y mensajes de error se escriben en la salida estándar.

El **/Zs** opción proporciona una forma rápida de encontrar y corregir errores de sintaxis antes de compilar y vincular un archivo de origen.

### <a name="to-set-this-compiler-option-in-the-visual-studio-development-environment"></a>Para establecer esta opción del compilador en el entorno de desarrollo de Visual Studio

1. Abra el cuadro de diálogo **Páginas de propiedades** del proyecto. Para obtener más información, vea [Trabajar con propiedades del proyecto](../../ide/working-with-project-properties.md).

1. Haga clic en la carpeta **C/C++** .

1. Haga clic en la página de propiedades **Línea de comandos** .

1. Escriba la opción del compilador en el cuadro **Opciones adicionales** .

### <a name="to-set-this-compiler-option-programmatically"></a>Para establecer esta opción del compilador mediante programación

- Vea <xref:Microsoft.VisualStudio.VCProjectEngine.VCCLCompilerTool.AdditionalOptions%2A>.

## <a name="see-also"></a>Vea también

[Opciones del compilador](../../build/reference/compiler-options.md)<br/>
[Establecer las opciones del compilador](../../build/reference/setting-compiler-options.md)