---
title: EmailAddress (NonEmptyStringType)
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
description: EmailAddress 要素は、メールボックスのユーザーのプライマリ SMTP アドレスを定義します。
ms.openlocfilehash: fcf2839c1e2e40a22d6b6a856608f52f2c9c2a1a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760223"
---
# <a name="emailaddress-nonemptystringtype"></a>EmailAddress (NonEmptyStringType)

**EmailAddress**要素は、メールボックスのユーザーのプライマリ SMTP アドレスを定義します。 
  
```XML
<EmailAddress/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ActingAs](actingas.md) <br/> |として送信する呼び出し元を識別します。  <br/> |
|[メールボックス](mailbox.md) <br/> | 完全に解決された電子メール アドレスを識別します。  <br/><br/>この要素にいくつかの XPath 式は、次のように。<br/><br/>`/CreateItem/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`/CreateFolder/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`CreateItem/Items/AcceptItem/ToRecipients/Mailbox`<br/><br/>`SyncFolderItemsResponseMessage/Changes/Create/CalendarItem/ConflictingMeetings/AcceptItem/CcRecipients/Mailbox`<br/><br/>メールボックス要素の他の親要素は、次のように。<br/><br/>- [BccRecipients](bccrecipients.md) <br/>- [ReplyTo](replyto.md) <br/>- [送信者](sender.md) <br/>- [差出人](from.md) <br/>- [開催者](organizer.md) <br/>- [DistinguishedFolderId](distinguishedfolderid.md) <br/>- [解像度](resolution.md) <br/>- [DLExpansion](dlexpansion.md) <br/>- [出席者](attendee.md) <br/> |
|[RoomList](roomlist.md) <br/> |電子メール アドレスを使用して会議室の一覧を識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

SMTP アドレスを表す文字列値は、必要があります。
  
## <a name="remarks"></a>備考

**EmailAddress**要素は、SMTP を表すことができますまたは従来の Exchange 識別名 (DN とも呼ばれます) のアドレスです。 **EmailAddress**要素は、唯一の必要な[メールボックス](mailbox.md)の要素です。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

