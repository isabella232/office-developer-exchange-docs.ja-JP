---
title: EmailAddress (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cdabfcb-7658-4c7d-bb03-1e776ed11e43
description: EmailAddress 要素は、サイトのメールボックス、または、関連付けられているため完全に解決済みの SMTP アドレスを指定します。
ms.openlocfilehash: c31a37fc0dbdcc2b501b82346a17a0a3b4775556
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760216"
---
# <a name="emailaddress-emailaddresstype"></a>EmailAddress (EmailAddressType)

**EmailAddress**要素は、サイトのメールボックス、または、関連付けられているため完全に解決済みの SMTP アドレスを指定します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[名 (文字列)](name-string.md) <br/> |検索の絞り込み条件の名前またはキー、または、電子メール ユーザーの名前を指定します。  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |メールボックスのユーザーのプライマリ SMTP アドレスを定義します。  <br/> |
|[RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) <br/> |電子メール アドレスのルーティングの種類を指定します。  <br/> |
|[MailboxType](mailboxtype.md) <br/> |電子メール アドレスで表されるメールボックスの種類を表します。  <br/> |
|[ItemId](itemid.md) <br/> |Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ペルソナ](persona.md) <br/> |**GetPersona**の要求によって返されるペルソナ データのセットを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素はオプションです。
  
**EmailAddress**要素は、オンラインの Exchange および Exchange 2013 を起動する Microsoft Exchange Server のバージョンを対象とするクライアントに適用されます。 
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

