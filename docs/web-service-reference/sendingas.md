---
title: SendingAs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendingAs
api_type:
- schema
ms.assetid: b43ce19f-9ab0-4946-acb2-c5aafead9d35
description: SendingAs 要素は、ユーザーが送信しようとする電子メール アドレスを表します。
ms.openlocfilehash: a5468ddb8facf99038d319252f7e1c780a888ca1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833338"
---
# <a name="sendingas"></a>SendingAs

**SendingAs**要素は、ユーザーが送信しようとする電子メール アドレスを表します。 
  
```XML
<SendingAs>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</SendingAs>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[名 (EmailAddressType)](name-emailaddresstype.md) <br/> |メールボックス ユーザーの名前を表します。 この要素はオプションです。  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |メールボックスのユーザーのプライマリ簡易メール転送プロトコル (SMTP) アドレスを定義します。 この要素はオプションです。  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |メールボックスのアドレスの種類を定義します。 既定値は、SMTP です。 この要素はオプションです。  <br/> |
|[MailboxType](mailboxtype.md) <br/> |電子メール ユーザーで表されるメールボックスの種類を表します。 この要素はオプションです。  <br/> |
|[ItemId](itemid.md) <br/> |ユーザーのアドレス帳フォルダーから受信者の連絡先または個人用配布リストの項目の識別子を定義します。 この要素はオプションです。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetMailTips](getmailtips.md) <br/> |受信者とメール ヒントの種類を取得するのにが含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

