---
title: Viewer.ReviewerName property (Visio Viewer)
ms.prod: visio
api_name:
- Visio.Viewer.ReviewerName
ms.assetid: 69127a8e-bb16-1162-e3a1-d4fd0288dc5c
ms.date: 06/21/2019
ms.localizationpriority: medium
---


# Viewer.ReviewerName property (Visio Viewer)

Gets the name of the specified reviewer in the drawing that is open in Microsoft Visio Viewer. Read-only.


## Syntax

_expression_.**ReviewerName** (_ReviewerIndex_)

_expression_ An expression that returns a **[Viewer](Visio.Viewer.md)** object.


## Parameters

|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
|_ReviewerIndex_|Required| **Long**|The index of the reviewer in the collection of reviewers.|

## Return value

**String**


## Remarks

The collection of reviewers is one-based, so the index of the first reviewer in the collection is 1. If there are no reviewers in the drawing, or if you pass the index of a nonexistent reviewer, Visio Viewer returns an error.


## Example

The following code gets the names of all reviewers in the drawing that is open in Visio Viewer.

```vb
Dim intCounter As Integer

    For intCounter = 1 To Viewer1.ReviewerCount

    Debug.Print Viewer1.ReviewerName(intCounter)

Next intCounter

```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]