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
description: メールボックス要素では、メールが有効な Active Directory のオブジェクトを識別します。
ms.openlocfilehash: e9fa21f3678249a9ac13d567b88beaf0177f989f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832258"
---
# <a name="mailbox"></a>メールボックス

**メールボックス**要素では、メールが有効な Active Directory のオブジェクトを識別します。 
  
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

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[名 (EmailAddressType)](name-emailaddresstype.md) <br/> |メールボックス ユーザーの名前を定義します。 この要素はオプションです。  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |メールボックスのユーザーの簡易メール転送プロトコル (SMTP) アドレスを定義します。 この要素はオプションです。  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |メールボックスに使用されるルーティングを定義します。 既定値は、SMTP です。 この要素はオプションです。  <br/> |
|[MailboxType](mailboxtype.md) <br/> |メールボックスのユーザーのメールボックスの種類を定義します。 この要素はオプションです。  <br/> |
|[ItemId](itemid.md) <br/> |ユーザーのアドレス帳フォルダーから受信者の連絡先または個人用配布リストの項目の識別子を定義します。 この要素はオプションです。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ExpandDL](expanddl.md) <br/> |配布リストを展開するための要求を定義します。 <br/> <br/> この要素への XPath 式は、次のようにします。` /ExpandDL ` <br/> |
|[ToRecipients](torecipients.md) <br/> |アイテムの受信者の配列が含まれています。  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |メッセージのコピーを受け取る受信者のコレクションを表します。  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |電子メールのブラインド カーボン コピー (Bcc) を受信する受信者のコレクションを表します。  <br/> |
|[ReplyTo](replyto.md) <br/> |応答を送信する電子メール アドレスの配列を指定します。  <br/> |
|[送信者](sender.md) <br/> |アイテムの送信者を識別します。  <br/> |
|[From](from.md) <br/> |メッセージの送信元アドレスを表します。  <br/> |
|[Organizer](organizer.md) <br/> |会議の開催者を表します。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> | Microsoft Exchange Server 2007 の既定のフォルダーを識別します。  <br/><br/>  この要素への XPath 式は、次のように。 <br/> <br/>  `/CreateItem/ParentFolderId/DistinguishedFolderId` <br/>  `/CreateFolder/ParentFolderId/DistinguishedFolderId` <br/> |
|[解決策](resolution.md) <br/> |解決された 1 つのエンティティが含まれています。  <br/> |
|[DLExpansion](dlexpansion.md) <br/> |配布リストに含まれているメールボックスの配列が含まれています。  <br/> |
|[Attendee](attendee.md) <br/> |出席者とリソースの予定表アイテムを表します。  <br/> |
|[CreateManagedFolder](createmanagedfolder.md) <br/> |メールボックスに管理フォルダーを追加する要求を定義します。  <br/> |
|[AddDelegate](adddelegate.md) <br/> |メールボックスに代理人を追加する要求を定義します。  <br/> |
|[GetDelegate](getdelegate.md) <br/> |メールボックスに代理人についての情報を取得する要求を定義します。  <br/> |
|[RemoveDelegate](removedelegate.md) <br/> |メールボックスからデリゲートを削除する要求を定義します。  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |メールボックスに代理人を更新する要求を定義します。  <br/> |
|[ReceivedBy](receivedby.md) <br/> |代理人アクセス シナリオでは、デリゲートをについて説明します。  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |代理人アクセスのシナリオでプリンシパルについて説明します。  <br/> |
|[メンバー](member-ex15websvcsotherref.md) <br/> |配布リストのメンバーを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)と[アイテム Id](itemid.md)要素は、メールボックスまたは配布リストを識別します。 

[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)の要素では、SMTP アドレスを使用してメールボックスまたは配布リストを識別します。 

[アイテム Id](itemid.md)要素は、特定のメールボックスに関連付けられている項目の識別子で、メールボックスを識別します。 

[アイテム Id](itemid.md)要素は、配布リスト、またはパブリックの連絡先フォルダーの連絡先にメッセージを送信するのには使用できません。 連絡先パブリック フォルダーの連絡先または配布リストにメッセージを送信しようとしましたがときに、createitem メソッド、UpdateItem、または SendItem 操作で使用される場合は、エラーがスローされます。 SMTP アドレスを取得し、[アイテム Id](itemid.md)の要素ではなく、 [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)の要素を使用してメッセージを送信するには、ExpandDL 操作を使用します。 
  
[(可用性) のメールボックス](mailbox-availability.md)、別の要素では、可用性の操作に関する情報を提供します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

