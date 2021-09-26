---
title: Address (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Address
api_type:
- schema
ms.assetid: 518641c8-7f6f-496c-86f9-341e7c1bb44c
description: Address 要素は、完全に解決された電子メール アドレスを表します。
ms.openlocfilehash: ff26a8d6de1e9bf36bb8dff5bc0141974220cf90
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546813"
---
# <a name="address-emailaddresstype"></a>Address (EmailAddressType)

**Address 要素** は、完全に解決された電子メール アドレスを表します。 
  
```XML
<Address>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Address >
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Name (EmailAddressType)](name-emailaddresstype.md) <br/> |メールボックス ユーザーの名前を定義します。 この要素は省略できます。  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |メールボックス ユーザーの簡易メール転送プロトコル (SMTP) アドレスを定義します。 この要素は省略できます。  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |メールボックスに使用されるルーティングを定義します。 既定値は SMTP です。 この要素は省略できます。  <br/> |
|[MailboxType](mailboxtype.md) <br/> |メールボックス ユーザーのメールボックスの種類を定義します。 この要素は省略できます。  <br/> |
|[ItemId](itemid.md) <br/> |ユーザーの連絡先フォルダーの受信者の連絡先またはプライベート配布リストのアイテム識別子を定義します。 この要素は省略できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[OriginalRecipients](originalrecipients.md) <br/> |追跡メッセージの元の受信者を表す電子メール アドレスのコレクションが含まれます。  <br/> |
|[RoomLists](roomlists.md) <br/> |組織内の会議室の一覧を含む。  <br/> |
|[SentToAddresses](senttoaddresses.md) <br/> |条件または例外を適用するために受信メッセージが送信される必要がある電子メール アドレスの一覧が含まれます。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md) 
- [GetRoomLists 操作](getroomlists-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

