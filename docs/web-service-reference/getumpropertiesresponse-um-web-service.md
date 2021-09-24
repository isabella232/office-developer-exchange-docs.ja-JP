---
title: GetUMPropertiesResponse (UM Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- GetUMPropertiesResponse
api_type:
- schema
ms.assetid: fcd93ce5-7403-46a9-b46e-56d2ebdd2f79
description: GetUMPropertiesResponse 要素は、GetUMProperties 操作 (UM Web サービス) 要求への応答を定義します。
ms.openlocfilehash: 97c3850d46369d4ab533629a8b24e199db3dd44a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522965"
---
# <a name="getumpropertiesresponse-um-web-service"></a>GetUMPropertiesResponse (UM Web サービス)

**GetUMPropertiesResponse** 要素は [、GetUMProperties 操作 (UM Web サービス)](getumproperties-operation-um-web-service.md)要求への応答を定義します。 
  
[GetUMPropertiesResponse (UM Web サービス)](getumpropertiesresponse-um-web-service.md)
  
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
|[MissedCallNotificationEnabled (UM Web サービス)](missedcallnotificationenabled-um-web-service.md) <br/> |欠けている通話通知が有効かどうかを示します。  <br/> |
|[PlayOnPhoneDialString (UM Web サービス)](playonphonedialstring-um-web-service.md) <br/> |[PlayOnPhone](playonphone-operation-um-web-service.md)操作 (UM Web サービス) および[PlayOnPhoneGreeting](playonphonegreeting-operation-um-web-service.md)操作 (UM Web サービス) に使用する既定のダイヤル文字列が含まれます。  <br/> |
|[TelephoneAccessNumbers (UM Web サービス)](telephoneaccessnumbers-um-web-service.md) <br/> |ユーザーが電話を介してユニファイド メッセージングにアクセスするために使用できる電話番号の一覧を格納します。  <br/> |
|[TelephoneAccessFolderEmail (UM Web サービス)](telephoneaccessfolderemail-um-web-service.md) <br/> |ユニファイド メッセージングが電話でメッセージを読み取る電子メール フォルダーの識別子を格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUMProperties 操作 (UM Web サービス)](getumproperties-operation-um-web-service.md)

