---
title: "ISymUnmanagedReaderSymbolSearchInfo::GetSymbolSearchInfo Method | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework-4.6"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "dotnet-clr"
ms.tgt_pltfrm: ""
ms.topic: "reference"
apiname: 
  - "ISymUnmanagedReaderSymbolSearchInfo.GetSymbolSearchInfo"
apilocation: 
  - "diasymreader.dll"
apitype: "COM"
f1_keywords: 
  - "ISymUnmanagedReaderSymbolSearchInfo::GetSymbolSearchInfo"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "GetSymbolSearchInfo method [.NET Framework debugging]"
  - "ISymUnmanagedReaderSymbolSearchInfo::GetSymbolSearchInfo method [.NET Framework debugging]"
ms.assetid: 40fcdbc5-3bb2-41e9-b995-40984c209a7f
caps.latest.revision: 9
author: "mairaw"
ms.author: "mairaw"
manager: "wpickett"
---
# ISymUnmanagedReaderSymbolSearchInfo::GetSymbolSearchInfo Method
Gets symbol search information.  
  
## Syntax  
  
```  
HRESULT GetSymbolSearchInfo(  
    [in]  ULONG32  cSearchInfo,  
    [out] ULONG32  *pcSearchInfo,  
    [out, size_is(cSearchInfo), length_is(*pcSearchInfo)]  
        ISymUnmanagedSymbolSearchInfo **rgpSearchInfo);  
```  
  
#### Parameters  
 `cSearchInfo`  
 [in] A `ULONG32` that indicates the size of `rgpSearchInfo`.  
  
 `pcSearchInfo`  
 [out] A pointer to a `ULONG32` that receives the size of the buffer required to contain the search information.  
  
 `rgpSearchInfo`  
 [out] A pointer that is set to the returned [ISymUnmanagedSymbolSearchInfo](../../../../docs/framework/unmanaged-api/diagnostics/isymunmanagedsymbolsearchinfo-interface.md) interface.  
  
## Return Value  
 S_OK if the method succeeds; otherwise, E_FAIL or some other error code.  
  
## Requirements  
 **Header:** CorSym.idl, CorSym.h  
  
## See Also  
 [ISymUnmanagedReaderSymbolSearchInfo Interface](../../../../docs/framework/unmanaged-api/diagnostics/isymunmanagedreadersymbolsearchinfo-interface.md)