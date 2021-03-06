---
title: "barrier | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: ["cpp-windows"]
ms.tgt_pltfrm: ""
ms.topic: "reference"
f1_keywords: ["barrier"]
dev_langs: ["C++"]
helpviewer_keywords: ["barrier OpenMP directive"]
ms.assetid: 5c73ad4f-c768-443a-8f9e-4fd8bc2253c7
caps.latest.revision: 8
author: "mikeblome"
ms.author: "mblome"
manager: "ghogen"
ms.workload: ["cplusplus"]
---
# barrier
Synchronizes all threads in a team; all threads pause at the barrier, until all threads execute the barrier.  
  
## Syntax  
  
```  
#pragma omp barrier  
```  
  
## Remarks  
 The `barrier` directive supports no OpenMP clauses.  
  
 For more information, see [2.6.3 barrier Directive](../../../parallel/openmp/2-6-3-barrier-directive.md).  
  
## Example  
 For a sample of how to use `barrier`, see [master](../../../parallel/openmp/reference/master.md).  
  
## See Also  
 [Directives](../../../parallel/openmp/reference/openmp-directives.md)