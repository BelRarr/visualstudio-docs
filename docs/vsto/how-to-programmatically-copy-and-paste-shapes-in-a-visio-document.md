---
title: "How to: Programmatically Copy and Paste Shapes in a Visio Document | Microsoft Docs"
ms.custom: ""
ms.date: "02/02/2017"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "office-development"
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: 
  - "VB"
  - "CSharp"
helpviewer_keywords: 
  - "shapes [Office development in Visual Studio], copying and pasting Visio shapes"
  - "Visio [Office development in Visual Studio], copying and pasting Visio shapes"
ms.assetid: 762d95cf-2d5c-4dea-988b-8f4da88fa1f1
caps.latest.revision: 15
author: "kempb"
ms.author: "kempb"
manager: "ghogen"
---
# How to: Programmatically Copy and Paste Shapes in a Visio Document
  You can programmatically copy shapes on one page of a document and paste them into a new page in the same document. You can choose to paste them into the default location (the center of the active window) or into the same coordinate locations as they had on the original page.  
  
## Copying and Pasting Shapes  
 For details about the object model, see the VBA reference documentation for the [Microsoft.Office.Interop.Visio.Shape.DrawRectangle](HV10070304), [Microsoft.Office.Interop.Visio.Shape.DrawOval](HV10070300), [Microsoft.Office.Interop.Visio.Shape.Copy](HV10070291), and [Microsoft.Office.Interop.Visio.Shape.Paste](HV10070437) methods and the [Microsoft.Office.Interop.Visio.VisCutCopyPasteCodes.visCopyPasteNormal](HV10071835) flag.  
  
#### To copy shapes to the center of another page  
  
-   The following example demonstrates how to copy the shapes from the first page and paste them into the center of the second page.  
  
     [!code-cs[Trin_VstcoreVisioAutomationAddIn#14](../vsto/codesnippet/CSharp/trin_vstcorevisioautomationaddin/ThisAddIn.cs#14)]
     [!code-vb[Trin_VstcoreVisioAutomationAddIn#14](../vsto/codesnippet/VisualBasic/trin_vstcorevisioautomationaddin/ThisAddIn.vb#14)]  
  
## Copying and Pasting Shapes With the Same Positions  
 For details about the object model, see the VBA reference documentation for the [Microsoft.Office.Interop.Visio.Shape.DrawRectangle](HV10070304), [Microsoft.Office.Interop.Visio.Shape.DrawOval](HV10070300), [Microsoft.Office.Interop.Visio.Shape.Copy](HV10070291), and [Microsoft.Office.Interop.Visio.Shape.Paste](HV10070437) methods and the [Microsoft.Office.Interop.Visio.VisCutCopyPasteCodes.visCopyPasteNoTranslate](HV10071835) flag.  
  
 If you need to control the format of the pasted information and (optionally) establish a link to a source file (for example, a Microsoft Office Word document), use the PasteSpecial method.  
  
#### To copy shapes and shape locations to another page  
  
-   The following example demonstrates how to copy the shapes from the first page and paste them into the second page with their original coordinate locations.  
  
     [!code-cs[Trin_VstcoreVisioAutomationAddIn#15](../vsto/codesnippet/CSharp/trin_vstcorevisioautomationaddin/ThisAddIn.cs#15)]
     [!code-vb[Trin_VstcoreVisioAutomationAddIn#15](../vsto/codesnippet/VisualBasic/trin_vstcorevisioautomationaddin/ThisAddIn.vb#15)]  
  
## See Also  
 [Visio Solutions](../vsto/visio-solutions.md)   
 [Visio Object Model Overview](../vsto/visio-object-model-overview.md)   
 [Working with Visio Shapes](../vsto/working-with-visio-shapes.md)   
 [How to: Programmatically Add Shapes to a Visio Document](../vsto/how-to-programmatically-add-shapes-to-a-visio-document.md)  
  
  