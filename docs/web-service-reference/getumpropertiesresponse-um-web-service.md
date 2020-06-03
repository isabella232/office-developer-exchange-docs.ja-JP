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
description: GetUMPropertiesResponse 要素は、GetUMProperties 操作 (UM web サービス) 要求への応答を定義します。
ms.openlocfilehash: 3247489a305c694c10764d7a0c6f02b1fad51ebf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459126"
---
# <a name="getumpropertiesresponse-um-web-service"></a>GetUMPropertiesResponse (UM web サービス)

**Getumpropertiesresponse**要素は、 [getumproperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)要求への応答を定義します。 
  
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MissedCallNotificationEnabled (UM web サービス)](missedcallnotificationenabled-um-web-service.md) <br/> |不在着信通知を有効にするかどうかを示します。  <br/> |
|[PlayOnPhoneDialString (UM web サービス)](playonphonedialstring-um-web-service.md) <br/> |[Playonphone 操作 (um web サービス)](playonphone-operation-um-web-service.md)および[Playonphone 案内応答操作 (um web サービス)](playonphonegreeting-operation-um-web-service.md)に使用する既定のダイヤル文字列が含まれています。  <br/> |
|[受付電話番号 (UM web サービス)](telephoneaccessnumbers-um-web-service.md) <br/> |ユーザーが電話でユニファイドメッセージングにアクセスする際に使用できる電話番号の一覧が含まれています。  <br/> |
|[受付電話 Accessfolderemail (UM web サービス)](telephoneaccessfolderemail-um-web-service.md) <br/> |ユニファイドメッセージングが電話でメッセージを読み取る電子メールフォルダーの識別子が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUMProperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)

