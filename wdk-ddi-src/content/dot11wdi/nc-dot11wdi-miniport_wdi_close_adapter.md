---
UID: NC:dot11wdi.MINIPORT_WDI_CLOSE_ADAPTER
title: MINIPORT_WDI_CLOSE_ADAPTER
author: windows-driver-content
description: The MiniportWdiCloseAdapter handler function is used by the Microsoft component to initiate the Close Task operation on the IHV driver.
old-location: netvista\miniportwdicloseadapter.htm
tech.root: netvista
ms.assetid: E6A96765-3D95-431B-B29A-5BD7641325A8
ms.author: windowsdriverdev
ms.date: 5/2/2018
ms.keywords: MINIPORT_WDI_CLOSE_ADAPTER, MINIPORT_WDI_CLOSE_ADAPTER callback, MiniportWdiCloseAdapter, MiniportWdiCloseAdapter callback function [Network Drivers Starting with Windows Vista], dot11wdi/MiniportWdiCloseAdapter, netvista.miniportwdicloseadapter
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: callback
req.header: dot11wdi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10
req.target-min-winversvr: Windows Server 2016
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
-	dot11wdi.h
api_name:
-	MiniportWdiCloseAdapter
product:
- Windows
targetos: Windows
req.typenames: 
---

# MINIPORT_WDI_CLOSE_ADAPTER callback function


## -description


The MiniportWdiCloseAdapter handler function is used by the Microsoft component to initiate the Close Task operation on the IHV driver.

This is a WDI miniport handler inside <a href="https://msdn.microsoft.com/library/windows/hardware/mt297617">NDIS_MINIPORT_DRIVER_WDI_CHARACTERISTICS</a>.

This call must complete quickly. If the close operation is successfully started, the IHV must return NDIS_STATUS_SUCCESS and call the WDI <a href="https://msdn.microsoft.com/42500F6F-8E97-454F-819F-8EA3785C0D04">CloseAdapterComplete</a> handler that was passed into <a href="https://msdn.microsoft.com/4CBC7230-6480-40C9-90B7-A286FCEB1FA8">MiniportWdiAllocateAdapter</a> with the <a href="https://msdn.microsoft.com/library/windows/hardware/mt297621">NDIS_WDI_INIT_PARAMETERS</a> structure.
<div class="alert"><b>Note</b>  You must declare the function by using the <b>MINIPORT_WDI_CLOSE_ADAPTER</b> type. For more
   information, see the following Examples section.</div><div> </div>

## -parameters




### -param MiniportAdapterContext [in]

The handle to the context area that the miniport driver allocated.


## -returns




            MiniportWdiCloseAdapter can return any of the following return values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>NDIS_STATUS_SUCCESS</b></dt>
</dl>
</td>
<td width="60%">
MiniportWdiCloseAdapter successfully completed.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>Other NDIS_STATUS codes</b></dt>
</dl>
</td>
<td width="60%">
An appropriate NDIS_STATUS code in the case of a failure.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/42500F6F-8E97-454F-819F-8EA3785C0D04">CloseAdapterComplete</a>



<a href="https://msdn.microsoft.com/4CBC7230-6480-40C9-90B7-A286FCEB1FA8">MiniportWdiAllocateAdapter</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/mt297617">NDIS_MINIPORT_DRIVER_WDI_CHARACTERISTICS</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/mt297621">NDIS_WDI_INIT_PARAMETERS</a>
 

 

