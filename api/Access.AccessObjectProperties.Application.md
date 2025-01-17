---
title: AccessObjectProperties.Application property (Access)
keywords: vbaac10.chm12699
f1_keywords:
- vbaac10.chm12699
ms.prod: access
api_name:
- Access.AccessObjectProperties.Application
ms.assetid: cbb83705-3e37-599e-4314-d247dfe99ef9
ms.date: 02/01/2019
ms.localizationpriority: medium
---


# AccessObjectProperties.Application property (Access)

Use the **Application** property to access the active Microsoft Access **[Application](Access.Application.md)** object and its related properties. Read-only **Application** object.


## Syntax

_expression_.**Application**

_expression_ A variable that represents an **[AccessObjectProperties](Access.AccessObjectProperties.md)** object.


## Remarks

The **Application** property is set by Microsoft Access and is read-only in all views.

Each Microsoft Access object has an **Application** property that returns the current **Application** object. Use this property to access any of the object's properties. For example, you could refer to the menu bar for the **Application** object from the current form by using the following syntax.

```vb
Me.Application.MenuBar 

```



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]