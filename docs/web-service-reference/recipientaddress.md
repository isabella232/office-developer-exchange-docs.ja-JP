---
title: RecipientAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RecipientAddress
api_type:
- schema
ms.assetid: 9ae6351a-2c60-4715-a489-5681a13641f9
description: RecipientAddress 要素は、受信者のメールボックスを表します。
ms.openlocfilehash: 23fdf9b1b340aac2049229f27d63161c8e05b10b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527650"
---
# <a name="recipientaddress"></a>RecipientAddress

**RecipientAddress 要素** は、受信者のメールボックスを表します。 
  
```xml
<RecipientAddress>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientAddress>
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
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |メールボックス ユーザーの簡易メール転送プロトコル (SMTP) アドレスを定義します。 この要素は省略できます。  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |受信者のルーティング プロトコルを表します。 既定値は SMTP です。 この要素は省略できます。  <br/> |
|[MailboxType](mailboxtype.md) <br/> |電子メール アドレスで表されるメールボックスの種類を表します。  <br/> |
|[ItemId](itemid.md) <br/> |ユーザーの連絡先フォルダーからの受信者の連絡先またはプライベート配布リストのアイテム識別子を定義します。 この要素は省略できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[メールヒント](mailtips.md) <br/> |さまざまな種類のメール ヒントの値を表します。  <br/> |
   
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



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

