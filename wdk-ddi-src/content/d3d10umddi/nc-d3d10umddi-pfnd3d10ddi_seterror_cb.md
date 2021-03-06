---
UID: NC:d3d10umddi.PFND3D10DDI_SETERROR_CB
title: PFND3D10DDI_SETERROR_CB
author: windows-driver-content
description: The pfnSetErrorCb function sets the return error code of a user-mode display driver's function.
old-location: display\pfnseterrorcb.htm
ms.assetid: 968b04a7-8869-410c-a6fc-83d57726858f
ms.author: windowsdriverdev
ms.date: 5/10/2018
ms.keywords: PFND3D10DDI_SETERROR_CB, PFND3D10DDI_SETERROR_CB callback, d3d10state_functions_1d57cbc9-ec37-47ce-ab4f-71535419375a.xml, d3d10umddi/pfnSetErrorCb, display.pfnseterrorcb, pfnSetErrorCb, pfnSetErrorCb callback function [Display Devices]
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: callback
req.header: d3d10umddi.h
req.include-header: D3d10umddi.h
req.target-type: Desktop
req.target-min-winverclnt: Available in Windows Vista and later versions of the Windows operating systems.
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	UserDefined
api_location:
-	d3d10umddi.h
api_name:
-	pfnSetErrorCb
product:
- Windows
targetos: Windows
tech.root: display
req.typenames: 
---

# PFND3D10DDI_SETERROR_CB callback function


## -description


The <b>pfnSetErrorCb</b> function sets the return error code of a user-mode display driver's function.


## -parameters




### -param Arg1


### -param Arg2








#### - hResult [in]

 An HRESULT value that specifies the error to set for a driver function. 


#### - hRuntimeDevice [in]

 A handle to a context for the core Microsoft Direct3D 10 runtime. This handle is supplied to the driver in a call to the driver's <a href="https://msdn.microsoft.com/c69eedb1-c975-412c-aa9f-cf64a702f937">CreateDevice(D3D10)</a> function. 


## -returns



None




## -remarks



A user-mode display driver can call <b>pfnSetErrorCb</b> many times for each driver invocation. For the driver's functions that do not return status codes, the driver uses <b>pfnSetErrorCb</b> to return error information to the Direct3D runtime. 




## -see-also




<a href="https://msdn.microsoft.com/c69eedb1-c975-412c-aa9f-cf64a702f937">CreateDevice(D3D10)</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff541820">D3D10DDI_CORELAYER_DEVICECALLBACKS</a>
 

 

