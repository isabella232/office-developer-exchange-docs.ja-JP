---
title: EmailAddress (非 Emptystringtype)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- EmailAddress
api_type:
- schema
ms.assetid: c0c708d1-b016-4902-a294-9af44aea2050
description: EmailAddress 要素は、メールボックスユーザーのプライマリ SMTP アドレスを定義します。
ms.openlocfilehash: fcc3e650d5fc32344022ed6f015d4096a4461f63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463133"
---
# <a name="emailaddress-nonemptystringtype"></a>EmailAddress (非 Emptystringtype)

**EmailAddress**要素は、メールボックスユーザーのプライマリ SMTP アドレスを定義します。 
  
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
|[ActingAs](actingas.md) <br/> |発信者が送信者として送信しているユーザーを識別します。  <br/> |
|[メールボックス](mailbox.md) <br/> | 完全に解決された電子メールアドレスを識別します。  <br/><br/>この要素のいくつかの XPath 式を次に示します。<br/><br/>`/CreateItem/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`/CreateFolder/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`CreateItem/Items/AcceptItem/ToRecipients/Mailbox`<br/><br/>`SyncFolderItemsResponseMessage/Changes/Create/CalendarItem/ConflictingMeetings/AcceptItem/CcRecipients/Mailbox`<br/><br/>Mailbox 要素の追加の親要素は次のとおりです。<br/><br/>- [BccRecipients](bccrecipients.md) <br/>- [ReplyTo](replyto.md) <br/>- [者](sender.md) <br/>- [差出人](from.md) <br/>- [者](organizer.md) <br/>- [DistinguishedFolderId](distinguishedfolderid.md) <br/>- [画質](resolution.md) <br/>- [DLExpansion 展開](dlexpansion.md) <br/>- [出席](attendee.md) <br/> |
|[RoomList](roomlist.md) <br/> |メールアドレスによって会議室のリストを識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

SMTP アドレスを表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

**EmailAddress**要素は、SMTP または従来の Exchange 識別名 (DN) アドレスを表すことができます。 **EmailAddress**要素は、唯一必要な[Mailbox](mailbox.md)要素です。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

