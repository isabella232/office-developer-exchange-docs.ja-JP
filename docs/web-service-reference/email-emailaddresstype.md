---
title: Email (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Email
api_type:
- schema
ms.assetid: dfffa1d5-2c3c-4f56-af63-5853df462e58
description: Email 要素は、GetUserAvailability クエリのメールボックス ユーザーを表します。
ms.openlocfilehash: 1176eeaac47e27971683d025beec29c1710432a1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513018"
---
# <a name="email-emailaddresstype"></a>Email (EmailAddressType)

**Email 要素** は、GetUserAvailability クエリのメールボックス ユーザーを表します。 
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)  
- [MailboxDataArray](mailboxdataarray.md) 
- [MailboxData](mailboxdata.md) 
- [Email (EmailAddressType)](email-emailaddresstype.md)
  
```xml
<Email>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Email>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Name (EmailAddress)](name-emailaddress.md) <br/> |メールボックス ユーザーの表示名を表します。  <br/> |
|[Address (string)](address-string.md) <br/> |メールボックス ユーザーの電子メール アドレスを表します。  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |メッセージのルーティング プロトコルを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MailboxData](mailboxdata.md) <br/> |個々のメールボックス ユーザーと、メールボックス ユーザーに関して返されるデータの種類のオプションを表します。  <br/> 次に、この要素の XPath を示します。  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの /EWS/ ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserAvailability 操作](getuseravailability-operation.md)  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [ユーザーの可用性の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

