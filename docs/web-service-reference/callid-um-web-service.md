---
title: CallId (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- CallId
api_type:
- schema
ms.assetid: 2e044109-8bf3-488c-a654-459ac62fa1e7
description: CallId 要素には、GetCallInfo (UM web サービス) 要求または Disconnect (UM web サービス) 要求の呼び出しの識別子を表す値が含まれています。
ms.openlocfilehash: 5d5f596d4a98cbfb4b53be04278dae2305fc10c3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529456"
---
# <a name="callid-um-web-service"></a>CallId (UM web サービス)

**Callid**要素には、 [Getcallinfo (um web サービス)](getcallinfo-um-web-service.md)要求または[Disconnect (um web サービス)](disconnect-um-web-service.md)要求の呼び出しの識別子を表す値が含まれています。 
  
[GetCallInfo (UM web サービス)](getcallinfo-um-web-service.md)
  
[CallId (UM web サービス)](callid-um-web-service.md)
  
[Disconnect (UM web サービス)](disconnect-um-web-service.md)
  
[CallId (UM web サービス)](callid-um-web-service.md)
  
```xml
<CallId/>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetCallInfo (UM web サービス)](getcallinfo-um-web-service.md) <br/> |呼び出しに関する情報を取得するための要求を定義します。  <br/> |
|[Disconnect (UM web サービス)](disconnect-um-web-service.md) <br/> |呼び出しを切断する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は、呼び出しの識別子を表します。
  
## <a name="remarks"></a>注釈

最初の呼び出しを開始するには、 [Playonphone 操作 (um web サービス)](playonphone-operation-um-web-service.md)または[Playonphone 機の案内応答操作 (um web サービス)](playonphonegreeting-operation-um-web-service.md)を使用します。 [PlayOnPhoneResponse (um web サービス)](playonphoneresponse-um-web-service.md)要素または[PlayOnPhoneGreetingResponse (um web サービス)](playonphonegreetingresponse-um-web-service.md)要素で、 **callid**要素のテキスト値として返されるテキスト値を使用します。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)
  
[Disconnect 操作 (UM web サービス)](disconnect-operation-um-web-service.md)
  
[PlayOnPhone 操作 (UM web サービス)](playonphone-operation-um-web-service.md)
  
[Playon電話案内応答操作 (UM web サービス)](playonphonegreeting-operation-um-web-service.md)

