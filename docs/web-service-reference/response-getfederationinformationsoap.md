---
title: Response (GetFederationInformation) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: ca48a4b3-5006-4bb7-973e-d9137ce67e16
description: Response 要素には、GetFederationInformation 操作 (SOAP) 応答情報が含まれる。
ms.openlocfilehash: b5618dc1d2c862e504ea3134b28edca39c71f62c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523525"
---
# <a name="response-getfederationinformation-soap"></a>Response (GetFederationInformation) (SOAP)

**Response 要素** には [、GetFederationInformation 操作 (SOAP) 応答情報が](getfederationinformation-operation-soap.md)含まれる。 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <ApplicationUri/>
   <Domains/>
</Response>
```

 **GetFederationInformationResponse**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |自動検出サービスによって返されるエラー コードを表します。  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |自動検出サービスによって返されるエラー コードに関連付けられているメッセージを表します。  <br/> |
|[ApplicationUri (SOAP)](applicationuri-soap.md) <br/> |アプリケーションの場所を定義します。  <br/> |
|[Domains (SOAP)](domains-soap.md) <br/> |[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)で返される構成、または組織が[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)でフェデレーションしたドメインで返されるドメイン コレクションを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetFederationInformationResponseMessage (SOAP)](getfederationinformationresponsemessage-soap.md) <br/> |[GetFederationInformation 操作 (SOAP) 要求への応答を定義](getfederationinformation-operation-soap.md)します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)

