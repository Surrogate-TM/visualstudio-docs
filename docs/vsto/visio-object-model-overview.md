---
title: "Visio object model overview"
description: Learn how you can interact with the Visio object model to develop Office solutions for Microsoft Visio.
ms.custom: SEO-VS-2020
ms.date: "02/02/2017"
ms.topic: "conceptual"
dev_langs:
  - "VB"
  - "CSharp"
helpviewer_keywords:
  - "Visio [Office development in Visual Studio], object model"
  - "object models [Office development in Visual Studio], Office"
  - "object models [Office development in Visual Studio], Visio"
  - "objects [Office development in Visual Studio], Office object models"
  - "Office object models"
  - "Visio object model"
author: John-Hart
ms.author: johnhart
manager: jmartens
ms.technology: office-development
ms.workload:
  - "office"
---
# Visio object model overview

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
  To develop Office solutions for Microsoft Office Visio, you can interact with the Visio object model. This object model consists of classes and interfaces that are provided in the primary interop assembly for Visio, and are defined in the `Microsoft.Office.Interop.Visio` namespace.

 This topic provides a brief overview of the Visio object model. For information about using the Visio object model to perform tasks in Office projects, see the following topics:

- [Work with Visio documents](../vsto/working-with-visio-documents.md)

- [Work with Visio shapes](../vsto/working-with-visio-shapes.md)

## Understand the Visio object model
 Visio provides many objects with which you can interact. These objects are organized in a hierarchy that closely follows the user interface. At the top of the hierarchy is the [Microsoft.Office.Interop.Visio.Application](/office/vba/api/Visio.Application) object. This object represents the current instance of Visio. The `Microsoft.Office.Interop.Visio.Application` object contains the `Microsoft.Office.Interop.Visio.Document` and `Microsoft.Office.Interop.Visio.Page` objects as well as the `Microsoft.Office.Interop.Visio.Documents` and `Microsoft.Office.Interop.Visio.Pages` collections. Each of these objects and collections has many methods and properties that you can access to manipulate and interact with it.

 For more information, see the VBA reference documentation for [Microsoft.Office.Interop.Visio.Application](/office/vba/api/Visio.Application), [Microsoft.Office.Interop.Visio.Document](/office/vba/api/Visio.Document), and [Microsoft.Office.Interop.Visio.Page](/office/vba/api/Visio.Page) objects, and also the [Microsoft.Office.Interop.Visio.Documents](/office/vba/api/Visio.Documents) and [Microsoft.Office.Interop.Visio.Pages](/office/vba/api/Visio.Pages) collections.

 The following sections briefly describe the top-level objects and how they interact with each other. These objects include the following objects:

- Application object

- Document object

- Page object

### Graphical representation of Visio object model
 Please refer to the following links for more information on other notable Visio objects.    
**[Global](https://docs.microsoft.com/en-us/office/vba/api/visio.global "Global collection (Visio)")** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; [ThisDocument](https://docs.microsoft.com/en-us/office/vba/api/visio.thisdocument "ThisDocumentobject (Visio)")    
├┉┉ [ActiveDocument](https://docs.microsoft.com/en-us/office/vba/api/visio.activedocument "ActiveDocument object (Visio)")    
├┉┉ [ActivePage](https://docs.microsoft.com/en-us/office/vba/api/visio.ActivePage "ActivePage object (Visio)")    
├┉┉ [ActiveWindow](https://docs.microsoft.com/en-us/office/vba/api/visio.activewindow "ActiveWindow object (Visio)")    
├┉┉ [Application](https://docs.microsoft.com/en-us/office/vba/api/visio.application "Application object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├ [ApplicationSettings](https://docs.microsoft.com/en-us/office/vba/api/visio.applicationsettings "ApplicationSettings object (Visio)")    
├┉┉├ [VBE](https://docs.microsoft.com/en-us/office/vba/api/visio.application.vbe "VBE object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├ [CommandBars](https://docs.microsoft.com/en-us/office/vba/api/office.commandbars "CommandBars object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├ [COMAddIns](https://docs.microsoft.com/en-us/office/vba/api/visio.application.comaddins "COMAddIns collection (Visio)")    
├┉┉├ **[Documents](https://docs.microsoft.com/en-us/office/vba/api/visio.documents "Documents collection (Visio)")**    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│└ [Document](https://docs.microsoft.com/en-us/office/vba/api/visio.document "Document object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;├ **[Pages](https://docs.microsoft.com/en-us/office/vba/api/visio.pages "Pages collection (Visio)")**    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp; │└ [Page](https://docs.microsoft.com/en-us/office/vba/api/visio.page "Page object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp; ├ **[Shapes](https://docs.microsoft.com/en-us/office/vba/api/visio.shapes "Shapes collection (Visio)")**    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│└ [Shape](https://docs.microsoft.com/en-us/office/vba/api/visio.shape "Shape object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp; ├ **[Shapes](https://docs.microsoft.com/en-us/office/vba/api/visio.shapes "Sub-shapes collection (Visio)" )**    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│ └ [Shape](https://docs.microsoft.com/en-us/office/vba/api/visio.shape "Sub-shape object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;├ **[Connects](https://docs.microsoft.com/en-us/office/vba/api/visio.connects "Connects collection (Visio)")**    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│ └ [Connect](https://docs.microsoft.com/en-us/office/vba/api/visio.connect "Connect object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;├ **[Hyperlinks](https://docs.microsoft.com/en-us/office/vba/api/visio.hyperlinks "Hyperlinks collection (Visio)")**    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│ └ [Hyperlink](https://docs.microsoft.com/en-us/office/vba/api/visio.hyperlink "Hyperlink object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;├ [Characters](https://docs.microsoft.com/en-us/office/vba/api/visio.characters "Characters object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp; ├ [Section](https://docs.microsoft.com/en-us/office/vba/api/visio.section "Section object (Visio)") — [Row](https://docs.microsoft.com/en-us/office/vba/api/visio.row "Row object (Visio)") — [Cell](https://docs.microsoft.com/en-us/office/vba/api/visio.cell "Cell object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp; └ **[Paths](https://docs.microsoft.com/en-us/office/vba/api/visio.paths "Paths collection (Visio)")**    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; └ [Path](https://docs.microsoft.com/en-us/office/vba/api/visio.path "Path object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp; └ [Curve](https://docs.microsoft.com/en-us/office/vba/api/visio.curve "Curve object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp; ├ **[Connects](https://docs.microsoft.com/en-us/office/vba/api/visio.connects "Connects collection (Visio)")**    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│ └ [ Connect](https://docs.microsoft.com/en-us/office/vba/api/visio.connect "Connect object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp; ├ **[Layers](https://docs.microsoft.com/en-us/office/vba/api/visio.layers "Layers collection (Visio)")**    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│ └ [ Layer](https://docs.microsoft.com/en-us/office/vba/api/visio.layer "Layer object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp; └ **[OLEObjects](https://docs.microsoft.com/en-us/office/vba/api/visio.oleobjects "OLEObjects collection (Visio)")**    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; └ [OLEObject](https://docs.microsoft.com/en-us/office/vba/api/visio.oleobject "OLEObject object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;├ **[Masters](https://docs.microsoft.com/en-us/office/vba/api/visio.masters "Masters collection (Visio)")**    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp; │ └ [Master](https://docs.microsoft.com/en-us/office/vba/api/visio.master "Master object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp; ├ **[Colors ](https://docs.microsoft.com/en-us/office/vba/api/visio.colors "Colors collection (Visio)")**    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp; │ └ [Color](https://docs.microsoft.com/en-us/office/vba/api/visio.color "Color object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;├ **[Fonts ](https://docs.microsoft.com/en-us/office/vba/api/visio.fonts "Fonts collection (Visio)")**    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp; │ └ [Font](https://docs.microsoft.com/en-us/office/vba/api/visio.font "Font object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;├ **[MasterShortcuts](https://docs.microsoft.com/en-us/office/vba/api/visio.mastershortcuts "MasterShortcuts collection (Visio)")**    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp; │ └ [MasterShortcut](https://docs.microsoft.com/en-us/office/vba/api/visio.mastershortcut "MasterShortcut object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;├ **[OLEObjects](https://docs.microsoft.com/en-us/office/vba/api/visio.oleobjects "OLEObjects collection (Visio)")**    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp; │ └ [OLEObject](https://docs.microsoft.com/en-us/office/vba/api/visio.oleobject "OLEObject object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;├ **[Styles](https://docs.microsoft.com/en-us/office/vba/api/visio.styles "Styles collection (Visio)")**    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp; │ └ [Style](https://docs.microsoft.com/en-us/office/vba/api/visio.style "Style object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;└ [VBProject](https://docs.microsoft.com/en-us/office/vba/api/visio.vbproject "VBProject object (Visio)")    
├┉┉├ **[Windows](https://docs.microsoft.com/en-us/office/vba/api/visio.windows "Windows collection (Visio)")**    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│└ [Window](https://docs.microsoft.com/en-us/office/vba/api/visio.window "Window object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;  ├ [Selection](https://docs.microsoft.com/en-us/office/vba/api/visio.selection "Selection object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;  ├ [Document](https://docs.microsoft.com/en-us/office/vba/api/visio.document "Document object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;  ├ [Master](https://docs.microsoft.com/en-us/office/vba/api/visio.master "Master object (Visio)")    
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;  └ [Page](https://docs.microsoft.com/en-us/office/vba/api/visio.page "Page object (Visio)")    
└┉┉├ **[Addons](https://docs.microsoft.com/en-us/office/vba/api/visio.addons "Addons collection (Visio)")**    
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│└ [Addon](https://docs.microsoft.com/en-us/office/vba/api/visio.document "Document object (Visio)")    
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ├ **[EventList](https://docs.microsoft.com/en-us/office/vba/api/visio.eventlist "EventList collection (Visio)")**    
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; │└ [Event](https://docs.microsoft.com/en-us/office/vba/api/visio.event "Event object (Visio)")    
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; └ [UIObject](https://docs.microsoft.com/en-us/office/vba/api/visio.uiobject "UIObject object (Visio)")    
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ├ **[AccelTables](https://docs.microsoft.com/en-us/office/vba/api/visio.acceltables "AccelTables collection (Visio)")**    
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; │└ [AccelTable](https://docs.microsoft.com/en-us/office/vba/api/visio.acceltable "AccelTable object (Visio)")    
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ├ **[MenuSets](https://docs.microsoft.com/en-us/office/vba/api/visio.menusets "MenuSets collection (Visio)")**    
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; │└ [MenuSet](https://docs.microsoft.com/en-us/office/vba/api/visio.menuset "MenuSet object (Visio)")    
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; └ **[ToolbarSets](https://docs.microsoft.com/en-us/office/vba/api/visio.toolbarsets "ToolbarSets collection (Visio)")**    
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; └ [ToolbarSet](https://docs.microsoft.com/en-us/office/vba/api/visio.toolbarset "ToolbarSet object (Visio)")    

### Application object
 The Microsoft.Office.Interop.Visio.Application object represents the Visio application, and is the parent of all of the other objects. Its members usually apply to Visio as a whole. You can use the properties and methods of the Microsoft.Office.Interop.Visio.Application and the `Microsoft.Office.Interop.Visio.ApplicationSettings` objects to control the Visio environment.

 In VSTO Add-in projects, you can access the Microsoft.Office.Interop.Visio.Application object by using the `Application` field of the `ThisAddIn` class. For more information, see [Programming VSTO Add-Ins](../vsto/programming-vsto-add-ins.md).

### Document object
 The Microsoft.Office.Interop.Visio.Document object is central to programming Visio. It represents a drawing, stencil, or template file. When you open a Visio document or create a new document, you create a new Microsoft.Office.Interop.Visio.Document object, which is added to the Microsoft.Office.Interop.Visio.Documents collection of the Microsoft.Office.Interop.Visio.Application object.

 The document that has the focus is called the active document. It is represented by the `Microsoft.Office.Interop.Visio.Application.ActiveDocument` property of the Microsoft.Office.Interop.Visio.Application object.

### Page object
 The Microsoft.Office.Interop.Visio.Page object represents the drawing area of a foreground page or a background page. You can use the `Microsoft.Office.Interop.Visio.Page.Background` property to determine whether a page is a foreground or background page.

 To create shapes, you can use methods that include the `Microsoft.Office.Interop.Visio.Page.DrawSpline` and `Microsoft.Office.Interop.Visio.Page.DrawOval` methods. Additionally, you can retrieve masters from stencils and place the shapes on a page by using the `Microsoft.Office.Interop.Visio.Page.Drop` or `Microsoft.Office.Interop.Visio.Page.DropMany` methods.

## Use the Visio object model documentation
 For complete information about the Visio object model, you can refer to the Visio VBA object model reference. The VBA object model reference documents the Visio object model as it is exposed to Visual Basic for Applications (VBA) code. For more information, see [Visio object model reference](/office/vba/api/overview/visio/object-model).

 All of the objects and members in the VBA object model reference correspond to types and members in the Visio primary interop assembly (PIA). For example, the `Document` object in the VBA object model reference corresponds to the Microsoft.Office.Interop.Visio.Document type in the Visio PIA. Although the VBA object model reference provides code examples for most properties, methods, and events, you must translate the VBA code in this reference to Visual Basic or Visual C# if you want to use them in a Visio VSTO Add-in project that you create by using Visual Studio.

> [!NOTE]
> At this time, there is no reference documentation for the Visio primary interop assembly.

 For related code samples and additional tools for creating Visio solutions, see [Visio 2010 software development kit](https://www.microsoft.com/download/details.aspx?id=12365).

### Additional types in primary interop assemblies
 You can find types in the primary interop assemblies that are not visible to VBA because of implementation differences. VBA provides a view of the Visio object model that includes only the objects and members that you can use directly. The primary interop assemblies expose the same object model, but they also include other interfaces, classes, and members that translate objects in the COM object model to managed code. These additional items are not intended to be used directly in your code.

 For more information, see [Overview of classes and interfaces in the Office primary interop assemblies](/previous-versions/office/office-12/ms247299(v=office.12)) and [Office primary interop assemblies](../vsto/office-primary-interop-assemblies.md).

## See also
- [Visio solutions](../vsto/visio-solutions.md)
- [Work with Visio documents](../vsto/working-with-visio-documents.md)
- [Work with Visio shapes](../vsto/working-with-visio-shapes.md)
