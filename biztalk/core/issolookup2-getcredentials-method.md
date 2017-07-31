---
title: "ISSOLookup2.GetCredentials Method | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 2e919858-90ba-4c72-98b6-cd37722aeae8
caps.latest.revision: 5
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# ISSOLookup2.GetCredentials Method
The **GetCredentials** method retrieves the user credentials for an application.  
  
## Syntax  
  
```cpp#  
  
HRESULT GetCredentials(  
BSTR bstrApplicationName,  
LONG lFlags,  
BSTR* pbstrExternalUserName,  
SAFEARRAY credentials  
);  
```  
  
```vb  
  
Function GetCredentials(  
bstrApplicationName As String,  
lFlags As Long,  
pbstrExternalUserName As String  
)  
As String  
```  
  
#### Parameters  
 `bstrApplicationName`  
 [in]  String that specifies the application name. This parameter cannot be NULL, an empty string, or contain spaces. Application names are not case-sensitive, but case will be preserved. For example, ABC, abc, and AbC are considered to be the same application.  
  
 `bstrApplicationName`  
 [in]  String that specifies the application name. This parameter cannot be NULL, an empty string, or contain spaces. Application names not case-sensitive, but case will be preserved. For example, ABC, abc, and AbC are considered to be the same application.  
  
 `lFlags`  
 [in]  Long integer that specifies the flags to set. Using the SSO_FLAG_REFRESH indicates that the credential cache should be bypassed.  
  
 `lFlags`  
 [in]  Long that specifies the flags to set. Using the SSO_FLAG_REFRESH indicates that the credential cache should be bypassed.  
  
 `pbstrExternalUserName`  
 [out]  Pointer to a string that receives the external user name.  
  
 `pbstrExternalUserName`  
 [out]  String that receives the external user name.  
  
 `credentials`  
 [out]  String array that receives the credentials.  
  
## Return Value  
 This method returns an HRESULT indicating whether it completed successfully. For more details, see the Error Values section.  
  
 String array that receives the credentials.  
  
## Error Values  
 This method returns an HRESULT containing one of the values in the following table.  
  
 This method indicates errors by setting the Number property of the global Err object to one of the values in the following table.  
  
|Value|Description|  
|-----------|-----------------|  
|S_OK|The method succeeded.|  
|E_ACCESSDENIED|Access is denied to the caller.|  
|E_INVALIDARG|An invalid parameter was detected.|  
  
## Remarks  
 To access this method, you must be an Application User. You can only retrieve your own credential.  
  
## Requirements  
 **Platforms:**  [!INCLUDE[btsPlatformsComApis](../includes/btsplatformscomapis-md.md)]  
  
## See Also  
 [ISSOLookup2 Interface (COM)](../core/issolookup2-interface-com.md)   
 [ISSOLookup2 Members](../core/issolookup2-members.md)   
 [Programming with Enterprise Single Sign-On](../core/programming-with-enterprise-single-sign-on.md)