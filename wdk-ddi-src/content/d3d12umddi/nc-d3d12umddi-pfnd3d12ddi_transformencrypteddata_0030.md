---
UID: NC:d3d12umddi.PFND3D12DDI_TRANSFORMENCRYPTEDDATA_0030
title: PFND3D12DDI_TRANSFORMENCRYPTEDDATA_0030
author: windows-driver-content
description: Used to transform encrypted data.
old-location: display\pfnd3d12ddi_transformencrypteddata_0030.htm
ms.assetid: B738C096-E821-4D7E-A713-47300E4E3779
ms.author: windowsdriverdev
ms.date: 5/10/2018
ms.keywords: PFND3D12DDI_TRANSFORMENCRYPTEDDATA_0030, PFND3D12DDI_TRANSFORMENCRYPTEDDATA_0030 callback, PFND3D12DDI_TRANSFORMENCRYPTEDDATA_0030 callback function [Display Devices], d3d12umddi/PFND3D12DDI_TRANSFORMENCRYPTEDDATA_0030, display.pfnd3d12ddi_transformencrypteddata_0030
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: callback
req.header: d3d12umddi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
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
-	d3d12umddi.h
api_name:
-	PFND3D12DDI_TRANSFORMENCRYPTEDDATA_0030
product:
- Windows
targetos: Windows
tech.root: display
req.typenames: 
---

# PFND3D12DDI_TRANSFORMENCRYPTEDDATA_0030 callback function


## -description


Used to transform encrypted data.


## -parameters




### -param hDrvDevice

The device being processed.


### -param Operation

The transform operation being performed.


### -param *pOutputArguments [in]

The output arguments for the transform being performed.


### -param *pInputArguments [in]

The input arguments for the transform being performed.


## -returns



Returns STATUS_SUCCESS if completed successfully.



