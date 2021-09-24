---
title: EmailAddress (NonEmptyStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- EmailAddress
api_type:
- schema
ms.assetid: c0c708d1-b016-4902-a294-9af44aea2050
description: EmailAddress 要素は、メールボックス ユーザーのプライマリ SMTP アドレスを定義します。
ms.openlocfilehash: 8740f6f7f67269de86aaa7383a7ad8f3cdf07a4a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512997"
---
# <a name="emailaddress-nonemptystringtype"></a>EmailAddress (NonEmptyStringType)

**EmailAddress 要素** は、メールボックス ユーザーのプライマリ SMTP アドレスを定義します。 
  
```XML
<EmailAddress/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ActingAs](actingas.md) <br/> |呼び出し元が送信するユーザーを識別します。  <br/> |
|[メールボックス](mailbox.md) <br/> | 完全に解決された電子メール アドレスを識別します。  <br/><br/>次に、この要素の XPath 式を示します。<br/><br/>`/CreateItem/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`/CreateFolder/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`CreateItem/Items/AcceptItem/ToRecipients/Mailbox`<br/><br/>`SyncFolderItemsResponseMessage/Changes/Create/CalendarItem/ConflictingMeetings/AcceptItem/CcRecipients/Mailbox`<br/><br/>Mailbox 要素の追加の親要素を次に示します。<br/><br/>- [BccRecipients](bccrecipients.md) <br/>- [ReplyTo](replyto.md) <br/>- [送信者](sender.md) <br/>- [差出人](from.md) <br/>- [オーガナイザー](organizer.md) <br/>- [DistinguishedFolderId](distinguishedfolderid.md) <br/>- [解決策](resolution.md) <br/>- [DLExpansion](dlexpansion.md) <br/>- [出席者](attendee.md) <br/> |
|[RoomList](roomlist.md) <br/> |電子メール アドレスで会議室の一覧を識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

SMTP アドレスを表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

**EmailAddress 要素は**、SMTP アドレスまたはレガシ Exchange識別名 (DN とも呼ばれる) アドレスを表します。 **EmailAddress 要素は**、唯一必要な [Mailbox 要素](mailbox.md)です。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

