---
title: CallId (UM Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- CallId
api_type:
- schema
ms.assetid: 2e044109-8bf3-488c-a654-459ac62fa1e7
description: CallId 要素には、GetCallInfo (UM Web サービス) 要求または Disconnect (UM Web サービス) 要求の呼び出しの識別子を表す値が含まれる。
ms.openlocfilehash: c19f1061d81bf7683fd2c84fb1c6968826046be6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522033"
---
# <a name="callid-um-web-service"></a>CallId (UM Web サービス)

**CallId 要素には**[、GetCallInfo (UM Web サービス)](getcallinfo-um-web-service.md)要求または Disconnect [(UM Web サービス)](disconnect-um-web-service.md)要求の呼び出しの識別子を表す値が含まれる。 
  
[GetCallInfo (UM Web サービス)](getcallinfo-um-web-service.md)
  
[CallId (UM Web サービス)](callid-um-web-service.md)
  
[切断 (UM Web サービス)](disconnect-um-web-service.md)
  
[CallId (UM Web サービス)](callid-um-web-service.md)
  
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
|[GetCallInfo (UM Web サービス)](getcallinfo-um-web-service.md) <br/> |呼び出しに関する情報を取得する要求を定義します。  <br/> |
|[切断 (UM Web サービス)](disconnect-um-web-service.md) <br/> |呼び出しを切断する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は、呼び出しの識別子を表します。
  
## <a name="remarks"></a>注釈

通話を開始するには [、PlayOnPhone 操作 (UM Web サービス)](playonphone-operation-um-web-service.md) または [PlayOnPhoneGreeting 操作 (UM Web サービス) を使用します](playonphonegreeting-operation-um-web-service.md)。 **CallId** 要素のテキスト値には [、PlayOnPhoneResponse (UM Web サービス)](playonphoneresponse-um-web-service.md)または [PlayOnPhoneGreetingResponse (UM Web サービス)](playonphonegreetingresponse-um-web-service.md)要素で返されるテキスト値を使用します。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetCallInfo 操作 (UM Web サービス)](getcallinfo-operation-um-web-service.md)
  
[切断操作 (UM Web サービス)](disconnect-operation-um-web-service.md)
  
[PlayOnPhone 操作 (UM Web サービス)](playonphone-operation-um-web-service.md)
  
[PlayOnPhoneGreeting 操作 (UM Web サービス)](playonphonegreeting-operation-um-web-service.md)

