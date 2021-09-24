---
title: Mailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Mailbox
api_type:
- schema
ms.assetid: befc70fd-51cb-4258-884c-80c9050f0e82
description: Mailbox 要素は、メールが有効な Active Directory オブジェクトを識別します。
ms.openlocfilehash: 8065c0472c3b847d538422aa77cd93f75d919a9b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535004"
---
# <a name="mailbox"></a>Mailbox

**Mailbox 要素** は、メールが有効な Active Directory オブジェクトを識別します。 
  
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
|[Name (EmailAddressType)](name-emailaddresstype.md) <br/> |メールボックス ユーザーの名前を定義します。 この要素は省略できます。  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |メールボックス ユーザーの簡易メール転送プロトコル (SMTP) アドレスを定義します。 この要素は省略できます。  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |メールボックスに使用されるルーティングを定義します。 既定値は SMTP です。 この要素は省略できます。  <br/> |
|[MailboxType](mailboxtype.md) <br/> |メールボックス ユーザーのメールボックスの種類を定義します。 この要素は省略できます。  <br/> |
|[ItemId](itemid.md) <br/> |ユーザーの連絡先フォルダーからの受信者の連絡先またはプライベート配布リストのアイテム識別子を定義します。 この要素は省略できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ExpandDL](expanddl.md) <br/> |配布リストを展開する要求を定義します。 <br/> <br/> 次に、この要素の XPath 式を示します。 ` /ExpandDL ` <br/> |
|[ToRecipients](torecipients.md) <br/> |アイテムの受信者の配列を含む。  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |メッセージのコピーを受信する受信者のコレクションを表します。  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |電子メールのブラインド カーボン コピー (Bcc) を受信する受信者のコレクションを表します。  <br/> |
|[ReplyTo](replyto.md) <br/> |返信を送信する電子メール アドレスの配列を識別します。  <br/> |
|[Sender](sender.md) <br/> |アイテムの送信者を識別します。  <br/> |
|[From](from.md) <br/> |メッセージの送信先の住所を表します。  <br/> |
|[開催者](organizer.md) <br/> |会議の開催者を表します。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> | 2007 フォルダー Microsoft Exchange Server既定のフォルダーを識別します。  <br/><br/>  この要素の XPath 式を次に示します。 <br/> <br/>  `/CreateItem/ParentFolderId/DistinguishedFolderId` <br/>  `/CreateFolder/ParentFolderId/DistinguishedFolderId` <br/> |
|[解決策](resolution.md) <br/> |1 つの解決済みエンティティを含む。  <br/> |
|[DLExpansion](dlexpansion.md) <br/> |配布リストに含まれるメールボックスの配列を含む。  <br/> |
|[Attendee](attendee.md) <br/> |予定表アイテムの出席者とリソースを表します。  <br/> |
|[CreateManagedFolder](createmanagedfolder.md) <br/> |メールボックスに管理フォルダーを追加する要求を定義します。  <br/> |
|[AddDelegate](adddelegate.md) <br/> |メールボックスに代理人を追加する要求を定義します。  <br/> |
|[GetDelegate](getdelegate.md) <br/> |メールボックスへの代理人に関する情報を取得する要求を定義します。  <br/> |
|[RemoveDelegate](removedelegate.md) <br/> |メールボックスから代理人を削除する要求を定義します。  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |メールボックス内の代理人を更新する要求を定義します。  <br/> |
|[ReceivedBy](receivedby.md) <br/> |代理人アクセス シナリオの代理人について説明します。  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |代理人アクセス シナリオのプリンシパルについて説明します。  <br/> |
|[メンバー](member-ex15websvcsotherref.md) <br/> |配布リストのメンバーを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)要素と[ItemId](itemid.md)要素は、メールボックスまたは配布リストを識別します。 

[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)要素は、SMTP アドレスによってメールボックスまたは配布リストを識別します。 

[ItemId 要素](itemid.md)は、特定のメールボックスに関連付けられたアイテム識別子によってメールボックスを識別します。 

[ItemId 要素](itemid.md)は、配布リストまたはパブリック連絡先フォルダー内の連絡先にメッセージを送信するために使用できません。 メッセージを連絡先パブリック フォルダー内の配布リストまたは連絡先に送信しようとすると、CreateItem、UpdateItem、または SendItem 操作で使用すると、エラーがスローされます。 ExpandDL 操作を使用して SMTP アドレスを取得し[、ItemId](itemid.md)要素の代わりに[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)要素を使用してメッセージを送信します。 
  
別の要素 [である Mailbox (Availability)](mailbox-availability.md)は、可用性操作に関する情報を提供します。 
  
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

