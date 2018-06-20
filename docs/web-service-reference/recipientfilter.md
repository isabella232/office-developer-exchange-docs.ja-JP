---
title: RecipientFilter
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientFilter
api_type:
- schema
ms.assetid: 956c287a-a38a-49a7-a877-6d2088dfbc06
description: RecipientFilter 要素は、指定したメッセージ追跡レポートを使用する受信者のアドレスを表します。
ms.openlocfilehash: c31ed469132b110a690416b112d5e4e96e44c501
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832972"
---
# <a name="recipientfilter"></a>RecipientFilter

**RecipientFilter**要素は、指定したメッセージ追跡レポートを使用する受信者のアドレスを表します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[名 (EmailAddressType)](name-emailaddresstype.md) <br/> |メールボックス ユーザーの名前を表します。 この要素はオプションです。  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |メールボックスのユーザーのプライマリ簡易メール転送プロトコル (SMTP) アドレスを定義します。 この要素はオプションです。  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |この受信者へのルーティング プロトコルを表します。 既定値は、SMTP です。 この要素はオプションです。  <br/> |
|[MailboxType](mailboxtype.md) <br/> |電子メール アドレスで表されるメールボックスの種類を表します。 この要素はオプションです。  <br/> |
|[ItemId](itemid.md) <br/> |ユーザーのアドレス帳フォルダーから受信者の連絡先または個人用配布リストの項目の識別子を定義します。 この要素はオプションです。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetMessageTrackingReport](getmessagetrackingreport.md) <br/> |レポートを指定した ID の追跡を取得するために[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)の要求が含まれています  <br/> |
   
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



[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

