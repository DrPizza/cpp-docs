---
title: "2.7.2.4 shared | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: ["cpp-windows"]
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: ["C++"]
ms.assetid: c9c5d653-58fc-4620-ab0a-443ac4f8ba2e
caps.latest.revision: 5
author: "mikeblome"
ms.author: "mblome"
manager: "ghogen"
ms.workload: ["cplusplus"]
---
# 2.7.2.4 shared
This clause shares variables that appear in the *variable-list* among all the threads in a team. All threads within a team access the same storage area for **shared** variables.  
  
 The syntax of the **shared** clause is as follows:  
  
```  
shared(variable-list)  
```