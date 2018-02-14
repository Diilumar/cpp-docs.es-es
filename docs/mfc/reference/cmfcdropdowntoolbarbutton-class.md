---
title: Clase CMFCDropDownToolbarButton | Documentos de Microsoft
ms.custom: 
ms.date: 11/04/2016
ms.reviewer: 
ms.suite: 
ms.technology: cpp-windows
ms.tgt_pltfrm: 
ms.topic: reference
f1_keywords:
- CMFCDropDownToolbarButton
- AFXDROPDOWNTOOLBAR/CMFCDropDownToolbarButton
- AFXDROPDOWNTOOLBAR/CMFCDropDownToolbarButton::CMFCDropDownToolbarButton
- AFXDROPDOWNTOOLBAR/CMFCDropDownToolbarButton::CopyFrom
- AFXDROPDOWNTOOLBAR/CMFCDropDownToolbarButton::DropDownToolbar
- AFXDROPDOWNTOOLBAR/CMFCDropDownToolbarButton::ExportToMenuButton
- AFXDROPDOWNTOOLBAR/CMFCDropDownToolbarButton::GetDropDownToolBar
- AFXDROPDOWNTOOLBAR/CMFCDropDownToolbarButton::IsDropDown
- AFXDROPDOWNTOOLBAR/CMFCDropDownToolbarButton::IsExtraSize
- AFXDROPDOWNTOOLBAR/CMFCDropDownToolbarButton::OnCalculateSize
- AFXDROPDOWNTOOLBAR/CMFCDropDownToolbarButton::OnChangeParentWnd
- AFXDROPDOWNTOOLBAR/CMFCDropDownToolbarButton::OnClick
- AFXDROPDOWNTOOLBAR/CMFCDropDownToolbarButton::OnClickUp
- AFXDROPDOWNTOOLBAR/CMFCDropDownToolbarButton::OnContextHelp
- AFXDROPDOWNTOOLBAR/CMFCDropDownToolbarButton::OnCustomizeMenu
- AFXDROPDOWNTOOLBAR/CMFCDropDownToolbarButton::OnDraw
- AFXDROPDOWNTOOLBAR/CMFCDropDownToolbarButton::OnDrawOnCustomizeList
- AFXDROPDOWNTOOLBAR/CMFCDropDownToolbarButton::Serialize
- AFXDROPDOWNTOOLBAR/CMFCDropDownToolbarButton::SetDefaultCommand
- AFXDROPDOWNTOOLBAR/CMFCDropDownToolbarButton::m_uiShowBarDelay
dev_langs: C++
helpviewer_keywords:
- CMFCDropDownToolbarButton [MFC], CMFCDropDownToolbarButton
- CMFCDropDownToolbarButton [MFC], CopyFrom
- CMFCDropDownToolbarButton [MFC], DropDownToolbar
- CMFCDropDownToolbarButton [MFC], ExportToMenuButton
- CMFCDropDownToolbarButton [MFC], GetDropDownToolBar
- CMFCDropDownToolbarButton [MFC], IsDropDown
- CMFCDropDownToolbarButton [MFC], IsExtraSize
- CMFCDropDownToolbarButton [MFC], OnCalculateSize
- CMFCDropDownToolbarButton [MFC], OnChangeParentWnd
- CMFCDropDownToolbarButton [MFC], OnClick
- CMFCDropDownToolbarButton [MFC], OnClickUp
- CMFCDropDownToolbarButton [MFC], OnContextHelp
- CMFCDropDownToolbarButton [MFC], OnCustomizeMenu
- CMFCDropDownToolbarButton [MFC], OnDraw
- CMFCDropDownToolbarButton [MFC], OnDrawOnCustomizeList
- CMFCDropDownToolbarButton [MFC], Serialize
- CMFCDropDownToolbarButton [MFC], SetDefaultCommand
- CMFCDropDownToolbarButton [MFC], m_uiShowBarDelay
ms.assetid: bc9d69e6-bd3e-4c15-9368-e80a504a0ba7
caps.latest.revision: "31"
author: mikeblome
ms.author: mblome
manager: ghogen
ms.workload: cplusplus
ms.openlocfilehash: 2f9481583c56676d206225ad76f8131c2a79821f
ms.sourcegitcommit: 8fa8fdf0fbb4f57950f1e8f4f9b81b4d39ec7d7a
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/21/2017
---
# <a name="cmfcdropdowntoolbarbutton-class"></a>Clase CMFCDropDownToolbarButton
Un tipo de botón de la barra de herramientas que se comporta como un botón normal cuando se hace clic en él. Sin embargo, abre una barra de herramientas desplegable ( [CMFCDropDownToolBar clase](../../mfc/reference/cmfcdropdowntoolbar-class.md) si el usuario presiona y mantiene presionado el botón de la barra de herramientas.  
  
## <a name="syntax"></a>Sintaxis  
  
```  
class CMFCDropDownToolbarButton : public CMFCToolBarButton  
```  
  
## <a name="members"></a>Miembros  
  
### <a name="public-constructors"></a>Constructores públicos  
  
|Name|Descripción|  
|----------|-----------------|  
|[CMFCDropDownToolbarButton::CMFCDropDownToolbarButton](#cmfcdropdowntoolbarbutton)|Construye un objeto `CMFCDropDownToolbarButton`.|  
|`CMFCDropDownToolbarButton::~CMFCDropDownToolbarButton`|Destructor.|  
  
### <a name="public-methods"></a>Métodos públicos  
  
|Name|Descripción|  
|----------|-----------------|  
|[CMFCDropDownToolbarButton::CopyFrom](#copyfrom)|Copia las propiedades de otro botón de barra de herramientas a la actual. (Invalida [CMFCToolBarButton::CopyFrom](../../mfc/reference/cmfctoolbarbutton-class.md#copyfrom).)|  
|`CMFCDropDownToolbarButton::CreateObject`|Usado por el marco para crear una instancia dinámica de este tipo de clase.|  
|[CMFCDropDownToolbarButton::DropDownToolbar](#dropdowntoolbar)|Se abre una barra de herramientas de la lista desplegable.|  
|[CMFCDropDownToolbarButton::ExportToMenuButton](#exporttomenubutton)|Copia el texto en el botón de barra de herramientas a un menú. (Invalida [CMFCToolBarButton::ExportToMenuButton](../../mfc/reference/cmfctoolbarbutton-class.md#exporttomenubutton).)|  
|[CMFCDropDownToolbarButton::GetDropDownToolBar](#getdropdowntoolbar)|Recupera la barra de herramientas de la lista desplegable que está asociado con el botón.|  
|`CMFCDropDownToolbarButton::GetThisClass`|Usado por el marco de trabajo para obtener un puntero a la [CRuntimeClass](../../mfc/reference/cruntimeclass-structure.md) objeto que está asociado a este tipo de clase.|  
|[CMFCDropDownToolbarButton::IsDropDown](#isdropdown)|Determina si la barra de herramientas de la lista desplegable está abierto actualmente.|  
|[CMFCDropDownToolbarButton::IsExtraSize](#isextrasize)|Determina si se puede mostrar el botón con un borde extendido. (Invalida [CMFCToolBarButton::IsExtraSize](../../mfc/reference/cmfctoolbarbutton-class.md#isextrasize).)|  
|[CMFCDropDownToolbarButton::OnCalculateSize](#oncalculatesize)|Lo llama el marco de trabajo para calcular el tamaño del botón para el contexto de dispositivo especificado y el estado de acoplamiento. (Invalida [CMFCToolBarButton::OnCalculateSize](../../mfc/reference/cmfctoolbarbutton-class.md#oncalculatesize).)|  
|`CMFCDropDownToolbarButton::OnCancelMode`|Lo llama el marco para controlar la [WM_CANCELMODE](http://msdn.microsoft.com/library/windows/desktop/ms632615) mensaje. (Invalida `CMCToolBarButton::OnCancelMode`).|  
|[CMFCDropDownToolbarButton::OnChangeParentWnd](#onchangeparentwnd)|Lo llama el marco cuando el botón se inserta en una nueva barra de herramientas. (Invalida [CMFCToolBarButton::OnChangeParentWnd](../../mfc/reference/cmfctoolbarbutton-class.md#onchangeparentwnd).)|  
|[CMFCDropDownToolbarButton::OnClick](#onclick)|Lo llama el marco cuando el usuario hace clic en el botón del mouse. (Invalida [CMFCToolBarButton::OnClick](../../mfc/reference/cmfctoolbarbutton-class.md#onclick).)|  
|[CMFCDropDownToolbarButton::OnClickUp](#onclickup)|Lo llama el marco cuando el usuario suelta el botón del mouse. (Invalida [CMFCToolBarButton::OnClickUp](../../mfc/reference/cmfctoolbarbutton-class.md#onclickup).)|  
|[CMFCDropDownToolbarButton::OnContextHelp](#oncontexthelp)|Lo llama el marco cuando la barra de herramientas primario controla un `WM_HELPHITTEST` mensaje. (Invalida [CMFCToolBarButton::OnContextHelp](../../mfc/reference/cmfctoolbarbutton-class.md#oncontexthelp).)|  
|[CMFCDropDownToolbarButton::OnCustomizeMenu](#oncustomizemenu)|Modifica el menú proporcionado cuando la aplicación muestra un menú contextual en la barra de herramientas primario. (Invalida [CMFCToolBarButton::OnCustomizeMenu](../../mfc/reference/cmfctoolbarbutton-class.md#oncustomizemenu).)|  
|[CMFCDropDownToolbarButton::OnDraw](#ondraw)|Lo llama el marco de trabajo para dibujar el botón con los estilos especificados y las opciones. (Invalida [CMFCToolBarButton::OnDraw](../../mfc/reference/cmfctoolbarbutton-class.md#ondraw).)|  
|[CMFCDropDownToolbarButton::OnDrawOnCustomizeList](#ondrawoncustomizelist)|Lo llama el marco para dibujar el botón el **comandos** panel de la **personalizar** cuadro de diálogo. (Invalida [CMFCToolBarButton::OnDrawOnCustomizeList](../../mfc/reference/cmfctoolbarbutton-class.md#ondrawoncustomizelist).)|  
|[CMFCDropDownToolbarButton::Serialize](#serialize)|Lee este objeto desde un archivo o lo escribe en un archivo. (Invalida [CMFCToolBarButton::Serialize](../../mfc/reference/cmfctoolbarbutton-class.md#serialize).)|  
|[CMFCDropDownToolbarButton::SetDefaultCommand](#setdefaultcommand)|Establece el comando predeterminado que el marco de trabajo que se usa cuando un usuario hace clic en el botón.|  
  
### <a name="data-members"></a>Miembros de datos  
  
|nombre|Descripción|  
|----------|-----------------|  
|[CMFCDropDownToolbarButton::m_uiShowBarDelay](#m_uishowbardelay)|Especifica el período de tiempo que un usuario debe contener el botón del mouse hacia abajo antes de que aparezca la barra de herramientas de la lista desplegable.|  
  
## <a name="remarks"></a>Comentarios  
 Un `CMFCDropDownToolBarButton` difiere de un botón normal porque tiene una pequeña flecha en la esquina inferior derecha del botón. Cuando el usuario selecciona un botón de la barra de herramientas de la lista desplegable, el marco de trabajo muestra su icono en el botón de barra de herramientas de nivel superior (el botón con la flecha pequeña situada en la esquina inferior derecha).  
  
 Para obtener información sobre cómo implementar una barra de herramientas de la lista desplegable, consulte [CMFCDropDownToolBar clase](../../mfc/reference/cmfcdropdowntoolbar-class.md).  
  
 El `CMFCDropDownToolBarButton` objeto puede exportarse a un [CMFCToolBarMenuButton clase](../../mfc/reference/cmfctoolbarmenubutton-class.md) objeto y se muestra como un botón de menú con un menú emergente.  
  
## <a name="inheritance-hierarchy"></a>Jerarquía de herencia  
 [CObject](../../mfc/reference/cobject-class.md)  
  
 [CMFCToolBarButton](../../mfc/reference/cmfctoolbarbutton-class.md)  
  
 [CMFCDropDownToolbarButton](../../mfc/reference/cmfcdropdowntoolbarbutton-class.md)  
  
## <a name="requirements"></a>Requisitos  
 **Encabezado:** afxdropdowntoolbar.h  
  
##  <a name="copyfrom"></a>CMFCDropDownToolbarButton::CopyFrom  
 Copia las propiedades de otro botón de barra de herramientas a la actual.  
  
```  
virtual void CopyFrom(const CMFCToolBarButton& src);
```  
  
### <a name="parameters"></a>Parámetros  
 [in] `src`  
 Una referencia al botón de origen desde el que se va a copiar.  
  
### <a name="remarks"></a>Comentarios  
 Llamar a este método para copiar otro botón de barra de herramientas en este botón de barra de herramientas. `src`debe ser del tipo `CMFCDropDownToolbarButton`.  
  
##  <a name="cmfcdropdowntoolbarbutton"></a>CMFCDropDownToolbarButton::CMFCDropDownToolbarButton  
 Construye un objeto `CMFCDropDownToolbarButton`.  
  
```  
CMFCDropDownToolbarButton();

 
CMFCDropDownToolbarButton(
    LPCTSTR lpszName,  
    CMFCDropDownToolBar* pToolBar);
```  
  
### <a name="parameters"></a>Parámetros  
 [in] `lpszName`  
 El texto predeterminado del botón.  
  
 [in] `pToolBar`  
 Un puntero a la `CMFCDropDownToolBar` objeto que se muestra cuando el usuario presiona el botón.  
  
### <a name="remarks"></a>Comentarios  
 La segunda sobrecarga del constructor de copia en el botón de lista desplegable el primer botón de la barra de herramientas que `pToolBar` especifica.  
  
 Normalmente, un botón de barra de herramientas desplegable utiliza el texto en el botón usado más recientemente en la barra de herramientas que `pToolBar` especifica. Utiliza el texto especificado por `lpszName` cuando el botón se convierte en un botón de menú o se muestra en el **comandos** pestaña de la **personalizar** cuadro de diálogo. Para obtener más información sobre la **personalizar** cuadro de diálogo, vea [CMFCToolBarsCustomizeDialog clase](../../mfc/reference/cmfctoolbarscustomizedialog-class.md).  
  
### <a name="example"></a>Ejemplo  
 En el ejemplo siguiente se muestra cómo construir un objeto de la `CMFCDropDownToolbarButton` clase. Este fragmento de código forma parte de la [ejemplo de demostración de Visual Studio](../../visual-cpp-samples.md).  
  
 [!code-cpp[NVC_MFC_VisualStudioDemo#31](../../mfc/codesnippet/cpp/cmfcdropdowntoolbarbutton-class_1.cpp)]  
  
##  <a name="dropdowntoolbar"></a>CMFCDropDownToolbarButton::DropDownToolbar  
 Se abre una barra de herramientas de la lista desplegable.  
  
```  
BOOL DropDownToolbar(CWnd* pWnd);
```  
  
### <a name="parameters"></a>Parámetros  
 [in] `pWnd`  
 La ventana primaria del marco de lista desplegable, o `NULL` para utilizar la ventana principal del botón de barra de herramientas de lista desplegable.  
  
### <a name="return-value"></a>Valor devuelto  
 Es distinto de cero si el método es correcto; en caso contrario es 0.  
  
### <a name="remarks"></a>Comentarios  
 El [CMFCDropDownToolbarButton::OnClick](#onclick) método llama a este método para abrir la barra de herramientas de la lista desplegable cuando el usuario presiona y mantiene presionado el botón de la barra de herramientas.  
  
 Este método crea la barra de herramientas de la lista desplegable mediante el [CMFCDropDownFrame::Create](../../mfc/reference/cmfcdropdownframe-class.md#create) método. Si la barra de herramientas primario se acopla verticalmente, este método coloca la barra de herramientas de la lista desplegable en el lado izquierdo o derecho de la barra de herramientas principal, según el ajuste. En caso contrario, este método coloca la barra de herramientas de la lista desplegable debajo de la barra de herramientas primario.  
  
 Este método produce un error si `pWnd` es `NULL` y el botón de barra de herramientas de lista desplegable no tiene una ventana primaria.  
  
##  <a name="exporttomenubutton"></a>CMFCDropDownToolbarButton::ExportToMenuButton  
 Copia el texto en el botón de barra de herramientas a un menú.  
  
```  
virtual BOOL ExportToMenuButton(CMFCToolBarMenuButton& menuButton) const;  
```  
  
### <a name="parameters"></a>Parámetros  
 [in] `menuButton`  
 Una referencia al botón de menú de destino.  
  
### <a name="return-value"></a>Valor devuelto  
 Distinto de cero si el método es correcto; de lo contrario, 0.  
  
### <a name="remarks"></a>Comentarios  
 Este método llama a la implementación de la clase base ( [CMFCToolBarButton::ExportToMenuButton](../../mfc/reference/cmfctoolbarbutton-class.md#exporttomenubutton)) y, a continuación, se anexa al botón de menú de destino que un menú emergente que contiene cada elemento de menú de barra de herramientas en este botón. Este método no anexa submenús al menú emergente.  
  
 Este método produce un error si la barra de herramientas principal, `m_pToolBar`, es `NULL` o la implementación de la clase base devuelve `FALSE`.  
  
##  <a name="getdropdowntoolbar"></a>CMFCDropDownToolbarButton::GetDropDownToolBar  
 Recupera la barra de herramientas de la lista desplegable que está asociado con el botón.  
  
```  
CMFCToolBar* GetDropDownToolBar() const;  
```  
  
### <a name="return-value"></a>Valor devuelto  
 La barra de herramientas de lista desplegable que está asociado con el botón.  
  
### <a name="remarks"></a>Comentarios  
 Este método devuelve el `m_pToolBar` miembro de datos.  
  
##  <a name="isdropdown"></a>CMFCDropDownToolbarButton::IsDropDown  
 Determina si la barra de herramientas de la lista desplegable está abierto actualmente.  
  
```  
BOOL IsDropDown() const;  
```  
  
### <a name="return-value"></a>Valor devuelto  
 Es distinto de cero si la barra de herramientas de la lista desplegable está abierta; en caso contrario es 0.  
  
### <a name="remarks"></a>Comentarios  
 El marco de trabajo abre la barra de herramientas de la lista desplegable con los [CMFCDropDownToolbarButton::DropDownToolbar](#dropdowntoolbar) método. El marco de trabajo cierra la barra de herramientas de la lista desplegable cuando el usuario presiona el botón izquierdo del ratón en el área no cliente de la barra de herramientas de la lista desplegable.  
  
##  <a name="isextrasize"></a>CMFCDropDownToolbarButton::IsExtraSize  
 Determina si se puede mostrar el botón con un borde extendido.  
  
```  
virtual BOOL IsExtraSize() const;  
```  
  
### <a name="return-value"></a>Valor devuelto  
 Es distinto de cero si se puede mostrar el botón de barra de herramientas con un borde extendido; en caso contrario es 0.  
  
### <a name="remarks"></a>Comentarios  
 Para obtener más información acerca de los bordes extendidos, vea [CMFCToolBarButton::IsExtraSize](../../mfc/reference/cmfctoolbarbutton-class.md#isextrasize).  
  
##  <a name="m_uishowbardelay"></a>CMFCDropDownToolbarButton::m_uiShowBarDelay  
 Especifica el período de tiempo que un usuario debe contener el botón del mouse hacia abajo antes de que aparezca la barra de herramientas de la lista desplegable.  
  
```  
static UINT m_uiShowBarDelay;  
```  
  
### <a name="remarks"></a>Comentarios  
 El tiempo de retardo se mide en milisegundos. El valor predeterminado es 500. Puede definir otra retraso cambiando el valor de este miembro de datos compartido.  
  
##  <a name="oncalculatesize"></a>CMFCDropDownToolbarButton::OnCalculateSize  
 Lo llama el marco de trabajo para calcular el tamaño del botón para el contexto de dispositivo especificado y el estado de acoplamiento.  
  
```  
virtual SIZE OnCalculateSize(
    CDC* pDC,  
    const CSize& sizeDefault,  
    BOOL bHorz);
```  
  
### <a name="parameters"></a>Parámetros  
 [in] `pDC`  
 El contexto de dispositivo que muestra el botón.  
  
 [in] `sizeDefault`  
 El tamaño predeterminado del botón.  
  
 [in] `bHorz`  
 El estado de acoplamiento de la barra de herramientas primario. Este parámetro es `TRUE` si la barra de herramientas está acoplado horizontalmente o está flotando, o `FALSE` si la barra de herramientas está acoplado verticalmente.  
  
### <a name="return-value"></a>Valor devuelto  
 Un `SIZE` estructura que contiene las dimensiones del botón, en píxeles.  
  
### <a name="remarks"></a>Comentarios  
 Este método extiende la implementación de la clase base ( [CMFCToolBarButton::OnCalculateSize](../../mfc/reference/cmfctoolbarbutton-class.md#oncalculatesize)) agregando el ancho de la flecha de lista desplegable a la dimensión horizontal del tamaño del botón.  
  
##  <a name="onchangeparentwnd"></a>CMFCDropDownToolbarButton::OnChangeParentWnd  
 Lo llama el marco cuando el botón se inserta en una nueva barra de herramientas.  
  
```  
virtual void OnChangeParentWnd(CWnd* pWndParent);
```  
  
### <a name="parameters"></a>Parámetros  
 [in] `pWndParent`  
 La nueva ventana primaria.  
  
### <a name="remarks"></a>Comentarios  
 Este método invalida la implementación de la clase base ( [CMFCToolBarButton::OnChangeParentWnd](../../mfc/reference/cmfctoolbarbutton-class.md#onchangeparentwnd)) mediante la desactivación de la etiqueta de texto ( [CMFCToolBarButton::m_strText](../../mfc/reference/cmfctoolbarbutton-class.md#m_strtext)) y estableciendo el [ CMFCToolBarButton::m_bText](../../mfc/reference/cmfctoolbarbutton-class.md#m_btext) y [CMFCToolBarButton::m_bUserButton](../../mfc/reference/cmfctoolbarbutton-class.md#m_buserbutton) los miembros de datos `FALSE`.  
  
##  <a name="onclick"></a>CMFCDropDownToolbarButton::OnClick  
 Lo llama el marco cuando el usuario hace clic en el botón del mouse.  
  
```  
virtual BOOL OnClick(
    CWnd* pWnd,  
    BOOL bDelay = TRUE);
```  
  
### <a name="parameters"></a>Parámetros  
 [in] `pWnd`  
 La ventana principal del botón de barra de herramientas.  
  
 [in] `bDelay`  
 `TRUE`Si el mensaje debe controlarse con un retraso.  
  
### <a name="return-value"></a>Valor devuelto  
 Es distinto de cero si el botón procesa el mensaje haga clic en; en caso contrario es 0.  
  
### <a name="remarks"></a>Comentarios  
 Este método extiende la implementación de la clase base, [CMFCToolBarButton::OnClick](../../mfc/reference/cmfctoolbarbutton-class.md#onclick), actualizando el estado de la barra de herramientas de la lista desplegable.  
  
 Cuando un usuario hace clic en el botón de barra de herramientas, este método crea un temporizador que espera a que el período de tiempo especificado por el [CMFCDropDownToolbarButton::m_uiShowBarDelay](#m_uishowbardelay) miembro de datos y, a continuación, se abre la lista desplegable barra de herramientas mediante el uso de la [CMFCDropDownToolbarButton::DropDownToolbar](#dropdowntoolbar) método. Este método cierra la segunda vez que el usuario hace clic en el botón de barra de herramientas de la barra de herramientas de la lista desplegable.  
  
##  <a name="onclickup"></a>CMFCDropDownToolbarButton::OnClickUp  
 Lo llama el marco cuando el usuario suelta el botón del mouse.  
  
```  
virtual BOOL OnClickUp();
```  
  
### <a name="return-value"></a>Valor devuelto  
 Es distinto de cero si el botón procesa el mensaje haga clic en; en caso contrario es 0.  
  
### <a name="remarks"></a>Comentarios  
 Este método extiende la implementación de la clase base, [CMFCToolBarButton::OnClickUp](../../mfc/reference/cmfctoolbarbutton-class.md#onclickup), actualizando el estado de la barra de herramientas de la lista desplegable.  
  
 Este método detiene el temporizador de la barra de herramientas de lista desplegable si está activa. Cierra la barra de herramientas de la lista desplegable si está abierto.  
  
 Para obtener más información acerca de la barra de herramientas de lista desplegable y el temporizador de la barra de herramientas de lista desplegable, consulte [CMFCDropDownToolbarButton::OnClick](#onclick).  
  
##  <a name="oncontexthelp"></a>CMFCDropDownToolbarButton::OnContextHelp  
 Lo llama el marco cuando la barra de herramientas primario controla un `WM_HELPHITTEST` mensaje.  
  
```  
virtual BOOL OnContextHelp(CWnd* pWnd);
```  
  
### <a name="parameters"></a>Parámetros  
 [in] `pWnd`  
 La ventana principal del botón de barra de herramientas.  
  
### <a name="return-value"></a>Valor devuelto  
 Es distinto de cero si el botón procesa el mensaje de ayuda; en caso contrario es 0.  
  
### <a name="remarks"></a>Comentarios  
 Este método extiende la implementación de la clase base ( [CMFCToolBarButton::OnContextHelp](../../mfc/reference/cmfctoolbarbutton-class.md#oncontexthelp)) mediante una llamada a la [CMFCDropDownToolbarButton::OnClick](#onclick) método con `bDelay` establecido en `FALSE` . Este método devuelve el valor devuelto por [CMFCDropDownToolbarButton::OnClick](#onclick).  
  
 Para obtener más información sobre la `WM_HELPHITTEST message, see` [TN028: compatibilidad con la Ayuda contextual](../../mfc/tn028-context-sensitive-help-support.md).  
  
##  <a name="oncustomizemenu"></a>CMFCDropDownToolbarButton::OnCustomizeMenu  
 Modifica el menú proporcionado cuando la aplicación muestra un menú contextual en la barra de herramientas primario.  
  
```  
virtual BOOL OnCustomizeMenu(CMenu* pMenu);
```  
  
### <a name="parameters"></a>Parámetros  
 [in] `pMenu`  
 El menú para personalizar.  
  
### <a name="return-value"></a>Valor devuelto  
 Este método devuelve `TRUE`.  
  
### <a name="remarks"></a>Comentarios  
 Este método extiende la implementación de la clase base ( [CMFCToolBarButton::OnCustomizeMenu](../../mfc/reference/cmfctoolbarbutton-class.md#oncustomizemenu)) deshabilitando los siguientes elementos de menú:  
  
- **Copiar imagen del botón**  
  
- **Apariencia del botón**  
  
- **Image**  
  
- **Texto**  
  
- **Imagen y texto**  
  
 Invalide este método para modificar el acceso directo que el marco de trabajo se muestra en el modo de personalización.  
  
##  <a name="ondraw"></a>CMFCDropDownToolbarButton::OnDraw  
 Lo llama el marco de trabajo para dibujar el botón con los estilos especificados y las opciones.  
  
```  
virtual void OnDraw(
    CDC* pDC,  
    const CRect& rect,  
    CMFCToolBarImages* pImages,  
    BOOL bHorz = TRUE,  
    BOOL bCustomizeMode = FALSE,  
    BOOL bHighlight = FALSE,  
    BOOL bDrawBorder = TRUE,  
    BOOL bGrayDisabledButtons = TRUE);
```  
  
### <a name="parameters"></a>Parámetros  
 [in] `pDC`  
 El contexto de dispositivo que muestra el botón.  
  
 [in] `rect`  
 El rectángulo delimitador del botón.  
  
 [in] `pImages`  
 La colección de imágenes de barra de herramientas que está asociada con el botón.  
  
 [in] `bHorz`  
 El estado de acoplamiento de la barra de herramientas primario. Este parámetro es `TRUE` cuando el botón está acoplado horizontalmente y `FALSE` cuando el botón está acoplado verticalmente.  
  
 [in] `bCustomizeMode`  
 Especifica si la barra de herramientas está en modo de personalización. Este parámetro es `TRUE` cuando la barra de herramientas está en modo de personalización y `FALSE` cuando la barra de herramientas no está en modo de personalización.  
  
 [in] `bHighlight`  
 Especifica si se resalta el botón. Este parámetro es `TRUE` cuando se resalta el botón y `FALSE` cuando no se resalta el botón.  
  
 [in] `bDrawBorder`  
 Especifica si el botón debe mostrar su borde. Este parámetro es `TRUE` cuando el botón debería mostrar su borde y `FALSE` cuando el botón no debería aparecer su borde.  
  
 [in] `bGrayDisabledButtons`  
 Especifica si se sombrean botones deshabilitados o usar la colección de imágenes deshabilitado. Este parámetro es `TRUE` cuando los botones deshabilitados deben estar atenuada y `FALSE` cuando este método debe utilizar la colección de imágenes deshabilitado.  
  
### <a name="remarks"></a>Comentarios  
 Invalide este método para personalizar el dibujo de botón de barra de herramientas.  
  
##  <a name="ondrawoncustomizelist"></a>CMFCDropDownToolbarButton::OnDrawOnCustomizeList  
 Lo llama el marco para dibujar el botón el **comandos** panel de la **personalizar** cuadro de diálogo.  
  
```  
virtual int OnDrawOnCustomizeList(
    CDC* pDC,  
    const CRect& rect,  
    BOOL bSelected);
```  
  
### <a name="parameters"></a>Parámetros  
 [in] `pDC`  
 El contexto de dispositivo que muestra el botón.  
  
 [in] `rect`  
 El rectángulo delimitador del botón.  
  
 [in] `bSelected`  
 Si el botón está seleccionado. Si este parámetro es `TRUE`, el botón está seleccionado. Si este parámetro es `FALSE`, el botón no está seleccionado.  
  
### <a name="return-value"></a>Valor devuelto  
 El ancho, en píxeles, del botón en el contexto de dispositivo especificado.  
  
### <a name="remarks"></a>Comentarios  
 Este método es invocado por el cuadro de diálogo de personalización ( **comandos** ficha) ¿cuándo se necesita el botón para que aparezca en el cuadro de lista dibujado por el propietario.  
  
 Este método extiende la implementación de la clase base ( [CMFCToolBarButton::OnDrawOnCustomizeList](../../mfc/reference/cmfctoolbarbutton-class.md#ondrawoncustomizelist)) cambiando la etiqueta de texto del botón en el nombre del botón (es decir, en el valor de la `lpszName` parámetro que se pasó en el constructor).  
  
##  <a name="serialize"></a>CMFCDropDownToolbarButton::Serialize  
 Lee este objeto desde un archivo o lo escribe en un archivo.  
  
```  
virtual void Serialize(CArchive& ar);
```  
  
### <a name="parameters"></a>Parámetros  
 [in] `ar`  
 La `CArchive` objeto desde la que o que se va a serializar.  
  
### <a name="remarks"></a>Comentarios  
 Este método extiende la implementación de la clase base ( [CMFCToolBarButton::Serialize](../../mfc/reference/cmfctoolbarbutton-class.md#serialize)) al serializar el identificador de recurso de la barra de herramientas primario. Cuando se está cargando el archivo ( [CArchive::IsLoading](../../mfc/reference/carchive-class.md#isloading) devuelve un valor distinto de cero), este método establece la `m_pToolBar` miembro de datos a la barra de herramientas que contiene el identificador de recurso serializado.  
  
##  <a name="setdefaultcommand"></a>CMFCDropDownToolbarButton::SetDefaultCommand  
 Establece el comando predeterminado que el marco de trabajo que se usa cuando un usuario hace clic en el botón.  
  
```  
void SetDefaultCommand(UINT uiCmd);
```  
  
### <a name="parameters"></a>Parámetros  
 [in] `uiCmd`  
 El identificador del comando predeterminado.  
  
### <a name="remarks"></a>Comentarios  
 Llamar a este método para especificar un comando predeterminado que el marco de trabajo se ejecuta cuando el usuario hace clic en el botón. Un elemento con el identificador de comando especificado por `uiCmd` debe estar ubicado en la barra de herramientas de la lista desplegable elemento primario.  
  
## <a name="see-also"></a>Vea también  
 [Gráfico de jerarquías](../../mfc/hierarchy-chart.md)   
 [Clases](../../mfc/reference/mfc-classes.md)   
 [Clase de CMFCDropDownToolBar](../../mfc/reference/cmfcdropdowntoolbar-class.md)   
 [Clase CMFCToolBar](../../mfc/reference/cmfctoolbar-class.md)   
 [Clase CMFCToolBarMenuButton](../../mfc/reference/cmfctoolbarmenubutton-class.md)   
 [Tutorial: Poner controles en las barras de herramientas](../../mfc/walkthrough-putting-controls-on-toolbars.md)


