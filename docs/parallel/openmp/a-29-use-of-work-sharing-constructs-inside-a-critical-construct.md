---
title: "A.29   Use of Work-Sharing Constructs Inside a critical Construct | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: ["cpp-windows"]
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: ["C++"]
ms.assetid: d5c8a83f-2f51-4f23-8ddf-d267e347507f
caps.latest.revision: 5
author: "mikeblome"
ms.author: "mblome"
manager: "ghogen"
ms.workload: ["cplusplus"]
---
# A.29   Use of Work-Sharing Constructs Inside a critical Construct
The following example demonstrates using a work-sharing construct inside a `critical` construct. This example is compliant because the work-sharing construct and the `critical` construct do not bind to the same parallel region.  
  
```  
void f()  
{  
  int i = 1;  
  #pragma omp parallel sections  
  {  
    #pragma omp section  
    {  
      #pragma omp critical (name)  
      {  
        #pragma omp parallel  
        {  
          #pragma omp single  
          {  
            i++;  
          }  
        }  
      }  
    }  
  }  
}  
```