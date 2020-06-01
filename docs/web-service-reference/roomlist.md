---
title: RoomList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoomList
api_type:
- schema
ms.assetid: cb02bdf0-df9f-4e31-b7dd-cd9f2f2cc2b2
description: RoomList 要素は、会議室の一覧を識別する電子メールアドレスを表します。
ms.openlocfilehash: 0444475cb9fffbb89ba2861096baee0c7e645995
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460520"
---
# <a name="roomlist"></a>RoomList

**RoomList**要素は、会議室の一覧を識別する電子メールアドレスを表します。 
  
[GetRooms](getrooms.md)
  
[RoomList](roomlist.md)
  
```XML
<RoomList>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RoomList>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Name (EmailAddressType)](name-emailaddresstype.md) <br/> |会議室一覧の表示名を定義します。 この要素は省略できます。  <br/> |
|[EmailAddress (非 Emptystringtype)](emailaddress-nonemptystringtype.md) <br/> |会議室一覧の簡易メール転送プロトコル (SMTP) アドレスを定義します。 この要素は省略できます。  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |メールボックスに使用されるルーティングを定義します。 既定値は SMTP です。 この要素は省略できます。  <br/> |
|[MailboxType](mailboxtype.md) <br/> |メールボックスユーザーのメールボックスの種類を定義します。 この要素は省略できます。  <br/> |
|[ItemId](itemid.md) <br/> |ユーザーの連絡先フォルダーにある受信者の連絡先またはプライベート配布リストのアイテム識別子を定義します。 この要素は省略できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetRooms](getrooms.md) <br/> |特定の会議室リスト内のルームのリストを取得する要求のルート要素。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetRooms 操作](getrooms-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

