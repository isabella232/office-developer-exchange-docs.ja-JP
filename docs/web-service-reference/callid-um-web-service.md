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
description: CallId 要素には、GetCallInfo (UM web サービス) の要求または切断 (UM web サービス) 要求の呼び出しの id を表す値が含まれています。
ms.openlocfilehash: 49690f41b9a002b05c7c9b1a1240073c7230ab92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759604"
---
# <a name="callid-um-web-service"></a>CallId (UM web サービス)

**CallId**要素には、 [GetCallInfo (UM web サービス)](getcallinfo-um-web-service.md)の要求または[切断 (UM web サービス)](disconnect-um-web-service.md)要求の呼び出しの id を表す値が含まれています。 
  
[GetCallInfo (UM web サービス)](getcallinfo-um-web-service.md)
  
[CallId (UM web サービス)](callid-um-web-service.md)
  
[(UM web サービス) に接続を切断します。](disconnect-um-web-service.md)
  
[CallId (UM web サービス)](callid-um-web-service.md)
  
```xml
<CallId/>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetCallInfo (UM web サービス)](getcallinfo-um-web-service.md) <br/> |呼び出しに関する情報を取得する要求を定義します。  <br/> |
|[(UM web サービス) に接続を切断します。](disconnect-um-web-service.md) <br/> |呼び出しの切断要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は、呼び出しの id を表します。
  
## <a name="remarks"></a>備考

最初の呼び出しを[PlayOnPhone 操作 (UM web サービス)](playonphone-operation-um-web-service.md)または[PlayOnPhoneGreeting 操作 (UM web サービス)](playonphonegreeting-operation-um-web-service.md)を使用します。 **CallId**要素のテキスト値の[PlayOnPhoneResponse (UM web サービス)](playonphoneresponse-um-web-service.md)または[PlayOnPhoneGreetingResponse (UM web サービス)](playonphonegreetingresponse-um-web-service.md)の要素で返される文字列値を使用します。 
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)
  
[操作 (UM web サービス) に接続を切断します。](disconnect-operation-um-web-service.md)
  
[PlayOnPhone 操作 (UM web サービス)](playonphone-operation-um-web-service.md)
  
[PlayOnPhoneGreeting 操作 (UM web サービス)](playonphonegreeting-operation-um-web-service.md)

