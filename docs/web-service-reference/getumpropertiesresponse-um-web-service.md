---
title: GetUMPropertiesResponse (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetUMPropertiesResponse
api_type:
- schema
ms.assetid: fcd93ce5-7403-46a9-b46e-56d2ebdd2f79
description: GetUMPropertiesResponse 要素は、GetUMProperties の操作 (UM web サービス) 要求に対する応答を定義します。
ms.openlocfilehash: c0df872ad6b8e6541fa750ab87f4c1e5f0118b00
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831685"
---
# <a name="getumpropertiesresponse-um-web-service"></a>GetUMPropertiesResponse (UM web サービス)

**GetUMPropertiesResponse**要素は、 [GetUMProperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)要求に対する応答を定義します。 
  
[GetUMPropertiesResponse (UM web サービス)](getumpropertiesresponse-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
  <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 **UMProperties**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[MissedCallNotificationEnabled (UM web サービス)](missedcallnotificationenabled-um-web-service.md) <br/> |不在着信通知が有効になっているかどうかを示します。  <br/> |
|[PlayOnPhoneDialString (UM web サービス)](playonphonedialstring-um-web-service.md) <br/> |[PlayOnPhone 操作 (UM web サービス)](playonphone-operation-um-web-service.md)と[PlayOnPhoneGreeting (UM web サービス) の操作](playonphonegreeting-operation-um-web-service.md)に使用する既定のダイヤル文字列が含まれています。  <br/> |
|[TelephoneAccessNumbers (UM web サービス)](telephoneaccessnumbers-um-web-service.md) <br/> |電話を使用してユニファイド メッセージングにアクセスするユーザーが使用できる電話番号の一覧が含まれています。  <br/> |
|[TelephoneAccessFolderEmail (UM web サービス)](telephoneaccessfolderemail-um-web-service.md) <br/> |ユニファイド メッセージングはの読み取り元のメッセージに電話、電子メール フォルダーの識別子が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUMProperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)

