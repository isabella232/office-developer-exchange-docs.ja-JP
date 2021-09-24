---
title: RecipientFilter
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RecipientFilter
api_type:
- schema
ms.assetid: 956c287a-a38a-49a7-a877-6d2088dfbc06
description: RecipientFilter 要素は、指定したメッセージ追跡レポートで使用する受信者アドレスを表します。
ms.openlocfilehash: bae574f83ca05a6c91c328909877d8c685849737
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534522"
---
# <a name="recipientfilter"></a>RecipientFilter

**RecipientFilter 要素は**、指定したメッセージ追跡レポートで使用する受信者アドレスを表します。 
  
```XML
 <RecipientFilter>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientFilter>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Name (EmailAddressType)](name-emailaddresstype.md) <br/> |メールボックス ユーザーの名前を表します。 この要素は省略できます。  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |メールボックス ユーザーのプライマリ簡易メール転送プロトコル (SMTP) アドレスを定義します。 この要素は省略できます。  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |この受信者のルーティング プロトコルを表します。 既定値は SMTP です。 この要素は省略できます。  <br/> |
|[MailboxType](mailboxtype.md) <br/> |電子メール アドレスで表されるメールボックスの種類を表します。 この要素は省略できます。  <br/> |
|[ItemId](itemid.md) <br/> |ユーザーの連絡先フォルダーの受信者の連絡先またはプライベート配布リストのアイテム識別子を定義します。 この要素は省略できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetMessageTrackingReport](getmessagetrackingreport.md) <br/> |指定した ID の完全なメッセージ追跡レポートを取得する [GetMessageTrackingReport](getmessagetrackingreport-operation.md) 操作の要求を格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

