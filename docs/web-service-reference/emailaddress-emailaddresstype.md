---
title: EmailAddress (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0cdabfcb-7658-4c7d-bb03-1e776ed11e43
description: EmailAddress 要素は、サイト メールボックスまたは関連するペルサの完全に解決された SMTP アドレスを指定します。
ms.openlocfilehash: 76b279a82f6f277d9f231866437359ceae46df59
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545259"
---
# <a name="emailaddress-emailaddresstype"></a>EmailAddress (EmailAddressType)

**EmailAddress 要素** は、サイト メールボックスまたは関連するペルサの完全に解決された SMTP アドレスを指定します。 
  
```xml
<EmailAddress>
    <Name></Name>
    <EmailAddress></EmailAddress>
    <RoutingType></RoutingType>
    <MailboxType></MailboxType>
    <ItemId></ItemId>
</EmailAddress>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Name (文字列)](name-string.md) <br/> |検索絞り込み条件の名前またはキー、または電子メール ユーザーの名前を指定します。  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |メールボックス ユーザーのプライマリ SMTP アドレスを定義します。  <br/> |
|[RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) <br/> |電子メール アドレスのルーティングの種類を指定します。  <br/> |
|[MailboxType](mailboxtype.md) <br/> |電子メール アドレスで表されるメールボックスの種類を表します。  <br/> |
|[ItemId](itemid.md) <br/> |ストア内のアイテムの一意の識別子と変更キー Exchangeします。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ユーザー](persona.md) <br/> |**GetPersona** 要求によって返されるペルソナ データのセットを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素は省略できます。
  
**EmailAddress** 要素は、2013 年Exchange Online開始するクライアントとバージョンのMicrosoft Exchange ServerにExchangeです。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

