---
title: EmailAddress (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cdabfcb-7658-4c7d-bb03-1e776ed11e43
description: EmailAddress 要素は、サイトメールボックスまたは関連するペルソナの完全に解決された SMTP アドレスを指定します。
ms.openlocfilehash: 8b04b75e91cc16be7f88c9a0ac08c5e36855056e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463462"
---
# <a name="emailaddress-emailaddresstype"></a>EmailAddress (EmailAddressType)

**EmailAddress**要素は、サイトメールボックスまたは関連するペルソナの完全に解決された SMTP アドレスを指定します。 
  
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
|[Name (string)](name-string.md) <br/> |検索絞り込み条件の名前またはキーまたはメールユーザーの名前を指定します。  <br/> |
|[EmailAddress (非 Emptystringtype)](emailaddress-nonemptystringtype.md) <br/> |メールボックスユーザーのプライマリ SMTP アドレスを定義します。  <br/> |
|[RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) <br/> |電子メールアドレスのルーティングの種類を指定します。  <br/> |
|[MailboxType](mailboxtype.md) <br/> |電子メールアドレスによって表されるメールボックスの種類を表します。  <br/> |
|[ItemId](itemid.md) <br/> |Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ユーザー](persona.md) <br/> |**Getpersona**要求によって返される一連のペルソナデータを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素は省略できます。
  
**EmailAddress**要素は、exchange Online および exchange 2013 以降のバージョンの Microsoft exchange Server を対象とするクライアントに適用されます。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

