---
title: メールボックス
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Mailbox
api_type:
- schema
ms.assetid: befc70fd-51cb-4258-884c-80c9050f0e82
description: Mailbox 要素は、メールが有効な Active Directory オブジェクトを識別します。
ms.openlocfilehash: 284c3ff6f9fece57611169a4ec41eeaa273c6ad3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468202"
---
# <a name="mailbox"></a>メールボックス

**Mailbox**要素は、メールが有効な Active Directory オブジェクトを識別します。 
  
```XML
<Mailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Mailbox>
```

**EmailAddressType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Name (EmailAddressType)](name-emailaddresstype.md) <br/> |メールボックスユーザーの名前を定義します。 この要素は省略できます。  <br/> |
|[EmailAddress (非 Emptystringtype)](emailaddress-nonemptystringtype.md) <br/> |メールボックスユーザーの簡易メール転送プロトコル (SMTP) アドレスを定義します。 この要素は省略できます。  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |メールボックスに使用されるルーティングを定義します。 既定値は SMTP です。 この要素は省略できます。  <br/> |
|[MailboxType](mailboxtype.md) <br/> |メールボックスユーザーのメールボックスの種類を定義します。 この要素は省略できます。  <br/> |
|[ItemId](itemid.md) <br/> |ユーザーの連絡先フォルダーにある受信者の連絡先またはプライベート配布リストのアイテム識別子を定義します。 この要素は省略できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ExpandDL](expanddl.md) <br/> |配布リストを展開するための要求を定義します。 <br/> <br/> この要素の XPath 式を次に示します。` /ExpandDL ` <br/> |
|[ToRecipients](torecipients.md) <br/> |アイテムの受信者の配列を格納します。  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |メッセージのコピーを受信する受信者のコレクションを表します。  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |電子メールのブラインドカーボンコピー (Bcc) を受信する受信者のコレクションを表します。  <br/> |
|[ReplyTo](replyto.md) <br/> |返信が送信される電子メールアドレスの配列を指定します。  <br/> |
|[Sender](sender.md) <br/> |アイテムの送信者を識別します。  <br/> |
|[From](from.md) <br/> |メッセージが送信された相手のアドレスを表します。  <br/> |
|[Organizer](organizer.md) <br/> |会議の開催者を表します。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> | Microsoft Exchange Server 2007 の既定のフォルダーを識別します。  <br/><br/>  この要素の XPath 式は次のとおりです。 <br/> <br/>  `/CreateItem/ParentFolderId/DistinguishedFolderId` <br/>  `/CreateFolder/ParentFolderId/DistinguishedFolderId` <br/> |
|[Resolution](resolution.md) <br/> |1つの解決済みエンティティを含みます。  <br/> |
|[DLExpansion 展開](dlexpansion.md) <br/> |配布リストに含まれているメールボックスの配列を格納します。  <br/> |
|[出席者](attendee.md) <br/> |予定表アイテムの出席者とリソースを表します。  <br/> |
|[CreateManagedFolder](createmanagedfolder.md) <br/> |メールボックスに管理フォルダーを追加する要求を定義します。  <br/> |
|[AddDelegate](adddelegate.md) <br/> |メールボックスに代理人を追加するための要求を定義します。  <br/> |
|[GetDelegate](getdelegate.md) <br/> |メールボックスへの代理人に関する情報を取得する要求を定義します。  <br/> |
|[RemoveDelegate](removedelegate.md) <br/> |メールボックスから代理人を削除するための要求を定義します。  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |メールボックスの代理人を更新する要求を定義します。  <br/> |
|[ReceivedBy](receivedby.md) <br/> |代理人アクセスのシナリオでのデリゲートについて説明します。  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |代理人アクセスシナリオのプリンシパルについて説明します。  <br/> |
|[メンバー](member-ex15websvcsotherref.md) <br/> |配布リストのメンバーを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

[EmailAddress (非 Emptystringtype)](emailaddress-nonemptystringtype.md)要素と[ItemId](itemid.md)要素は、メールボックスまたは配布リストを識別します。 

[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)要素は、SMTP アドレスによってメールボックスまたは配布リストを識別します。 

[ItemId](itemid.md)要素は、特定のメールボックスに関連付けられているアイテムの識別子によってメールボックスを識別します。 

[ItemId](itemid.md)要素を使用して、配布リストまたはパブリック連絡先フォルダー内の連絡先にメッセージを送信することはできません。 CreateItem、UpdateItem、または SendItem 操作で、連絡先パブリックフォルダーの配布リストまたは連絡先にメッセージを送信しようとすると、エラーがスローされます。 ExpandDL 操作を使用して SMTP アドレスを取得してから、 [ItemId](itemid.md)要素ではなく[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)要素を使用してメッセージを送信します。 
  
もう1つの要素である[メールボックス (可用性)](mailbox-availability.md)は、可用性の運用に関する情報を提供します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

