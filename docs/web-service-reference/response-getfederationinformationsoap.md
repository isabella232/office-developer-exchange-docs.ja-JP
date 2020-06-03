---
title: Response (GetFederationInformation) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ca48a4b3-5006-4bb7-973e-d9137ce67e16
description: Response 要素には、GetFederationInformation operation (SOAP) 応答情報が含まれています。
ms.openlocfilehash: 0b9a2c518b968faa6ef86b7c1f544eac40f8e5c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530587"
---
# <a name="response-getfederationinformation-soap"></a>Response (GetFederationInformation) (SOAP)

**Response**要素には、 [GETFEDERATIONINFORMATION operation (SOAP)](getfederationinformation-operation-soap.md)応答情報が含まれています。 
  
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
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |自動検出サービスによって返されるエラーコードを表します。  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |自動検出サービスによって返されるエラーコードに関連付けられているメッセージを表します。  <br/> |
|[ApplicationUri (SOAP)](applicationuri-soap.md) <br/> |アプリケーションの場所を定義します。  <br/> |
|[Domains (SOAP)](domains-soap.md) <br/> |は、 [Getdomainsettings 操作 (soap)](getdomainsettings-operation-soap.md)で返される構成、または組織が[GETFEDERATIONINFORMATION 操作 (soap)](getfederationinformation-operation-soap.md)でフェデレーションしたドメインのドメインコレクションを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetFederationInformationResponseMessage (SOAP)](getfederationinformationresponsemessage-soap.md) <br/> |[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)要求に対する応答を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)

