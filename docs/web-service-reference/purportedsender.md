---
title: PurportedSender
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PurportedSender
api_type:
- schema
ms.assetid: eb7a54ec-2e48-4030-bbcf-50a31609691b
description: PurportedSender 要素には、電子メールメッセージの申し立て sender の連絡先情報が含まれています。
ms.openlocfilehash: 5ecf352484a423e3955736620bf5a65c4e98099a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468335"
---
# <a name="purportedsender"></a>PurportedSender

**PurportedSender**要素には、電子メールメッセージの申し立て sender の連絡先情報が含まれています。 
  
```XML
<PurportedSender>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</PurportedSender>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Name (EmailAddressType)](name-emailaddresstype.md) <br/> |メールボックスユーザーの名前を表します。 この要素は省略できます。  <br/> |
|[EmailAddress (非 Emptystringtype)](emailaddress-nonemptystringtype.md) <br/> |メールボックスユーザーの簡易メール転送プロトコル (SMTP) アドレスを定義します。 この要素は省略できます。  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |受信者のルーティングプロトコルを表します。 既定値は SMTP です。 この要素は省略できます。  <br/> |
|[MailboxType](mailboxtype.md) <br/> |電子メールアドレスによって表されるメールボックスの種類を表します。 この要素は省略できます。  <br/> |
|[ItemId](itemid.md) <br/> |ユーザーの連絡先フォルダーにある受信者の連絡先またはプライベート配布リストのアイテム識別子を定義します。 この要素は省略できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindMessageTrackingReport](findmessagetrackingreport.md) <br/> |検索するメッセージの種類の条件を指定します。  <br/> |
|[および search-messagetrackingreport](messagetrackingreport.md) <br/> |[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)で返される1つのメッセージを格納します。  <br/> |
|[MessageTrackingSearchResult](messagetrackingsearchresult.md) <br/> |[Findmessagetrackingreportresponse](findmessagetrackingreportresponse.md)要素の単一メッセージ結果を格納します。  <br/> |
   
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



[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

